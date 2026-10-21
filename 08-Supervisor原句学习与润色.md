# 用 paper-polish 学原句：保留、改写与暂缓

日期：2026-10-20。实际采用 paper-polish 的步骤：理解句子任务→检查表达问题与证据强度→决定保留/最小改写/暂缓→解释改动并核对含义。

61 份材料均有记录；C46 因残余 OCR 不做原句练习。其余记录中的原句来自分页抽取，已合并断行，未逐一视觉核验排版。因此不把文本层错误认定为作者原稿错误；学生与合著措辞也不归为导师独有。

改写是独立学习练习，不写回原论文，不声称是导师原句。所有数值、引文编号、信号与限定必须与原文一致；科学含义不确定时保留或暂缓，不用更流畅的句子掩盖不确定性。

## J01 · PDF p8 · 最小语言改写

来源：A Guaranteed Secure Scan Design based on Test Data Obfuscation by Cryptographic Hash.pdf；归因：first-author-paper。

分页抽取句：

> We can see that the test time is really reduced by (N - Td) test clock cycles (i.e., 3,348 clock cycles in the example design), although it is trivial to the overall test time.

独立语言练习：

The test time is reduced by (N - Td) test clock cycles (i.e., 3,348 clock cycles in the example design), although this reduction is small relative to the overall test time.

学习与改动说明：删除 We can see 和 really；将 it 的指代明确为 reduction。保留绝对节省量及其占比很小的让步。没有把小幅收益夸大。

## J02 · PDF p7 · 保留

来源：A New PUF Based Lock and Key Solution for Secure In-field Testing of Cryptographic Chips.pdf；归因：first-author-paper。

分页抽取句：

> During production test, the manufacturer only needs to keep SI = ‘0’ before TC is pulled low to commence the scan test as usual.

学习与改动说明：保留。During production test 定位阶段，only needs to 给最少动作，before 给时序；SI、TC 及取值不可为了流畅省略。

## J03 · PDF p10 · 保留

来源：A refined affine approximation method of multiplication for range analysis in word-length optimization.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> However, the polygon is larger than the true domain, and all the same noise symbols of different variables are not taken into account together.

学习与改动说明：保留为缺口句。However 后同时给几何范围偏大和相关噪声未联合处理两点；这里不将 noise symbols 换成含义未核实的新术语。

## J04 · PDF p11 · 最小语言改写

来源：A Robust FSM Watermarking Scheme for IP Protection of Sequential Circuit Design.pdf；归因：first-author-paper。

分页抽取句：

> It is evident that most designs watermarked by our method have lower area, timing, and power overheads.

独立语言练习：

Most designs watermarked by our method have lower area, timing, and power overheads.

学习与改动说明：移去 It is evident that，保留 most 及全部指标。比较对象承接前文，不额外写成所有设计、所有指标均优。

## J05 · PDF p12 · 最小语言改写

来源：Acceleration of the Bootstrapping in TFHE by FPGA.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> The data of other schemes using a similar parameter set are included for a fair comparison with the proposed scheme.

独立语言练习：

Data from other schemes using a similar parameter set are included for a fair comparison with the proposed scheme.

学习与改动说明：data of 改为 data from，信息来源更直接；similar 必须保留，不能润色成 identical。

## J06 · PDF p10 · 保留

来源：Design of Optimal Scan Tree Based on Compact Test Patterns for Test Time Reduction.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> On average, our scan trees save 56.7 percent (55.4 percent with AAC only) of test time over the baseline designs as opposed to the average saving of 30.1 percent by [24].

学习与改动说明：保留。两个平均值分别对应本文和文献基线，括号另报 AAC-only。数字属于原文，不迁移为用户新实验结果；over baseline 的分母不能省。

## J07 · PDF p10 · 保留

来源：FREGAT：An FSM Reverse Engineering Method using Graph Attention Network on Scan-Dump Data.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> For the remaining three designs ‘ae18’, ‘mem_ctrl’, and ‘gcm-aes’, only one target state register is missed.

