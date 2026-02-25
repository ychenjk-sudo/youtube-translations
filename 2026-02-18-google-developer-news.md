# YouTube 视频翻译：Project Genie, #GoogleIO, and more! - Google Developer News February 2026

## 视频元信息
- **视频ID**: xNW_0F8JT3U
- **视频链接**: https://www.youtube.com/watch?v=xNW_0F8JT3U
- **发布时间**: 2026-02-18
- **频道**: Google for Developers
- **时长**: 6.5 分钟
- **主题**: Google 开发者新闻 2026年2月

---

## 核心观点

### 1. DeepMind 发布 Project Genie：交互式世界生成模型
DeepMind 推出了 Project Genie，这是一个基于 Genie 3、Nano Banana Pro 和 Gemini 模型的实验性原型。它允许用户通过文本或图像提示"草绘"出世界，并以第一人称或第三人称视角实时探索这些动态生成的环境。与静态 3D 快照不同，Genie 3 能实时生成前方的路径。此外，用户还可以通过"世界混音"（World Remixing）功能，在现有世界的基础上进行二次创作。目前该功能仅面向美国 18 岁以上的 Google AI Ultra 订阅用户开放。

### 2. Android Studio Otter 3：支持任意 LLM 模型
Android Studio Otter 3 带来重大更新，最大的亮点是 AI 助手的模型选择更加自由。开发者现在不仅可以使用 Gemini，还可以选择 OpenAI、Anthropic 的模型，甚至通过 Ollama 和 LM Studio 运行本地模型。对于 Gemini 用户，使用 API Key 可以获得更高的配额（支持 Gemini 3 Flash 和 Pro）。

### 3. Android Studio 新增"Journeys"与 UI 开发增强
新推出的"Journeys"功能允许开发者使用自然语言描述端到端的 UI 测试步骤和断言，AI 会将其转化为实际的测试操作并总结结果。在 UI 开发方面，Compose Preview 深度集成了 Agent 模式，支持从设计稿或参考图直接生成代码，并能通过自然语言指令迭代修改 UI，极大地加速了从设计到实现的流程。

### 4. TranslateGemma：多尺寸开源翻译模型
Google 推出了基于 Gemma 3 构建的 TranslateGemma 开源翻译模型系列。该系列包含三种参数规模：40 亿参数（适配移动端）、120 亿参数（适配消费级笔记本）和 270 亿参数（云端）。模型在 55 种核心语言对上进行了训练和评估，并额外覆盖了近 500 种语言对，现已在 Kaggle、Hugging Face 和 Vertex AI 上线。

### 5. Genkit Go 1.4.0 发布：增强会话与评估工具
Genkit Go 更新至 1.4.0 版本，引入了实验性的 Session 功能以维持多轮对话状态，并重构了工具中断（Tool Interrupts）API 以优化"人机回环"工作流。此外，新版支持了 Anthropic 的 Claude 模型，并在 Dev UI 中上线了 Prompt 评估功能，允许开发者批量测试和对比 Prompt 效果。Genkit MCP 服务器也已登录 Antigravity MCP 商店。

### 6. Chrome 145 进入稳定版
Chrome 145 正式发布，带来了新的 CSS 样式能力，包括用于多列布局的列包裹（column wrapping）功能，以及对可自定义 select 下拉列表框的扩展支持，进一步丰富了 Web 前端的样式控制能力。

### 7. Google I/O 2026 定档五月
Google 正式宣布了年度开发者大会 Google I/O 2026 的时间。大会将于 2026 年 5 月 19 日至 20 日在加利福尼亚州山景城的海岸线圆形剧场（Shoreline Amphitheater）举行。

---

## 完整中文翻译

欢迎收看 2026 年第一期 Google 开发者新闻。本月我们带来了 DeepMind 团队最新的实验性研究原型、Android Studio 的重大功能更新、Gemma 生态系统中全新的开源翻译模型家族，以及 Genkit Go 和 Chrome 的最新动态。

我是主持人 Christine。希望大家已经关注了 Google 开发者在 2026 开年发布的所有公告。如果没有，别担心，我们这就带你一探究竟。

**DeepMind Project Genie：创造与探索世界**
首先是 Google DeepMind 团队的最新成果：DeepMind 推出了 Project Genie，这是一个让你能够创造并探索世界的实验性研究原型。Project Genie 是一个网页应用原型，由 Genie 3、Nano Banana Pro 和 Gemini 驱动，让用户能亲身体验我们世界模型的沉浸感。

Genie 3 就是这个核心的世界模型。它是一个通用世界模型，能够生成多样化、可交互的环境。与静态 3D 快照中的探索体验不同，Genie 3 会随着你在世界中的移动和交互，实时生成前方的路径。

这种体验有三个核心能力：
第一是"世界草绘"（World Sketching）：你可以通过文本和图像提示词来创建一个鲜活的、不断扩展的环境。
第二是"世界探索"（World Exploration）：你可以在创造的世界中漫游，并在探索过程中调整相机视角，支持第一人称或第三人称。
第三是"世界混音"（World Remixing）：你可以选取现有的世界，在它们的提示词基础上进行修改，加入你自己的创意。

