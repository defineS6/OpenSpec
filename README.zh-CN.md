<p align="center">
  <a href="https://github.com/Fission-AI/OpenSpec">
    <picture>
      <source srcset="assets/openspec_bg.png">
      <img src="assets/openspec_bg.png" alt="OpenSpec 标志">
    </picture>
  </a>
</p>

<p align="center">
  <a href="README.md">English</a> | <a href="README.zh-CN.md">简体中文</a>
</p>

<p align="center">
  <a href="https://github.com/Fission-AI/OpenSpec/actions/workflows/ci.yml"><img alt="CI" src="https://github.com/Fission-AI/OpenSpec/actions/workflows/ci.yml/badge.svg" /></a>
  <a href="https://www.npmjs.com/package/@fission-ai/openspec"><img alt="npm 版本" src="https://img.shields.io/npm/v/@fission-ai/openspec?style=flat-square" /></a>
  <a href="./LICENSE"><img alt="许可证：MIT" src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" /></a>
  <a href="https://discord.gg/YctCnvvshC"><img alt="Discord" src="https://img.shields.io/discord/1411657095639601154?style=flat-square&logo=discord&logoColor=white&label=Discord&suffix=%20online" /></a>
</p>

<details>
<summary><strong>最受喜爱的规格框架。</strong></summary>