学习与改动说明：保留 only、目标对象及三项设计名；仅据此单句不改写为三个设计合计漏一个，或每个设计均漏一个，需结合上下文确认。

## J08 · PDF p11 · 最小语言改写

来源：Identification of FSM State Registers by Analytics of Scan-Dump Data.pdf；归因：first-author-paper。

分页抽取句：

> It should be noted that some designs may appear to have many more state registers than they are required by the functional states of an FSM.

独立语言练习：

Some designs may appear to have many more state registers than are required by the functional states of an FSM.

学习与改动说明：去掉提醒套语并修正 than they are required 的句法；may appear 保留，避免把表观数量写成必然事实。functional states 的术语保留。

## J09 · PDF p5 · 保留

来源：IP Watermarking Using Incremental Technology Mapping at Logic Synthesis Level.pdf；归因：first-author-paper。

分页抽取句：

> However, as τ increases, the number of qualiﬁed disjoint closed cones is reduced, and Pc and Pr become higher.

学习与改动说明：保留。as 引导参数变化，同时报告可用闭锥减少和两个概率量增大，形成代价链。符号的定义由原文提供，本练习不重释公式。

## J10 · PDF p11 · 最小语言改写

来源：LEXGART：Leveraging XGBoost and Register Topology for Reverse Engineering FSM from Scan-Dump Data.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> After applying the incremental procedure, CDR reached 100% for all three designs, confirming the utility of the proximity-based refinement in mitigating limitations due to insufficient state excitation during functional analysis.

独立语言练习：

After the incremental procedure was applied, CDR reached 100% for all three designs, confirming the utility of the proximity-based refinement in mitigating limitations due to insufficient state excitation during functional analysis.

学习与改动说明：改为被动时间从句，避免 CDR 成为 applying 的逻辑施事。保留 all three designs、100% 及原句的解释；其 HR 代价必须在相邻讨论中一起读。

## J11 · PDF p13 · 最小语言改写

来源：Non-Invasive Reverse Engineering of One-Hot Finite State Machines Using Scan Dump Data.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> It can be seen that the preprocessing for identiﬁcation of data registers costs most time, however, the preprocessing does help to reduce the complexity of consequent operations.

独立语言练习：

Preprocessing for identification of data registers takes the most time. However, it helps reduce the complexity of subsequent operations.

学习与改动说明：修正逗号拼接、costs most time 和 consequent operations 的搭配。两句保留最耗时但帮助后续的关系，不将预处理直接说成降低总时间。

## J12 · PDF p10 · 保留

来源：Printed Electronics Based Optical Unclonable Label for Artificial Intelligence Authentication.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> Although Han et al. [38] extend the number of classes to 60 and achieve an accuracy of 0.996, its fabrication cost remains high.

学习与改动说明：保留让步与具体比较条件。精度高不自动意味着成本低；不把这句重新写成对比方法全面失败。数字仅为原文对该文献的报告。

## J13 · PDF p12 · 保留

来源：SATAM：A SAT Attack Resistant Active Metering Against IC Overbuilding.pdf；归因：first-author-paper。

分页抽取句：

> After a chip is protected by the proposed metering method and fabricated, if a correct key is input, the design structure is equivalent to the original design and the test vectors can be applied transparently without compromising the fault coverage or testability achievable by the original test set.

学习与改动说明：保留条件链作为学习对象：保护与制造完成→正确密钥→结构等价→原测试集可用。without compromising 的对象必须随句保留，不只留下 testability 一词。

## J14 · PDF p11 · 保留

来源：Static and Dynamic Obfuscations of Scan Data Against Scan-Based Side-Channel Attacks.pdf；归因：first-author-paper。

分页抽取句：

> The secure scan design can be tested with the original test patterns without sacriﬁcing its testability.

