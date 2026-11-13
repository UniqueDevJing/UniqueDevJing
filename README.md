<div align="center">

# 胡景晟｜AI 应用开发工程师

把模型能力做成可验证、可维护、能上线的业务系统。

</div>

我关注的不是把接口接通，而是把角色、状态、权限、异常和数据流一起设计清楚：模型负责理解与生成，业务结果由后端规则、事务和人工确认控制。

## 主力项目

| 项目 | 一句话说明 | 重点能力 |
| --- | --- | --- |
| [CareNexus](https://github.com/UniqueDevJing/CareNexus/) | 基于 LangChain4j + Spring Boot 的智能分诊就医系统 | 预问诊、风险拦截、预约并发控制、医生接诊、病历与运营观测 |
| [MinutesTrace](https://github.com/UniqueDevJing/minutestrace/) | 基于 FastAPI + LangGraph 的智能会议助手 | 资料导入、异步转写、证据链纪要、Agent 自检、人工审批与行动项 |

## 在线体验（仅演示）

演示环境使用独立的公开账号，不包含真实患者、医生或会议资料；生产环境账号和密钥不会写进仓库。

- [CareNexus 在线体验](http://114.215.186.113/CareNexus/)：`patient / 123456`、`doctor / 123456`、`admin / 123456`
- [MinutesTrace 在线体验](http://114.215.186.113/minutestrace/)：`demo / demo123456`、`admin / demo123456`

## 我的工程方法

- 先定义角色、状态和数据归属，再接入模型和工具。
- 把高风险写入放在服务端：权限、预约、病历、审批和版本发布都由确定性逻辑控制。
- 为结论保留来源：医疗项目追踪就诊链路，会议项目追踪转写片段和证据位置。
- 对异常路径负责：超时、重试、幂等、并发竞争、断线恢复和失败后回滚都纳入测试。
- 用接口测试、浏览器流程和生产构建验证“能运行”与“可交付”之间的差距。

## 技术方向

- **Agent 与模型应用**：Python、FastAPI、LangGraph、LangChain4j、提示词版本、工具调用、SSE、异步 Worker
- **后端工程**：Spring Boot、Spring Security、SQLAlchemy、JDBC、事务、权限与状态机
- **前端工程**：Vue 3、TypeScript、Vite、Vue Router、Element Plus、GSAP、响应式工作台
- **数据与交付**：MySQL、SQLite、H2、Nginx、Docker Compose、systemd、Linux 部署

## 其他项目

- [Mira](https://github.com/UniqueDevJing/Mira/)：文档检索与可溯源问答系统。
- [Triagent](https://github.com/UniqueDevJing/triagent/)：多角色任务协作与工具编排框架。
- [CodeCanvas](https://github.com/UniqueDevJing/CodeCanvas/)：从需求到可运行页面的开发验证工作台。

## 联系与交流

欢迎交流智能应用落地、Agent 工作流、检索系统、业务状态设计和全栈交付。

<div align="center">

[CareNexus](https://github.com/UniqueDevJing/CareNexus/) · [MinutesTrace](https://github.com/UniqueDevJing/minutestrace/) · [Mira](https://github.com/UniqueDevJing/Mira/) · [Triagent](https://github.com/UniqueDevJing/triagent/) · [CodeCanvas](https://github.com/UniqueDevJing/CodeCanvas/)

</div>
