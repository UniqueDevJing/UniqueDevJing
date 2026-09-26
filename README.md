<h3 align="center">胡景晟 · Jing</h3>

<p align="center">AI 应用开发 / Agent 开发 &nbsp;·&nbsp; 2027 届 &nbsp;·&nbsp; 河南理工大学 计算机科学与技术</p>

<p align="center"><sub>把「AI 能跑」做成「AI 能用」</sub></p>

---

我关心的是模型之外的那些事：输出能不能真的用、多轮之后贵不贵、出错的时候降不降得住。
所以下面这些项目里，测试、降级链和成本台账占的篇幅，比「接了个大模型」多得多。

### 主力项目

**[CodeCanvas](http://114.215.186.113/canvas/)** — 一句话生成可运行的 Web 应用

五阶段状态机编排（需求澄清 → 任务规划 → 代码生成 → 质量校验 → 自检修复）。生成物必须先过确定性静态校验才有资格交付，页面运行时报错由探针捕获后自动重做。

`15 次实测零误报` 　`第 8 轮上下文仅占全量 15%` 　`同等 token 量成本降 75%`

<br>

**[基于 RAG 的可信问答系统](http://114.215.186.113/mira/)** — 可信护栏 · [源码](https://github.com/UniqueDevJing/Mira)

回答里每个数字都要能在检索原文里找到依据，对不上就拒答并附原文。校验层是纯规则实现（AST 白名单求值、禁用 eval），不依赖模型自查。

`幻觉拦截率 100%` 　`正确回答误拒率 0%` 　`按 MCP 对外输出`

<br>

**[triagent](http://114.215.186.113/triagent/)** — 医疗分诊多 Agent 系统 · [源码](https://github.com/UniqueDevJing/triagent)

急症（红旗）症状由状态机强制短路，不经过模型；分诊与预约 Agent 共享结论，「该去急诊却挂了普通号」会被确定性拦住。

`0 次模型调用` 　`6–24ms 返回` 　`危险方向误判 0 例`

### 小工具

| 仓库 | 做什么 |
| --- | --- |
| [promptslim](https://github.com/UniqueDevJing/promptslim) | 调用前压缩 Prompt，砍冗余但保住代码块与语义 · 省 5–40% Token |
| [ai-cost-sentinel](https://github.com/UniqueDevJing/ai-cost-sentinel) | 改一行 `base_url` 接入的 LLM 成本追踪代理 |
| [agent-orchestrator](https://github.com/UniqueDevJing/agent-orchestrator) | Python 推理核心 + Java 管理面板，跨语言 Agent 编排 |
| [job-apply-assistant](https://github.com/UniqueDevJing/job-apply-assistant) | 求职流程管理桌面应用 |

---

**技术栈**　Java · Python · Spring Boot · Spring AI / LangChain4j · FastAPI · MySQL · Redis · SSE · MCP

**联系**　[UniqueDevJing@foxmail.com](mailto:UniqueDevJing@foxmail.com) ｜ [个人主页](https://uniquedevjing.github.io/portfolio/)
