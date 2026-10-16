# make-knowledge-cards

`make-knowledge-cards` 是一个 Codex Skill，可将用户粘贴的文章或本地 Markdown/TXT 文件整理成便于复习的知识卡片。

## 解决什么问题

长文章里重要观点容易被重复内容和细节淹没。本 Skill 提炼真正重要的知识点，并整理成简短、可复习的卡片，同时保持内容忠于原文。

## 主要功能

- 每张卡片包含标题、核心知识，以及简明例子或自测问题。
- 文章内容充足时生成 5–8 张；不足时少生成，不为凑数拆分或编造知识点。
- 合并重复内容，保留原文的限定条件和不确定性。
- 支持粘贴文章及本地 `.md`、`.txt` 文件。
- 不支持网页抓取、PDF、Anki 导出或图形界面。

## 安装方法

将 `skills/make-knowledge-cards` 文件夹复制到 Codex 的 Skills 目录。默认位置为：

- Windows：`%USERPROFILE%\.codex\skills\make-knowledge-cards`
- macOS / Linux：`~/.codex/skills/make-knowledge-cards`

如果设置了 `CODEX_HOME`，请将文件夹复制到 `$CODEX_HOME/skills/make-knowledge-cards`。安装后，在 Codex 中调用 `$make-knowledge-cards`。

## 使用方法

粘贴文章并调用技能：

```text
$make-knowledge-cards
请把这篇文章整理成知识卡片：
<粘贴文章>
```

处理本地文件时，调用技能并提供 `.md` 或 `.txt` 文件路径：

```text
$make-knowledge-cards
请根据 `articles/文章.md` 制作知识卡片。
```

## 输入与输出示例

**输入：**

> 间隔练习是把学习分散到多个时间段，而不是集中在一次长时间学习中。学习者在遗忘前重新提取信息，通常比反复重读更能促进长期记忆。每次练习之间的间隔可以逐步拉长。

**输出：**

### 1. 间隔练习的基本做法 / How Spaced Practice Works
- **核心知识 / Key idea：** 将学习分散到多个时间段，并在遗忘前重新提取信息。Spread learning across multiple sessions and retrieve information again before forgetting it.
- **例子 / 自测 · Example / Check：** 间隔练习与一次长时间集中学习有什么区别？How does spaced practice differ from one long study session?

### 2. 提取练习与长期记忆 / Retrieval and Long-Term Memory
- **核心知识 / Key idea：** 原文指出，重新提取信息通常比反复重读更能促进长期记忆。The text says retrieving information usually supports long-term memory better than rereading it repeatedly.
- **例子 / 自测 · Example / Check：** 按原文，哪种做法通常更有助于长期记忆？According to the text, which practice usually helps long-term memory more?

实际卡片数量取决于原文中可区分的重要知识点；上例节选较短，因此只展示两张。
