# Ops Toolbox

> 运维实用工具箱：生产环境排错笔记、自动化运维脚本与现成配置模板沉淀。

---

## 📂 目录导航与结构

在 Markdown 中，纯文本代码块内无法添加超链接，因此推荐使用 **交互式快速导航（可点击跳转）** 配合 **树状层级概览**。

### 🚀 快速导航（点击直达对应目录）

- 📁 [**`docs/`**](docs/) — 运维排错笔记、架构心得、Cheatsheet
  - 📂 [**`kubernetes/`**](docs/kubernetes/) — K8s 运维经验、集群配置与故障排查
- 📁 [**`scripts/`**](scripts/) — 自动化 Shell / PowerShell 脚本
  - 📂 [**`maintenance/`**](scripts/maintenance/) — 日常系统巡检、日志清理与磁盘维护
  - 📂 [**`cert-renew/`**](scripts/cert-renew/) — SSL/TLS 证书管理与自动化续期脚本
- 📁 [**`templates/`**](templates/) — 生产级现成配置文件与模板
  - 📂 [**`grafana/`**](templates/grafana/) — Grafana Dashboard 仪表盘配置 (JSON)
  - 📂 [**`prometheus/`**](templates/prometheus/) — 监控告警规则与抓取配置

---

### 🌳 树状层级视图

```plaintext
ops-toolbox/
├── docs/                # 运维排错笔记、架构心得与 Cheatsheet
│   └── kubernetes/      # K8s 运维经验与集群配置
├── scripts/             # 自动化 Shell / PowerShell 脚本
│   ├── maintenance/     # 日常巡检、磁盘清理等
│   └── cert-renew/      # 证书管理与自动化更新任务
└── templates/           # 生产级现成配置文件与模板
    ├── grafana/         # Grafana Dashboard 仪表盘 JSON
    └── prometheus/      # 监控告警规则与配置
```

---

## 📌 使用与沉淀规范

1. **文档规范**：新添加的排错笔记与经验分享放入 [**`docs/`**](docs/) 下对应技术栈目录，推荐 Markdown 格式并附带拓扑或关键日志。
2. **脚本规范**：所有 [**`scripts/`**](scripts/) 目录下的脚本建议在头部添加作者、参数说明、测试环境及用法示例，且执行时需具备参数检查与错误容忍机制。
3. **配置模板**：[**`templates/`**](templates/) 中的配置文件建议去除敏感信息（如密码、AK/SK 等），改用占位符（如 `<YOUR_SECRET>`）标注。
