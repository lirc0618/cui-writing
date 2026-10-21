# IEEE 图表技能集成与验收（cui-writing 2.1.0 起内置）

2026-10-21。用户提供 `drawio-academic-chatgpt.zip` 与 `ieee-figure-table-chatgpt.zip` 两个适配包，要求并入写作分身，迁移时仍只需一份 `cui-writing`。已作为内置流程放入 `references/workflows/`，并重新生成独立包；2.2.0 未改动这两个流程，只新增安装器与分发说明。

## 集成了什么

| 任务 | 内置流程 | 关键工具 |
|---|---|---|
| 架构/算法流程/控制拓扑，可编辑 | `drawio-academic-chatgpt` | `scripts/make_drawio.py`：JSON 节点边 → `.drawio`（XML） |
| 实验曲线、散点、分组柱状图 | `ieee-figure-table-chatgpt` | `scripts/plot_csv.py` + `vector_plot.py`：CSV → SVG/PDF |
| 表格与图注 | `ieee-figure-table-chatgpt` 的 workflow 规则 | 按真实数据生成，不自造测量 |

- 两个流程共 10 个文件，连同原有 10 个流程 75 个文件，合计 12 个流程、90 个工作流文件；入口仍是根目录唯一 `SKILL.md`，内部不产生第二个可发现技能。
- 绘图后端为纯 Python 标准库：自行解析 TrueType `cmap/hmtx`，生成带 `FontFile2` 嵌入字体的 Type0 PDF 和带 `@font-face` base64 的 SVG，不依赖 Matplotlib/Pandas。字体为包内 `LiberationSans-Regular.ttf`（SIL OFL 1.1，随包保留许可证）。
- 来源、原包 SHA-256、改动与字体版本记录在 `references/workflows/ieee-integration-provenance.json`；许可见 `NOTICE.md`。不是 IEEE 官方工具，版式以目标期刊现行要求为准。

## 本次实测（隔离环境）

将 `cui-writing` 单独复制到临时目录，用 `env -i /usr/bin/python3 -I -S` 运行，无同级 skill、无 site-packages。

|检查|结果|
|---|---|
|包完整性、12 个流程、61 份语料/742 选页|通过（`ok=true`；2.1.0 实测，2.2.0 复验相同）|
|`.drawio`：3 个带标签节点、2 条正确连接的边|通过|
|非法端点（指向不存在的节点）报错退出且不生成文件|通过|
|折线/散点/分组柱状图 PDF+SVG 导出|通过|
|PDF 嵌入字体（`/FontFile2`）、SVG 内嵌 `@font-face`|通过|
|缺测点在折线中保留断口，不插值|通过（同一序列被拆成两段）|
|对数轴绘图；非正数据被拒且不导出|通过|
|非数值、缺列等错误输入非零退出|通过|
|科学符号标签（如 `µJ`）由包内字体覆盖|通过|
|迁移后语料检索仍可用（J02 第 9 页整页回查）|通过|

数据均为刻意构造的 QA 样例，不代表任何研究结果。PDF 已用 Ghostscript 转 PNG 并抽取文本核对轴标签、刻度与图例；本机无 Poppler。

## 边界

- 内置 helper 是起点而非通用绘图引擎：误差条、多面板、特殊数学排版需按真实数据另写脚本，不冒充上游完整软件。
- PNG 需由宿主环境的渲染工具转换；未实际导出时不列为已交付。
- 不校验源论文的科学结论，也不构成 IEEE 合规认证。

验收明细：[IEEE技能集成验收.json](IEEE技能集成验收.json) · [独立技能验收](14-独立技能验收.md) · [使用说明第11节](崔老师写作分身-使用说明.md)