学习与改动说明：保留。can be tested 描述能力，with 指出原测试模式，without sacrificing 限定保持性。结合 p11 邻句，不能扩大为新增保护电路的所有故障也可测。

## J15 · PDF p10 · 最小语言改写

来源：Synthesis-for-Testability Watermarking for Field Authentication of VLSI Intellectual Property.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> It is possible that Bob may add some minor circuitry around Alice’s watermarked IP to map the input/output signals in front of the test chain or block access to part of her IP core to prevent her watermark to be detectable in the ﬁeld.

独立语言练习：

It is possible that Bob may add some minor circuitry around Alice’s watermarked IP to map the input/output signals in front of the test chain or block access to part of her IP core to prevent her watermark from being detected in the field.

学习与改动说明：仅将 prevent ... to be detectable 修为 prevent ... from being detected；保留 may 的假设，不把潜在攻击写成实际发生。仍较长，可在读懂 map 的技术对象后另做结构改写。

## J16 · PDF p12 · 最小语言改写

来源：Ultra-Low Overhead Dynamic Watermarking on Scan Design for Hard IP Protection.pdf；归因：first-author-paper。

分页抽取句：

> The ‘Torg’ column shows the numbers of total transitions during testing for the originally optimized scan design.

独立语言练习：

The ‘Torg’ column shows the total number of transitions during testing for the originally optimized scan design.

学习与改动说明：numbers of total transitions 改为 total number of transitions。保持基线 exactly 为 originally optimized design；不将它缩写成任意原电路。

## J17 · PDF p9 · 最小语言改写

来源：Why current secure scan designs fail and how to fix them.pdf；归因：first-author-paper。

分页抽取句：

> After the insertion of the proposed secure design, the area of the complete design equals to 212432 NAND gates.

独立语言练习：

After insertion of the proposed secure design, the total design area is equivalent to 212432 NAND gates.

学习与改动说明：面积门数口径用 is equivalent to 表达，保留 212432 及保护后总面积。仅此句还不能证明开销很低，必须连读原基线与差值。

## J18 · PDF p12 · 保留

来源：YAXY：A New Hybrid FPGA-Based Hardware Acceleration of TFHE.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> However, the resource consumption of this external host processor is not reflected in its FPGA resource usage or area-efficiency metrics.

学习与改动说明：保留。However 指出比较边界，external host processor 与 not reflected 解释资源核算缺口；未把吞吐落后说成优于基线。

## C02 · PDF p4 · 保留

来源：A hybrid watermarking scheme for sequential functions.pdf；归因：first-author-paper。

分页抽取句：

> Without changing Alice’s design, Bob may select some bits in the output sequence to form his own watermark.

学习与改动说明：保留。Without changing 与 may 规定了攻击动作的限制和假设性。后文须再解释为何观察到匹配位不等于能证明自己的权属。

## C05 · PDF p3 · 保留

来源：A low-overhead dynamic watermarking scheme on scan design for easy authentication.pdf；归因：first-author-paper。

分页抽取句：

> Bob may want to find his own watermark from Alice’s design without touching her design.

学习与改动说明：保留。先描述攻击者目标，再约束不能修改设计；语言简单也能准确建立后续分析情境。

## C08 · PDF p2 · 最小语言改写

来源：A memristor-based scan hold flip-flop.pdf；归因：first-author-paper。

分页抽取句：

> The signals Clk, D, SD, TC and Q denoted the clock, normal input data, scan data, test control signal, and the output of SFF, respectively.

独立语言练习：

The signals Clk, D, SD, TC, and Q denote the clock, normal input data, scan data, test control signal, and SFF output, respectively.

学习与改动说明：图示说明用 denote 并统一列表；respectively 保留，确保五个符号与五个含义一一对应。未改变任何信号定义。

## C10 · PDF p4 · 最小语言改写

来源：A new active IC metering technique based on locking scan cells.pdf；归因：first-author-paper。

分页抽取句：

> Bob may conceive to predict the PUF key directly without intruding Alice’s design.

