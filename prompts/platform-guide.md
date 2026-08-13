# Platform Guide

通用 Prompt 不依赖特定模型。不同平台只需调整输入方式。

## ChatGPT

- 直接上传 PDF、DOCX 或截图，再粘贴通用 Prompt。
- 长简历先要求输出事实账本，确认后再生成最终版。
- 使用 Projects 时，可将通用 Prompt 放入项目说明中重复使用。

## Claude

- 适合一次输入简历、职位描述和项目补充材料。
- 要求 Claude 用 `<verified>`、`<needs-confirmation>` 区分事实，可降低长上下文中的归因混淆。
- 最终输出前再运行一次 `Interviewer` 模式。

## Gemini

- 上传 Google Drive 文档或 PDF 后，明确要求读取所有页面。
- 若输出过于概括，要求逐项目保留“个人边界”和“关键机制”。

## DeepSeek / Kimi / 豆包

- 文本输入最稳定；复杂版式简历建议先提取为 Markdown。
- 如果上下文有限，按“事实账本 -> 单个项目改写 -> 整体合并”分三轮执行。
- 不要在不同轮次省略事实账本，否则容易产生未经确认的数字。

## 本地模型

- 将通用 Prompt 设为 system prompt 或首轮用户消息。
- 小模型建议先使用 `Audit`，每次只处理一个项目。
- 无视觉能力时，先通过 OCR 或 PDF 文本抽取转成 Markdown。