Project Genie 目前面向美国的 Google AI Ultra 订阅用户开放，需年满 18 岁。更多关于 Project Genie 的详情，请查看描述中的博客链接。我们还附上了 DeepMind 提供的一份很棒的资源——Genie 高效提示词编写指南。

**Android Studio Otter 3：AI 模型自由选**
Android Studio Otter 3 功能满满。从这个版本开始，你可以选择任意 LLM（大语言模型）来驱动 Android Studio 中的 AI 助手。你现在可以利用 OpenAI、Anthropic 的模型，或者通过 Ollama 和 LM Studio 运行本地模型。当然，你仍然可以使用 Gemini，而且通过使用 Gemini API 密钥，你可以获得 Gemini 3 Flash 和 Pro 更高的使用限额。

**Android Studio：Journeys 与 UI 开发新体验**
Android Studio 的"Journeys"功能让你能用自然语言描述端到端 UI 测试的步骤和断言。你的一组指令（即一个 Journey）会转化为 AI 在你应用上执行的动作，它还会为你总结测试结果。

Agent 模式下的 UI 开发变得更简单了。Gemini 和 Android Studio 现在更深度地集成到了 UI 开发工作流中，直接嵌入在 Compose Preview（预览）里，帮助你更快地从设计稿转变为高质量的实现代码。

这些新能力旨在辅助你开发的每一个阶段，从初始代码生成到迭代、优化和调试，入口就在你的工作上下文中。如果你在 Compose Preview 中，你可以直接从设计模版创建一个 UI。你还可以将你的 UI 与目标图像进行匹配，上传参考设计图，Agent 就会建议出与之高度匹配的代码。你可以使用自然语言迭代修改 UI，Agent 会帮你应用代码变更。

这只是 Android Studio Otter 3 版本中旨在改善工作流和提升生产力的部分功能。要查看 Android Studio Otter 3 和 Android Studio Panda 的完整功能列表和改进，请访问 developer.android.com/studio 查看官方发布说明。你也可以查看下方链接中我们 Android Studio 开发者 YouTube 频道朋友们的视频。

**TranslateGemma：开源翻译模型**
在 Gemma 开源模型的世界里，我们推出了 TranslateGemma，这是一套基于 Gemma 3 构建的全新开源翻译模型集合，旨在帮助人们跨越 55 种语言进行交流，无论身处何地或使用何种设备。

这是因为 TranslateGemma 提供了三种参数规模：40 亿参数版本适用于移动端，120 亿参数版本适用于消费级笔记本电脑，270 亿参数版本适用于云端。TranslateGemma 在 55 个语言对上进行了训练和评估，确保在西班牙语、法语、中文和印地语等主要语言上具有可靠、高质量的表现。

但我们并未止步于此。除了这些核心语言，我们还突破界限，在近 500 个额外的语言对上进行了训练。要开始使用 TranslateGemma，你可以在 Kaggle 或 Hugging Face 上下载，在 Vertex AI 中部署，或者尝试描述中链接的 Gemma Cookbook。

**Genkit Go 1.4.0：更强的开发体验**
Genkit Go 1.4.0 版本现已发布。本次更新引入了实验性的 Session（会话）功能，用于在多轮对话中维持状态，并重构了 Tool Interrupts（工具中断）API，以实现更流畅的"人机回环"（human-in-the-loop）工作流。

如果你错过了 1.3.0 版本，现在官方已经支持了 Anthropic 的 Claude 模型、后台模型以及带重连功能的持久流式传输。

开发者体验也得到了巨大提升。Prompt（提示词）评估功能现已在 Genkit Dev UI 中上线，允许开发者通过批量测试 Prompt 并使用并排比较功能，不再仅凭感觉（vibes）来判断效果。此外，Genkit MCP 服务器现已上架 Antigravity MCP 商店，带来更强大的 AI 辅助开发体验。要开始使用 Genkit Go，请查看描述中链接的介绍视频。

**Chrome 145：CSS 新特性**
接下来是 Chrome 的新动态。Chrome 145 现已进入稳定版。这个版本带来了新的 CSS 样式能力，例如用于 CSS 多列布局的列包裹（column wrapping），以及对可自定义 select 列表框的扩展支持。这只是部分更新，要查看 Chrome 145 的完整新功能列表，请查看下方的公告链接。

**Google I/O 2026 定档**
虽然 2026 年才刚刚开始，但我们已经开始展望年度开发者盛会——Google I/O 了。没错，拿出日历记下这个日子吧，因为 Google I/O 2026 将于 5 月 19 日和 5 月 20 日在加利福尼亚州山景城的海岸线圆形剧场举行。更多详情，请访问 io.google。

以上就是 2026 年第一期新闻的全部内容。我们期待看到今年会为开发者们带来什么。我是 Christine，感谢收看，我们下期再见。

---

**翻译说明**：
- 翻译基于视频英文字幕逐字稿