独立语言练习：

Bob may consider predicting the PUF key directly without intruding into Alice’s design.

学习与改动说明：修正 conceive to 和 intruding 的搭配，保留 may consider 的假设层级，不写成 Bob 已经发起攻击。

## C15 · PDF p3 · 最小语言改写

来源：A new scheme to extract PUF information by scan chain.pdf；归因：first-author-paper。

分页抽取句：

> To overcome the overbuilding problem, metering scheme has been proposed to enable the design house to achieve the post-fabrication control over their ICs.

独立语言练习：

To overcome the overbuilding problem, a metering scheme has been proposed to enable the design house to achieve post-fabrication control over its ICs.

学习与改动说明：补冠词并把 their 的指代统一为单数 design house 的 its。保持被引入的是计量方案，不暗示所有芯片已受控制。

## C18 · PDF p3 · 保留

来源：A post-processing scan-chain watermarking scheme for VLSI intellectual property protection.pdf；归因：first-author-paper。

分页抽取句：

> The authorship proof is stronger if the length of the watermark is longer.

学习与改动说明：保留条件比较的结构。只从此句学习 if 与比较级的关系；水印长度如何影响证明强度须读相邻概率定义，不能由语言练习另造公式。

## C20 · PDF p4 · 最小语言改写

来源：A scan design method based on two complementary connection styles to minimize test power.pdf；归因：first-author-paper。

分页抽取句：

> For comparison, we also repeat the methods in [4], [8] and [12] on each design with the same EDA tools.

独立语言练习：

For comparison, we also apply the methods in [4], [8], and [12] to each design using the same EDA tools.

学习与改动说明：repeat the methods 改为 apply the methods，保留 each design 与 same EDA tools。未宣称与原论文环境逐项完全相同。

## C21 · PDF p5 · 最小语言改写

来源：A secure and low-overhead active IC metering scheme.pdf；归因：first-author-paper。

分页抽取句：

> We analyze some typical possible attacks against the proposed metering method to evaluate its security.

独立语言练习：

We analyze typical attacks against the proposed metering method to evaluate its security.

学习与改动说明：删除 some 和 possible 的重复修饰，典型攻击集合并未变成所有攻击；不外推出安全定理。

## C23 · PDF p3 · 最小语言改写

来源：An improved publicly detectable watermarking scheme based on scan chain ordering.pdf；归因：first-author-paper。

分页抽取句：

> When τ decreases, Pλ increases and a threshold for τ can be determined empirically that with high degree of confidence, Y’ will not appear in the output responses for a given number of input vectors tested.

独立语言练习：

When τ decreases, Pλ increases, and a threshold for τ can be determined empirically such that, with a high degree of confidence, Y’ will not appear in the output responses for a given number of tested input vectors.

学习与改动说明：修正 that 引导方式、缺失冠词及 tested 的位置。保留经验阈值、置信限定和测试向量数量条件；未重新计算概率。

## C25 · PDF p2 · 最小语言改写

来源：An improved scan design for minimization of test power under routing constraint.pdf；归因：first-author-paper。

分页抽取句：

> Generally speaking, a big K means more small clusters and more scan cells which are close to each other can be connected.

独立语言练习：

In general, a larger K produces more small clusters, allowing more scan cells that are close to each other to be connected.

学习与改动说明：big 改为 larger，整理两个 more 的依附。后句中小簇可能损害全局功耗最优的代价不可省略。

## C33 · PDF p5 · 最小语言改写

来源：How to retrieve PUF response from a fabricated chip securely.pdf；归因：first-author-paper。

分页抽取句：

> We evaluate the existing PUF retrieval schemes with regards to the area overhead, security.

独立语言练习：

We evaluate existing PUF retrieval schemes in terms of area overhead and security.

学习与改动说明：with regards to 改为 in terms of，并列两个评价轴。没有把 area 与 security 合成单个优劣分数。

## C37 · PDF p3 · 最小语言改写