[![Stars](https://img.shields.io/github/stars/Fission-AI/OpenSpec?style=flat-square&label=Stars)](https://github.com/Fission-AI/OpenSpec/stargazers)
[![Downloads](https://img.shields.io/npm/dm/@fission-ai/openspec?style=flat-square&label=Downloads/mo)](https://www.npmjs.com/package/@fission-ai/openspec)
[![Contributors](https://img.shields.io/github/contributors/Fission-AI/OpenSpec?style=flat-square&label=Contributors)](https://github.com/Fission-AI/OpenSpec/graphs/contributors)

</details>
<p></p>
我们的理念：

```text
→ 灵活，而非僵化
→ 迭代，而非瀑布式
→ 简单，而非复杂
→ 不只为全新项目打造，也适用于现有项目
→ 从个人项目到企业项目均可扩展
```

> [!TIP]
> **全新工作流现已推出！** 我们使用新的制品引导式工作流重构了 OpenSpec。
>
> 运行 `/opsx:propose "你的想法"` 即可开始。→ [在此了解更多](docs/opsx.md)

<p align="center">
  在 X 上关注 <a href="https://x.com/0xTab">@0xTab</a> 获取最新动态 · 加入 <a href="https://discord.gg/YctCnvvshC">OpenSpec Discord</a> 获取帮助并参与讨论。
</p>

<!-- TODO: 添加 /opsx:propose → /opsx:archive 工作流的 GIF 演示 -->

## 实际效果

```text
你：/opsx:propose add-dark-mode
AI：已创建 openspec/changes/add-dark-mode/
    ✓ proposal.md — 为什么要做，以及将发生哪些变化
    ✓ specs/       — 需求和场景
    ✓ design.md    — 技术方案
    ✓ tasks.md     — 实现清单
    可以开始实现了！

你：/opsx:apply
AI：正在实现任务……
    ✓ 1.1 添加主题上下文提供器
    ✓ 1.2 创建切换组件
    ✓ 2.1 添加 CSS 变量
    ✓ 2.2 接入 localStorage
    所有任务均已完成！

你：/opsx:archive
AI：已归档至 openspec/changes/archive/2025-01-23-add-dark-mode/
    规格已更新，可以开始下一个功能了。
```

<details>
<summary><strong>OpenSpec 仪表板</strong></summary>

<p align="center">
  <img src="assets/openspec_dashboard.png" alt="OpenSpec 仪表板预览" width="90%">
</p>

</details>

## 快速开始

**需要 Node.js 20.19.0 或更高版本。**

全局安装 OpenSpec：

```bash
npm install -g @fission-ai/openspec@latest
```

然后进入你的项目目录并初始化：

```bash
cd your-project
openspec init
```

现在告诉你的 AI：`/opsx:propose <你想构建的内容>`

如果你想使用扩展工作流（`/opsx:new`、`/opsx:continue`、`/opsx:ff`、`/opsx:verify`、`/opsx:bulk-archive`、`/opsx:onboard`），请使用 `openspec config profile` 选择该工作流，并通过 `openspec update` 应用。

> [!NOTE]
> 不确定你的工具是否受支持？[查看完整列表](docs/supported-tools.md)——我们已支持 25 种以上的工具，并且还在不断增加。
>
> 同样支持 pnpm、yarn、bun 和 nix。[查看安装选项](docs/installation.md)。

## 文档

→ **[入门指南](docs/getting-started.md)**：第一步<br>
→ **[工作流](docs/workflows.md)**：组合与模式<br>
→ **[命令](docs/commands.md)**：斜杠命令与技能<br>
→ **[CLI](docs/cli.md)**：终端参考<br>
→ **[支持的工具](docs/supported-tools.md)**：工具集成与安装路径<br>
→ **[核心概念](docs/concepts.md)**：了解各部分如何协同工作<br>
→ **[多语言](docs/multi-language.md)**：多语言支持<br>
→ **[自定义](docs/customization.md)**：按你的需求定制


## 社区 Schema

由独立仓库分发的第三方 Schema 包——它们提供了一套将 OpenSpec 与其他工具集成的特色工作流，类似于 [github/spec-kit 的社区扩展目录](https://github.com/github/spec-kit/tree/main/extensions) 对工具集成的处理方式。

→ 在自定义文档中**[浏览目录](docs/customization.md#community-schemas)**。


## 为什么选择 OpenSpec？

AI 编程助手功能强大，但如果需求只存在于聊天记录中，其表现便难以预测。OpenSpec 增加了轻量级规格层，让你在编写任何代码之前，先对要构建的内容达成共识。

- **构建前先达成共识**——人类与 AI 在编写代码前就规格达成一致
- **保持井然有序**——每项变更都有独立文件夹，其中包含提案、规格、设计和任务
- **灵活工作**——随时更新任何制品，不受僵化阶段关卡的限制
- **使用你的工具**——通过斜杠命令支持 20 多种 AI 助手

### 横向对比

**对比 [Spec Kit](https://github.com/github/spec-kit)**（GitHub）——全面但较为笨重。它有僵化的阶段关卡、大量 Markdown 和 Python 环境设置。OpenSpec 更轻量，让你能够自由迭代。

**对比 [Kiro](https://kiro.dev)**（AWS）——功能强大，但会被锁定在其 IDE 中，并且只能使用 Claude 模型。OpenSpec 可与你已经使用的工具配合工作。

**对比不使用规格**——在没有规格的情况下使用 AI 编程，意味着提示含糊且结果不可预测。OpenSpec 无需繁琐仪式即可带来可预测性。

## 更新 OpenSpec

**升级软件包**

```bash
npm install -g @fission-ai/openspec@latest
```

**刷新代理说明**

在每个项目中运行以下命令，以重新生成 AI 指引并确保最新的斜杠命令已启用：

```bash
openspec update
```

## 使用说明

**模型选择**：OpenSpec 最适合搭配高推理能力模型使用。对于规划和实现，我们推荐 Codex 5.5 和 Opus 4.7。

**上下文管理**：OpenSpec 在干净的上下文窗口中效果更佳。开始实现前请清理上下文，并在整个会话过程中保持良好的上下文管理习惯。

## 贡献

**小型修复**——错误修复、拼写纠正和小幅改进可以直接通过 PR 提交。

**较大变更**——对于新功能、重大重构或架构变更，请先提交 OpenSpec 变更提案，以便我们在实现前就意图和目标达成一致。

编写提案时，请牢记 OpenSpec 的理念：我们服务于使用不同编程代理、模型和用例的广大用户。变更应当适合所有人使用。

**欢迎 AI 生成的代码**——只要它经过测试和验证。包含 AI 生成代码的 PR 应注明所使用的编程代理和模型（例如，“Generated with Claude Code using claude-opus-4-5-20251101”）。

### 开发

- 安装依赖：`pnpm install`
- 构建：`pnpm run build`
- 测试：`pnpm test`
- 在本地开发 CLI：`pnpm run dev` 或 `pnpm run dev:cli`
- 约定式提交（单行）：`type(scope): subject`

## 其他

<details>
<summary><strong>遥测</strong></summary>

OpenSpec 会收集匿名使用统计信息。

我们只收集命令名称和版本，以了解使用模式。不会收集参数、路径、内容或个人身份信息（PII）。在 CI 中会自动禁用。

**选择退出：** `export OPENSPEC_TELEMETRY=0` 或 `export DO_NOT_TRACK=1`

</details>

<details>
<summary><strong>维护者与顾问</strong></summary>

有关帮助指导项目的核心维护者和顾问名单，请参阅 [MAINTAINERS.md](MAINTAINERS.md)。

</details>



## 许可证

MIT
