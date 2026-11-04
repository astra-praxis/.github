# astra-praxis · .github

组织主页展示页在 [profile/README.md](profile/README.md)，渲染于 https://github.com/astra-praxis 。

动画素材在 [profile/assets/](profile/assets)：纯手写 SVG（SMIL，无 JS、无第三方统计服务）。

| 文件 | 用在哪 |
| --- | --- |
| `profile/assets/banner.svg` | 页首标题动画 |
| `profile/assets/boot.svg` | `astra --boot` 终端自检动画 |
| `profile/assets/engine.svg` | 引擎室数据流示意图 |

> 注意：GitHub 组织主页 README 里的**相对路径图片不会解析到本仓库**（会被重写成 `github.com/astra-praxis/assets/...` 而 404），所以 `profile/README.md` 里统一用 `raw.githubusercontent.com` 绝对地址。

## 内容维护

`profile/README.md` 里的「仓库地图」一节，把组织下每个仓的职责写清楚：

- **公开仓**（astra / astra-bot / astra-memory-mcp / .github）给链接与详细职责。
- **内部仓**（astra-core / astra-serve / astra-desktop / astra-workflow / astra-memory / astra-bid / jev-test）只写一句定位，**不挂链接**，避免把还没交付的东西指给访客。

新增仓库或某仓转公开时，记得同步改这一节；职责描述以该仓自己 README 为准，不要凭印象写。

本仓库只放组织级配置与展示内容。