来源：Intellectual property authentication by watermarking scan chain in design-for-testability flow.pdf；归因：first-author-paper。

分页抽取句：

> In this section, we illustrate the basic percept of a nonintrusive watermarking scheme that can be seamlessly blent into any existing Design for Testability (DfT) flow.

独立语言练习：

In this section, we illustrate the basic percept of a nonintrusive watermarking scheme that can be seamlessly blended into any existing Design for Testability (DfT) flow.

学习与改动说明：只改 blent→blended。percept 可能意指 concept 或 precept，但未仅凭词形擅自替换；应结合原段确认。any 属原文能力范围，不成为新稿自动可用的断言。

## C38 · PDF p2 · 保留

来源：Kernel extraction for watermarking combinational logic networks.pdf；归因：first-author-paper。

分页抽取句：

> The remapping of C8-C16 shows no timing constraint violation and incurs the least overhead to the design.

学习与改动说明：保留具体候选与全局约束的比较。least 的范围是本例候选，不扩展为对所有网表和候选的全局最优证明。

## C46 · PDF p4 · 暂缓

来源：Stego-signature at logic synthesis level for digital design IP protection.pdf；归因：first-author-paper。

学习与改动说明：残余 OCR 尚未全量视觉校对，仅按已核验首页做结构学习。本条不把机器残缺句润色成导师用词样本。

## C48 · PDF p3 · 保留

来源：Watermarking for IP protection through template substitution at logic synthesis level.pdf；归因：first-author-paper。

分页抽取句：

> In the distributed copy, we search for the nodes whose logic functions are equivalent to those of the input and output nodes connected to each seed cell.

学习与改动说明：保留原件/分发副本、逻辑等价和连接到 seed 的范围。为了简短删除这些限定会改变水印提取步骤。

## D01 · PDF p25 · 暂缓

来源：11级_保护大规模集成电路知识产权的动态水印技术研究_刘永霞.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, we mainly review dynamic watermarking research at different design and different design methods of test response space compactor.

学习与改动说明：可以学习章末回顾的动作；different design 后缺明确名词，未擅自补成 levels、stages 或 methods。学生原稿及抽取错误不进入导师个人用词结论。

## D02 · PDF p32 · 保留

来源：11级_旨在降低测试时间和测试功耗的扫描树设计研究_陈林枫.caj；归因：supervised-student-thesis。

分页抽取句：

> Generating power-aware test patterns during ATPG might result in a less compact test pattern set, leading to longer test time and larger test data volume.

学习与改动说明：保留 might 与从测试集不紧凑到时间/数据量增加的链。这里写的是潜在代价，不能替换为必然导致。

## D03 · PDF p27 · 最小语言改写

来源：12级_基于扫描的耗时少低功耗的可测试性技术研究_于婷婷.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, the research status of scan design for optimization of test power, test time and test data volume is reviewed.

独立语言练习：

This chapter reviews scan-design research on optimizing test power, test time, and test data volume.

学习与改动说明：将长被动名词化改为直接主谓结构，三条研究线及优化对象保留。仅是学生章末摘要的语言练习。

## D04 · PDF p31 · 最小语言改写

来源：13级_抗扫描旁路攻击的安全扫描链设计研究_骆彦辉.caj；归因：supervised-student-thesis。

分页抽取句：

> Some of them were proposed to obfuscate the scan data from scan chain to resist scan-based attacks.

独立语言练习：

Some of them were proposed to obfuscate scan data from the scan chain to resist scan-based attacks.

学习与改动说明：补 the scan chain 并去掉无必要的 the scan data；some 与攻击类型保持。需要上文确定 them 的指代后才可单独复用。

## D05 · PDF p25 · 最小语言改写

来源：13级_满足面积约束的低功耗扫描设计技术研究_何禄成.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, the research status of scan design for test power optimization is reviewed.

独立语言练习：

This chapter reviews scan-design research on test-power optimization.

