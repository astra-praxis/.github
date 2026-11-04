<div align="center">

# ✦ ASTRA PRAXIS

**Astra 是星，Praxis 是动手。**
星图画在你自己的硬盘上。

</div>

```text
$ astra --boot
[ ok ] 权限引擎 ......... 已挂载 · 越权硬拦截
[ ok ] 长期记忆 ......... 已加密 · 仅存本机
[ ok ] 工具舱 .......... 文件 · 命令 · 搜索 · MCP · Skills
[ ok ] Serve 宿主 ...... 在线 · 无人值守待命
[ >> ] 等待你的第一条指令 _
```

<div align="center">

[![Astra release](https://img.shields.io/github/v/release/astra-praxis/astra?style=flat-square&label=astra&color=5b4dff)](https://github.com/astra-praxis/astra/releases)
![platforms](https://img.shields.io/badge/macOS%20%C2%B7%20Windows%20%C2%B7%20Linux-Tauri%202-111111?style=flat-square)

**local-first AI Agent 桌面应用** —— 选一个工作目录，用对话让它读文件、改文件、跑命令、搜网页、写文档、出图。会话多开几扇标签；每次伸手碰工具，都先过权限引擎；记得住的东西加密后留在本机。模型走 OpenAI 兼容接口就行，本地服务也可以。

### 脑子可以借，抽屉是自己的。

</div>

## 🗺 航图 · 你大概是来找这些的

| 想做什么 | 去哪 | 备注 |
| --- | --- | --- |
| 🚀 **现在就用** | [astra Releases](https://github.com/astra-praxis/astra/releases) | macOS / Windows / Linux 安装包都在这 |
| 🖥 **参观驾驶舱** | [astra](https://github.com/astra-praxis/astra) | Tauri 2 + Rust + React。能力、权限，以及还没做完的部分，README 写得很坦白 |
| 🛰 **让 Agent 值夜班** | [astra-bot](https://github.com/astra-praxis/astra-bot) | 只放 `astra-serve-host` 二进制和自动下载用的 [latest.json](https://github.com/astra-praxis/astra-bot/blob/main/latest.json)，源码不在这 |
| 🧠 **把记忆接给别的 Agent** | [astra-memory-mcp](https://github.com/astra-praxis/astra-memory-mcp) | 记忆 MCP：stdio、本地加密 SQLite，没有云也没有遥测。Cursor、Claude Code、DeepSeek Harness 都能接；换模型，记忆还跟着你 |

## 🛸 座舱里现在有的

| 系统 | 能干什么 |
| --- | --- |
| 🗂 工作区 | 在你点名的目录里读、改、管理文件 |
| 🧰 工具舱 | 文件、命令、网页搜索，再加 MCP、ACP 和 Skills |
| 💬 会话 | 多标签并行，历史能翻回来接着做 |
| 🛡 权限 | 分级放权，越权硬拦截；工具吐出来的内容不会因此多得到任何权限 |
| 🧠 记忆 | 跨会话沉淀，本地加密；记错了可以纠正，旧结论会失效 |
| 📦 Artifact | 任务生成的文档和结果集中放 |
| 🌗 三端安装包 | macOS、Windows、Linux，从 Releases 走 |

## ⚙️ 引擎室

```mermaid
flowchart TD
  You["你选定工作目录"] --> Astra["Astra"]
  Astra --> Tools["文件 · 命令 · 搜索"]
  Astra --> Ext["MCP / ACP / Skills"]
  Astra --> Mem["加密长期记忆"]
  Model["模型 API 或本地模型"] -.-> Astra
  Host["astra-serve-host"] -.-> Astra
```

## 🚀 起飞

1. 打开 **[astra Releases](https://github.com/astra-praxis/astra/releases)**，领你那块系统的安装包。
2. 在设置里填一个 OpenAI 兼容的模型服务。
3. 选一个工作目录，把任务说清楚。剩下的交给它。

记忆要单独接：去 [astra-memory-mcp Releases](https://github.com/astra-praxis/astra-memory-mcp/releases) 拿对应平台的二进制。

<details>
<summary>📖 船员守则（我们造东西的原则）</summary>

- **Local-first**：星图画在你自己的硬盘上，不在别人的服务器上。
- **密钥留舰**：API key 不出本机。
- **权限先行**：Agent 每次伸手碰工具，都先过权限引擎。
- **坦白从宽**：没做完的就写没做完，README 里不吹牛。

</details>

## 📡 船员日志

> runtime / core 还在灶上，公开航图里先不挂链接。能下载、能接上的，就是上面航图里的三处。

---

合用的话，给 [astra](https://github.com/astra-praxis/astra) 一颗 **Star** —— 这是本舰唯一的燃料。或者 **Watch** 它的 Releases，新安装包出来你会先知道。

---

桌面应用许可证是 [MIT](https://github.com/astra-praxis/astra/blob/main/LICENSE)。记忆组件的许可见它自己的仓库。`astra-serve-host` 二进制按现状分发。有问题或想法，到对应仓库开 Issue。
