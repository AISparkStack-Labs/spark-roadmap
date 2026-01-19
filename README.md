# AISparkStack

> 把灵感火花变成开箱即用、可复用的工程栈。

AISparkStack 是一个开源矩阵，围绕「简单易用」「可复用」「可持续迭代」构建。
你可以把它理解为：一套可复制的工程模板 + 一组可复用的工具库 + 一批可运行的示例工程。

---

## 🧭 Matrix Map（项目总览）

### ⭐ Pinned（置顶 6 个仓库）
- **spark-roadmap**：索引 / 路线图 / 贡献入口
- **spark-template**：通用模板（所有项目通用的骨架与规范）
- **spark-starter**：统一“开箱即用”入口（端到端最小闭环示例）
- **spark-toolkit**：可复用工具库（跨项目共用）
- **spark-rag-starter**：RAG 示例工程（写教程、做内容的最佳抓手）
- **spark-evals**：评测/基准（专家形象与可验证能力）

> 说明：具体技术栈写在各仓库 README，并用 GitHub Topics 标注（如 go / flutter / unity / unreal / hardware 等）。

---

## 🧩 Categories（5 大类项目）

> 规则：仓库名只表达“类别 + 主题”，不包含技术栈；同类多技术实现用仓库内子目录区分。

### 1) Server（服务端）
目标：稳定、可扩展、可部署的服务端模板与示例（含接口规范、错误码、日志、配置、CI/CD 约定等）
- 推荐仓库：
  - spark-server-starter（示例入口）
  - spark-toolkit（服务端也会依赖的通用能力）
- 典型子目录（示例）：
  - /go/ ...

### 2) Client（客户端）
目标：开箱即用的客户端工程结构（网络层、路由、状态管理、环境切换、构建）
- 推荐仓库：
  - spark-client-starter
- 典型子目录：
  - /flutter/ ...

### 3) Game2D（2D 游戏）
目标：2D 工程模板与规范（资源目录、命名规则、可复用 UI/场景示例）
- 推荐仓库：
  - spark-game2d-starter
- 典型子目录：
  - /unity/ ...

### 4) Game3D（3D 游戏）
目标：3D 工程模板与规范（Unity/Unreal 的工程约定、资源治理、性能与打包建议）
- 推荐仓库：
  - spark-game3d-starter
- 典型子目录：
  - /unity/ ...
  - /unreal/ ...

### 5) Hardware（硬件相关）
目标：把“硬件项目最容易乱”的部分标准化：协议、固件、上位机、验证流程
- 推荐仓库：
  - spark-hardware-starter
- 典型子目录：
  - /protocol/（通信协议与版本化）
  - /firmware/（固件工程骨架）
  - /host/（上位机/接入侧示例）

---

## 🚀 Getting Started

### Step 1：从模板创建新项目
1. 打开 **spark-template**
2. 点击 **Use this template**
3. 新建仓库命名：`spark-<category>-<topic>`
4. 填好 README 的 Quick Start（必须做到“5 分钟跑起来”）

### Step 2：按规范提交 PR
- 所有变更走 PR（即使只有维护者自己）
- PR 必须包含：变更摘要 / 影响范围 / 验证方式 / 是否 Breaking

### Step 3：打第一个版本
- 完成最小可运行 + CI 绿色后打 tag：`v0.1.0`
- 同步更新 `CHANGELOG.md` + GitHub Release Notes

---

## 📦 Repository Naming（命名规范）

### 前缀
统一：`spark-`

### 格式
- 通用：`spark-<category>-<topic>`
- 简化：`spark-<topic>`（少数门面仓库可用，比如 spark-template）

### Category 固定词表
- server / client / game2d / game3d / hardware

> 技术栈不进仓库名：写在 README 的第一屏，并用 Topics 标注。

---

## ✅ Quality Bar（最低质量门槛：必须满足）

每个仓库（至少）必须具备：
- README：3 分钟读懂 + 5 分钟跑起来
- LICENSE
- CONTRIBUTING / SECURITY / CODE_OF_CONDUCT
- CHANGELOG + 版本 tag（从 v0.1.0 起）
- CI：最少 lint/test（游戏/硬件可先做可选，但要写清验证方式）

---

## 🤝 Contributing（如何参与？）
- 从 `good first issue` 开始（我们会优先把任务拆成可协作颗粒度）
- 提交 PR 前请确保：
  - 能本地跑通（或说明无法跑通的原因）
  - CI 通过
  - 文档同步更新（若涉及使用方式变化）

---

## 🗺️ Roadmap（路线图）
我们会按节奏推进：
- v0.1：每个核心仓库具备 Quick Start + CI + tag
- v0.2：抽出更多可复用模块（toolkit/sdk/协议规范）
- v1.0：形成端到端示例闭环（服务端 + 客户端 + 游戏接入 +（可选）硬件接入）

---

## 📣 Follow / Updates（关注更新）
- Release：以 GitHub Releases 为准
- 讨论：Issues / Discussions

---

## 📄 License
默认使用宽松许可证（MIT / Apache-2.0 之一），以各仓库 LICENSE 为准。