学习与改动说明：以 this chapter 作主语，消除 research status ... is reviewed 的绕行；不补写该章未给出的具体结论。

## D06 · PDF p23 · 最小语言改写

来源：14级_基于可测试性设计结构的IP水印技术研究_黄晓男.caj；归因：supervised-student-thesis。

分页抽取句：

> Among the constraint-based watermarking schemes, the dynamic watermarking techniques as FSM-based watermarking and DFT watermarking are mainly reviewed as they can enable the watermark to be detected in field.

独立语言练习：

Among constraint-based watermarking schemes, this chapter mainly reviews dynamic watermarking techniques such as FSM-based and DFT watermarking because they allow the watermark to be detected in the field.

学习与改动说明：修正 techniques as、冠词和 in field；保留分类、重点选择与可现场检测的因果。不是把导师所有论文都改成此句式。

## D07 · PDF p22 · 最小语言改写

来源：14级_基于密码散列函数的安全可测试性设计技术研究_李孟扬.caj；归因：supervised-student-thesis。

分页抽取句：

> The mode-reset countermeasure cannot resist such attack and is hence vulnerable.

独立语言练习：

The mode-reset countermeasure cannot resist such an attack and is hence vulnerable.

学习与改动说明：补 an；such 必须回指刚分析的攻击，不能删去并写成抗不了任何攻击。

## D08 · PDF p25 · 最小语言改写

来源：14级_基于延迟的PUF设计及其应用研究_王佳东.caj；归因：supervised-student-thesis。

分页抽取句：

> Recent years, many PUF schemes have been proposed and it can be classified as delay-based PUF and memory-based PUF.

独立语言练习：

In recent years, many PUF schemes have been proposed, and they can be classified as delay-based or memory-based PUFs.

学习与改动说明：补 In，修正 it 的数和分类项；仅复述本段的实现分类轴，不与 strong/weak 轴混合。

## D09 · PDF p33 · 最小语言改写

来源：15级_基于并行扫描链的延迟型PUF设计及其应用研究_王文煊.caj；归因：supervised-student-thesis。

分页抽取句：

> According to the number of CRPs, the PUFs can be divided into strong PUF weak PUF.

独立语言练习：

According to the number of CRPs, PUFs can be divided into strong and weak PUFs.

学习与改动说明：修正缺少连词和数的一致；这是抽取句练习，未逐一视觉核对，不能认定连词缺失一定出自作者原排版。

## D10 · PDF p30 · 保留

来源：15级_旨在防伪造的主动式IC计量技术研究_钱学森.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, most existing IC metering methods are reviewed and evaluated.

学习与改动说明：保留章末回顾功能。most 已限定覆盖范围；该句本身没有说明评价结论，不能把它当作综述已充分综合的证明。

## D11 · PDF p31 · 最小语言改写

来源：16级_基于pay-per-use...PGA知识产权保护技术研究_孙佩琦.caj；归因：supervised-student-thesis。

分页抽取句：

> We in this chapter introduce some related work about the earlier proposed FPGA IP protection mechanisms, such as signature-based scheme, encryption-based scheme, pay-per-use licensing scheme and PUF-based scheme, and then evaluate their advantages and disadvantages respectively.

独立语言练习：

In this chapter, we introduce related work on previously proposed FPGA IP protection mechanisms, including signature-based, encryption-based, pay-per-use licensing, and PUF-based schemes, and evaluate their respective advantages and disadvantages.

学习与改动说明：整理副词、on 的搭配与复数列表，保留四类保护机制。这里学习章组织，不推断后续付费实现结果。

## D12 · PDF p29 · 最小语言改写

来源：16级_基于忆阻器的D触发器设计及其在扫描链设计中的应用研究_常振兴.caj；归因：supervised-student-thesis。

分页抽取句：

> As a non-volatile device, memristor has been widely explored to implement non-volatile sequential devices so that the important data stored in memory is immune to the unexpected power failure in the system.

独立语言练习：

