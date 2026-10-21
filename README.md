# cui-writing · 崔老师写作分身

按崔爱娇（Aijiao Cui）论文的**论证结构、措辞选择与证据边界**起草、改写、润色学术论文的 Agent Skill，并附 IEEE 论文图表制作能力。

不是一个"模仿风格"的提示词。它把 61 份论文拆解成可检索的原文块、可执行的写作规则和明确的证据约束，用**ID + 页码**支撑每一条建议。

---

## 这是什么

| | |
|---|---|
| 类型 | Agent Skill（`SKILL.md` + 参考资料 + 标准库脚本） |
| 适配 | Codex、DeepSeek Harness、Claude Code 等支持 Agent Skills 的代理 |
| 依赖 | Python 3 标准库，**无第三方包** |
| 语料 | 61 份材料 / 742 个选页位置，逐页精读 |
| 版本 | 2.2.0 |

---

## 核心思路

普通"写得像某位教授"的做法有两个通病：模型只学会堆 however / hence，或者把源论文的数字和结论直接搬进新稿。

本技能反其道而行：

- **学论证，不学词频** —— 还原"工程矛盾 → 技术缺口 → 机制选择 → 收益与代价"的链条
- **禁止事实迁移** —— 源研究的数字、器件、实验、攻击结论不得进入用户新稿
- **区分可学与不可学** —— 原文的笔误、过强断言、OCR 错误被记为**反例**，不是要模仿的风格
- **每条建议可追溯** —— 必须给出语料 ID 与 PDF 页码

---

## 语料构成

| 类别 | 数量 | 在技能中的角色 |
|---|---:|---|
| 期刊论文 | 18 | 主要口吻参照：论证、机制解释、实验讨论 |
| 第一作者会议论文 | 15 | 压缩篇幅下的问题定位与贡献写法 |
| 指导的硕士论文 | 27 | 仅前两章，补长篇组织与综述结构 |
| 合著书籍章节 | 1 | 教学性实例、能力边界表述 |

归因分层使用：**24 篇第一作者**为主要参照，**10 篇合著**只补体裁，**27 篇学生论文**只提供结构证据，不假定为导师亲笔。

---

## 12 个内置流程

**写作**

| 流程 | 用途 |
|---|---|
| `tech-paper-template` | 梳理论证骨架，检查问题—挑战—模块—贡献是否对应 |
| `intro-drafter` | 引言起草与重组 |
| `paper-writer` | 其他章节与全文 |
| `paper-polish` | 忠实润色，保留科学含义 |

**IEEE 图表**

| 流程 | 用途 |
|---|---|
| `drawio-academic-chatgpt` | 生成可编辑 `.drawio` 架构 / 流程 / 拓扑图 |
| `ieee-figure-table-chatgpt` | CSV → 矢量 PDF/SVG，内置字体，纯标准库 |

**评估与流程**

`figure-designer` · `idea-evaluator` · `benchmark-paper-template` · `deep-research` · `rebuttal-guidance` · `pre-submission-reviewer`

---

## 证据规则举例

技能会主动拦截这些常见错误：

**数字不能换分母**
> 同样的 8076 额外门，在 pipelined AES 是 3.80%，在 iterative AES 是 31.66%。只摘 3.8% 是误导。

**观察不能升级为定理**
> 10⁶ 次随机测试零匹配，只能写 "none was observed under…"，不能写 "false positives are impossible"。

**收益必须带代价**
> J15 总体面积更低但 delay 略高；J16 前文面积总是更低、本文 timing 只有 23/38 更好，不能改写成"全面最优"。

**机制论证 ≠ 实测**
> C08 的功耗比例是器件数推算，不能改称实测。

**跨论文不能强行统一**
> J07/J11 与 J10 的 self-loop 行为规则并不相同，不建立"崔老师总用某个判据"。

---

## 安装

### 自动（推荐）

```bash
python3 scripts/install.py
```

