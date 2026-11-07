<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=2800&pause=900&color=5B46F2&center=true&vCenter=true&width=780&lines=Hi%2C+I'm+Jing+%F0%9F%91%8B;AI+Agent+%26+Application+Engineer;I+build+agents+that+self-verify+before+shipping." alt="typing" />

**把「AI 能写代码」做成「AI 交付可用软件」——带校验、带护栏、带预算、可审计。**

[![Projects](https://img.shields.io/badge/Projects-3-5B46F2?style=flat-square)](#-我在做什么)
[![Tests](https://img.shields.io/badge/Tests-1000%2B-16a34a?style=flat-square)](#-工程质量)
[![CI](https://img.shields.io/badge/CI-all%20green-brightgreen?style=flat-square)](#-工程质量)

</div>

---

## 🚀 我在做什么

三个可运行、有测试、有 CI 的项目，覆盖 AI 应用开发的三种主流形态：

| 项目 | 一句话定位 | 关键能力 |
|---|---|---|
| **[CodeCanvas](https://github.com/UniqueDevJing/CodeCanvas)** | 一句话生成**可运行**的前端应用，并自检自愈到可交付 | 多阶段 Agent 编排 · 运行时验证 · 自愈修复 · 视觉能力网关（配图 + 预算 + 降级）· SSE 契约快照 |
| **[triagent](https://github.com/UniqueDevJing/triagent)** | 医疗**多智能体分诊**，把"能力边界"写进代码 | 角色→能力→工具白名单 · 输入/输出护栏（fail-closed）· 决策日志与回放 · 100 例红队 · 变异测试 |
| **[Mira](https://github.com/UniqueDevJing/Mira)** | 可评测的 **RAG 问答**，把"效果好"变成可度量 | 混合检索与重排 · 分级拒答 · 降级等级 · RAGAS 评测 · 性能回归门禁（P95）· 多模态检索基座 |

---

## 🧠 技术栈

<div align="center">

![Java](https://img.shields.io/badge/Java%2017-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Spring AI](https://img.shields.io/badge/Spring%20AI-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Python](https://img.shields.io/badge/Python%203.13-3776AB?style=for-the-badge&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Vue](https://img.shields.io/badge/Vue%203-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

</div>

---

## 🛠 工程质量（我关心的不是"能跑"，而是"敢上线"）

<table>
<tr><td width="50%">

**测试分层**
- 单元 → 契约 → 集成（真 MySQL/Redis）→ 真机 E2E
- 契约快照锁协议：SSE 事件名、DTO 字段、工具 schema
- 红队：文本 75 例 + 图像 25 例

</td><td width="50%">

**质量门禁**
- CI 全绿才进主干（三个仓）
- 覆盖率门禁 + 分层 80%
- 性能回归门禁：P95 退化 >10% 直接失败
- 变异测试：量化"断言强度"而非"执行过"

</td></tr>
</table>

---

## 📈 GitHub 数据

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=UniqueDevJing&show_icons=true&hide_border=true&theme=tokyonight&include_all_commits=true&count_private=true" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=UniqueDevJing&layout=compact&hide_border=true&theme=tokyonight&langs_count=8" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=UniqueDevJing&hide_border=true&theme=tokyonight" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=UniqueDevJing&theme=tokyo-night&hide_border=true&area=true" />

</div>

---

## 🎯 我关注的问题

- **可验证性**：生成的页面到底能不能打开、点了按钮会不会报错——用真浏览器验，不靠模型自述
- **安全边界**：医疗/健康场景下，"不做什么"比"能做什么"更重要（护栏 fail-closed）
- **成本与延迟**：Agent 会自己循环，所以必须有预算、超时与熔断
- **可解释**：每一次工具调用、每一次拦截，都要能事后审计与回放

---

<div align="center">

**愿意聊聊 AI 应用落地、Agent 工程化、以及怎么把 Demo 变成产品。**

[CodeCanvas](https://github.com/UniqueDevJing/CodeCanvas) · [triagent](https://github.com/UniqueDevJing/triagent) · [Mira](https://github.com/UniqueDevJing/Mira)

<sub>README 会随项目演进更新 · 最近更新：2026-11</sub>

</div>