As a non-volatile device, the memristor has been widely explored for implementing non-volatile sequential devices so that important data stored in memory are immune to unexpected system power failure.

学习与改动说明：修正冠词、data 的数及搭配。immune 属原句较强主张，只保留作源句练习，未据此推荐新稿使用无条件不丢数据断言。

## D13 · PDF p27 · 最小语言改写

来源：16级_基于扫描链的PUF信息提取技术及其应用研究_周炜.caj；归因：supervised-student-thesis。

分页抽取句：

> Some work also proposed to insert some inverters [47] or XOR gates [48] at some random positions in scan chain to obfuscate scan output.

独立语言练习：

Some studies also proposed inserting inverters [47] or XOR gates [48] at random positions in the scan chain to obfuscate the scan output.

学习与改动说明：some work→some studies，proposed to insert→proposed inserting，并修正冠词。保留方案来源编号和插入位置条件。

## D14 · PDF p32 · 保留

来源：16级_防IC过量生产的主动式计量技术研究_杨燕.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, most of the existing IC metering methods are reviewed and evaluated.

学习与改动说明：保留。与 D10 相近的句法说明此为共享章末导航结构；相似不证明导师本人逐句执笔。

## D15 · PDF p29 · 最小语言改写

来源：17级_PUF信息的安全提取及其在IC计量技术中的应用研究_王宇溪.caj；归因：supervised-student-thesis。

分页抽取句：

> The work in [25] proposed a protection scheme whose protocol can be applicable to a broad category of bus-based IC.

独立语言练习：

The work in [25] proposed a protection scheme whose protocol can be applied to a broad category of bus-based ICs.

学习与改动说明：can be applicable→can be applied，IC 用复数。broad category 保留，不能自动改为 all bus-based ICs。

## D16 · PDF p25 · 保留

来源：17级_基于大数据分析的有限状态机结构反演技术研究_何诚慷.caj；归因：supervised-student-thesis。

分页抽取句：

> The registers with high Impact and Relevancy will finally be identified as the FSM state registers.

学习与改动说明：保留特征筛选的收束句。Impact、Relevancy 是该文定义的特征名，不能在语言层换成普通同义词；是否足够识别是方法论问题。

## D17 · PDF p31 · 最小语言改写

来源：17级_基于扫描链设计的老化芯片检测技术研究_徐志超.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, existing methods to detect recycled IC are reviewed and evaluated.

独立语言练习：

This chapter reviews and evaluates existing methods for detecting recycled ICs.

学习与改动说明：将被动式改成章节作主语的直接表述，修正复数；未补写温度、成本等此句未出现的评价结果。

## D18 · PDF p31 · 保留

来源：17级_防故障注入攻击的FSM状态寄存器安全设计研究_王子铭.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, the FIA methods based on underfeeding, overheating and overclocking in FSM are first reviewed and analyzed.

学习与改动说明：不在语言练习中将 underfeeding 自动改为某种物理攻击名称，需读原段确定含义；学习攻击类型先分类再分析的结构。

## D19 · PDF p30 · 暂缓

来源：18级_基于扫描旁路攻击的LFSR和计数器结构反演技术研究_王启东.caj；归因：supervised-student-thesis。

分页抽取句：

> In this chapter, some basic percept and related research are introduced.

学习与改动说明：percept 的技术意图未由单句确定，不将其静默替换为 concept。可记录章节入口功能，暂不抽成推荐原句。

## D20 · PDF p31 · 最小语言改写

来源：18级_基于柔性电子的PUF设计及其应用研究_翟明皓.caj；归因：supervised-student-thesis。

分页抽取句：

> The work in [1] used PUF and finite state machine (FSM) model to propose a secure and lightweight authentication scheme.

独立语言练习：

The work in [1] proposed a secure and lightweight authentication scheme based on a PUF and a finite state machine (FSM) model.

学习与改动说明：将 used ... to propose 改成 proposed ... based on，保留两项构件和原文对其性能的描述；这些形容词仍只是该章对文献的报告。