默认装入 `~/.agents/skills/cui-writing` —— Codex 与 DeepSeek Harness 共同扫描的目录，装一次两边都能用。

```bash
python3 scripts/install.py --list      # 查看本机技能目录
python3 scripts/install.py --all       # 装入所有已存在目录
python3 scripts/install.py --dest DIR  # 指定目录
python3 scripts/install.py --dry-run   # 只看不动
```

### 手动

把整个 `cui-writing/` 文件夹放进任一技能目录，保留完整结构：

| 代理 | 目录 |
|---|---|
| Codex + DeepSeek Harness 共用 | `~/.agents/skills/` |
| DeepSeek Harness 专用 | `~/.dsh/skills/` |
| Codex 旧版 | `~/.codex/skills/` |
| Claude Code | `~/.claude/skills/` |

### 验证

```bash
cd ~/.agents/skills/cui-writing
python3 scripts/check_install.py
```

应输出 `"ok": true`、`"workflows": 12`、`"documents": 61`、`"selected_page_positions": 742`。

---

## 使用

```text
使用 $cui-writing，按崔老师的论证和口吻润色下面的 Introduction。
保留我的事实、数字、术语和引用，先调整逻辑，再修改措辞。
正文英文，修改说明中文。
```

内部执行顺序：读作者规则 → 按章节读组织规则 → 检索 2–3 条最相近原句块 → 核对 ID/页码/归因 → 动笔。

检索器可按章节、ID、页码、整页回查：

```bash
python3 scripts/find_examples.py --section discussion --query "overhead limitation" --limit 4
python3 scripts/find_examples.py --ids J02 --pages 9 --inspect-pages
```

---

## 目录结构

```
cui-writing/
├── SKILL.md                    # 唯一技能入口
├── INSTALL.md                  # 接收方安装说明
├── manifest.json               # 223 个文件的 SHA-256 清单
├── agents/openai.yaml          # UI 元数据
├── scripts/
│   ├── find_examples.py        # 语料检索
│   ├── check_install.py        # 完整性校验
│   └── install.py              # 跨代理安装器
├── assets/corpus/              # 61 份分页语料
└── references/
    ├── voice.md                # 作者口吻规则
    ├── sections.md             # 章节组织规则
    ├── corpus-status.json      # 范围、归因、精读状态
    ├── close-reading/          # 61 份逐篇精读笔记
    └── workflows/              # 12 个内置流程
```

---

## 本仓库内容

除技能本体外，本仓库保留了完整的学习过程记录：

- `01`–`02` 写作风格与措辞手册
- `03`–`09` 早期窗口学习阶段（历史记录，状态可能过时）
- `10` 全文精读与逐篇验收表
- `13` 期刊写法与跨文反例复核
- `14`–`15` 独立打包与 IEEE 集成验收
- `逐页精读覆盖.csv`、`精读核验.json` 等台账

**注意**：`03`–`09` 属于早期阶段，其中"待精读"等状态已被 `10` 号文档的 61/742 完成记录取代。

---

## 许可与归属

- 内置工作流改编自 [HKUSTDial/Supervisor-Skills](https://github.com/HKUSTDial/Supervisor-Skills)，采用 **CC BY-NC-SA 4.0**，方法论署名为 Yuyu Luo 及贡献者，完整许可见 `references/workflows/SUPERVISOR-LICENSE.txt`。
- IEEE 图表流程改编自用户提供的适配包，来源与改动记录见 `references/workflows/ieee-integration-provenance.json`。
- 内置字体为 Liberation Sans，SIL Open Font License 1.1。
- **论文原文的版权归原作者与出版方所有**，本仓库所含提取文本仅用于写作研究，不构成对原文的再分发授权，也不代表原作者或导师认可本项目。

因包含 CC BY-NC-SA 4.0 材料，本仓库整体按相同许可分享，**不得用于商业用途**。

---

## 免责声明

本技能通过检索与规则约束工作，不是模型微调，不代表崔爱娇本人意见，不验证论文技术结论的正确性，也不替使用者补充研究证据。
