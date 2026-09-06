# 方法来源与迁移边界

## 本轮实际核验的方法

以下为 2026-09-06 实际读取的范围。只采用能改变操作的机制与边界，来源的政策要求、产品默认值和案例结果不成为运营默认。专业方法的可用性仍需符合本次数据、设计和任务条件。

| 来源、版本 | 实际读取范围 | 采用与不采用 |
|---|---|---|
| GDS Service Manual：[Learning about users and their needs](https://www.gov.uk/service-manual/user-research/start-by-learning-user-needs)，2017-03-23 更新；[Measuring success](https://www.gov.uk/service-manual/measuring-success/measuring-the-success-of-your-service)，2018-08-06；[Measuring completion rate](https://www.gov.uk/service-manual/measuring-success/measuring-completion-rate)，2021-02-19 更新 | 需求研究、对象、记录与验证；交易、完整任务及政策目标的测量；完成率的起终点、保存返回、跨渠道和支持方式 | 以任务与障碍取证，分清提交和完整结果。机构强制指标、资格排除口径、公开发布要求不迁移；方法指南不证明特定改动有效。 |
| Amplitude：[Retention FAQ](https://amplitude.com/docs/analytics/charts/retention-analysis/faq) 与 [Usage interval](https://amplitude.com/docs/analytics/charts/retention-analysis/retention-analysis-interpret-usage)，访问版 | 两页正文，留存口径、未成熟队列和重复使用者的纳入条件 | 固定回返定义与成熟分母；重复者的间隔存在选择边界。不采用产品时间窗、界面或增长建议。 |
| NIST/SEMATECH：[Censoring](https://www.itl.nist.gov/div898/handbook/apr/section1/apr131.htm)，访问版 | §8.1.3.1 全节 | 区分已发生事件与观察截止；从设备可靠性有限迁移数据状态，未回返不直接编码为永久流失，亦不据本节宣称掌握生存分析。 |
| Little, “Little’s Law as Viewed on Its 50th Anniversary”, 2011，DOI 10.1287/opre.1110.0940，[原作者论文的大学托管 PDF](https://people.cs.umass.edu/~emery/classes/cmpsci691st/readings/OS/Littles-Law-50-Years-Later.pdf) | §1、§2.1–2.3，印刷页 536–540 | 时间平均数量与对象平均停留须同边界；有限空窗可精确核对，非空窗需处理边界。恒等式不单独支持干预预测或个体时效承诺。 |
| Gallien：[MIT Capacity Lecture](https://www.ocw.mit.edu/courses/15-760b-introduction-to-operations-management-spring-2004/16dde953a29f89a4d2018361900ce886_lec3_capacity.pdf)，课件 2002／课程 2004 | PDF 页 5–8、14–20 | 平均负荷之外检查到达、耗时与时段变异；不搬用课堂参数或近似排队公式作为默认。 |
| HM Treasury：[Green Book 2026](https://www.gov.uk/government/publications/the-green-book-appraisal-and-evaluation-in-central-government/the-green-book-2026)，2026-02-05 版 | Chapter 6 方法、沉没成本、方案选择和敏感性；Chapter 7 分配；Chapter 8 资源估值 | 下一步的未来差额、机会成本、非货币结果和改变选择的条件。只迁移比较机制，不引入英国政策、折现率或审批流程。 |
| Microsoft ExP：[Diagnosing Sample Ratio Mismatch](https://www.microsoft.com/en-us/research/articles/diagnosing-sample-ratio-mismatch-in-a-b-testing/)，2020-09-14 | SRM 影响、检测、根因与触发诊断正文；下表试验后文章的分母、触发与权衡部分亦重新读取 | 核对实际分配机制并定位受影响估计；分母也可能受干预影响。无异常不证明全部可信，企业阈值和工具不是通用要求。 |
| Hernán & Robins：[Causal Inference: What If](https://miguelhernan.org/whatifbook)，2026-08-19 PDF；引文年份 2020 | §22.1、Fine Points 22.2–22.3，印刷页 305–308；另核对 §3.6 相关定义 | 区分分配效果、实际接受效果及事后筛选；保留缺失的识别问题。仅迁移这些界限，不默认实施整套目标试验模拟或依从调整。 |
| HM Treasury：[Magenta Book Annex A](https://www.gov.uk/government/publications/the-magenta-book/magenta-book-annex-a-analytical-methods-for-use-within-an-evaluation-html)，2026 更新版 | A2.1 随机试验、A2.4 中断时间序列、A2.7 双重差分；A3.1、A3.3、A3.5 价值评价 | 无随机时选择合适设计并实际检查假设；成本效果与分配可分别评价。原则框架不是效果估计，既往平行趋势不证明反事实成立。 |

## 原有方法的来源沿革

以下链接与读取范围承接原运营方法的来源记录。原记录标注核验日期为 2026-09-06；拆分时读取的是已有方法及其来源记录，未逐页重新核验网站。除上表明确重新读取的内容外，不能将其记为本轮网页核验。链接不证明当前功能、访问权限或任何项目的效果；需要动态事实时重新核对。

| 来源 | 已有记录的实际读取范围 | 本技能采用与限制 |
|---|---|---|
| [The Secrets to AWS Product Management](https://aws.amazon.com/executive-insights/content/product-management-at-amazon/) | 网页四节；未下载电子书 | 从真实问题反推可交付价值，区分想法与证据。企业自述不是普遍效果证明，不要求固定提案体例。 |
| [智能分析最佳实践——指标逻辑树](https://tech.meituan.com/2017/12/04/logictree.html)，2017-12-04 | 正文方法与限制 | 拆分指标和维度定位变化。分解不自动建立因果，不依赖大型分析平台。 |
| [Quick Tracking 漏斗分析](https://help.aliyun.com/zh/document_detail/250880.html) | 概述、计算逻辑及实例 | 路径比较需固定主体、顺序、窗口与关联对象。不继承特定产品的数据访问与功能。 |
| [Patterns of Trustworthy Experimentation: During-Experiment Stage](https://www.microsoft.com/en-us/research/articles/patterns-of-trustworthy-experimentation-during-experiment-stage/)，2021-01-25 | 方法正文 | 目标、诊断、保护和数据质量指标；异常分配、反复窥视及新奇效应。使用统计判断仍须满足相应设计条件。 |
| [Patterns of Trustworthy Experimentation: Post-Experiment Stage](https://www.microsoft.com/en-us/research/articles/patterns-of-trustworthy-experimentation-post-experiment-stage/)，2021-12-24 | 方法正文 | 核对实现、口径、分母及权衡，再解释结果；不推称拥有来源企业的实验能力。 |
| [Upload schedule tips](https://support.google.com/youtube/answer/13616979) | 正文 | 供给节奏要与容量、成本和工作性质相容。平台发布频率、时段、时长等不是通用要求。 |
| [Characterizing and Minimizing Divergent Delivery in Meta Advertising Experiments](https://arxiv.org/html/2508.21251v1)，2025-08-28 | 预印本摘要、披露及方法/分析 | 广告方案间比较与有无广告的增量比较回答不同问题；存在研究者雇佣/持股披露，不保证其他环境具备同一工具或结果。 |
| [Google Ads 对 ROAS 与增量回报的说明](https://support.google.com/google-ads/answer/14102450?hl=en) | 原收益方法引用该官方说明，未单独记录读取层级 | 作为归因与增量、转化价值与投入的术语出处；不作为本次独立核验的证据或特定数值目标。 |
| [Shopify 对获客成本的说明](https://www.shopify.com/blog/customer-acquisition-cost) | 原收益方法引用该说明，未单独记录读取层级 | 用于费用与新客口径追溯；其目标比例与经营建议不成为默认标准。 |

这些公开说明、研究和产品文档为专业判断提供有限依据，不是统一运营规范。候选方法还需在不同用途的任务中检验；无论结果好坏，个别项目的定位、数字、风格、经营边界和授权都不能沿来源说明进入底层能力。