## D21 · PDF p31 · 最小语言改写

来源：18级_安全可靠的主动式IC计量技术研究_张慧.caj；归因：supervised-student-thesis。

分页抽取句：

> According to different implementation mechanisms, IC metering technology can be divided into passive and active IC metering technology.

独立语言练习：

According to the implementation mechanism, IC metering can be classified as passive or active.

学习与改动说明：压缩重复 technology 和类别名，保持分类轴。不能从 passive/active 分类本身推导其中一类在所有场景都更好。

## D22 · PDF p34 · 保留

来源：19级_基于PUF的PCB认证技术研究_张玥熙.pdf；归因：supervised-student-thesis。

分页抽取句：

> Based on the above analysis, it is necessary to find a board-level PUF implementation method to complete the PCB authentication, which can solve the above problems.

学习与改动说明：可分析 Based on the above analysis 的承接，但 this/above problems 需上文才能具体化；不擅补 PCB 方案的性能或替它证明可以解决全部问题。

## D23 · PDF p32 · 最小语言改写

来源：19级_基于光学PUF的印刷电子认证技术研究_翁镇.pdf；归因：supervised-student-thesis。

分页抽取句：

> This technology based on additive manufacturing process can manufacture electronic devices on a large scale at low cost.

独立语言练习：

This additive-manufacturing technology can produce electronic devices on a large scale at low cost.

学习与改动说明：压缩 technology based on ... process 的名词堆叠；can、large scale 和 low cost 保留为源段描述，不加新的制造量或成本数字。

## D24 · PDF p35 · 保留

来源：19级_基于忆阻器的安全扫描链设计研究_陆孟强.pdf；归因：supervised-student-thesis。

分页抽取句：

> Many countermeasures have been proposed to resist the scan-based side-channel attacks.

学习与改动说明：保留作为综述入口。Many countermeasures 并非充分的具体缺口，后续必须连读哪些机制为何仍不满足要求。

## D25 · PDF p27 · 保留

来源：19级_基于扫描数据分析的FSM状态寄存器识别技术研究_卢昊.pdf；归因：supervised-student-thesis。

分页抽取句：

> This chapter first introduces the scan-based side-channel attack.

学习与改动说明：保留章节导航句。introduces 不等于提出一种新的扫描攻击；不能为显得创新把它改成 proposes。

## D26 · PDF p32 · 最小语言改写

来源：19级_基于无芯RFID的PUF设计研究_李迅.pdf；归因：supervised-student-thesis。

分页抽取句：

> This chapter first introduces the development of chipless RFID tag and PUF.

独立语言练习：

This chapter first introduces the development of chipless RFID tags and PUFs.

学习与改动说明：统一类别的复数；没有把 chipless、TDR 等分类关系追加到此句，详细分类应来自相邻原文。

## D27 · PDF p30 · 最小语言改写

来源：20级_基于印刷电子的轻量级物理不可克隆函数的设计研究_王剑鸣.pdf；归因：supervised-student-thesis。

分页抽取句：

> This chapter reviews several commonly used printing technologies, and introduces the corresponding research directions and research progresses.

独立语言练习：

This chapter reviews several commonly used printing technologies and introduces the corresponding research directions and research progress.

学习与改动说明：修正不可数 progress，并去掉并列谓语前不必要的逗号。原句的章节回顾任务不变。

## O01 · PDF p120 · 保留

来源：Digital Fingerprint A Practical Hardware Security Primitive.pdf；归因：coauthored-paper-or-chapter。

分页抽取句：

> A fingerprinted IP will not directly prevent misuse of the IP, but will allow the IP provider to detect the source of the redistributed IP and therefore trace the traitor.

学习与改动说明：保留。will not directly prevent 与 will allow 构成明确能力边界；后半句追溯来源不能被润色成已经阻止滥用。第四作者合著样本，不归为导师独有句法。

