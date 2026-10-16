---
name: make-knowledge-cards
description: Turn pasted articles or local Markdown and TXT files into concise, source-faithful knowledge cards for learning and review.
---

# Make Knowledge Cards

Convert the user's pasted article or supplied local `.md`/`.txt` file into a compact set of knowledge cards. Do not fetch webpages, process PDFs, create Anki decks, or build a graphical interface.

## Workflow

1. Read the full supplied text or requested local file. For files, use the available file tools and report a clear access or format limitation if it cannot be read. Do not search for or retrieve additional source material.
2. Identify the article's central claims, definitions, mechanisms, distinctions, and actionable procedures. Prefer ideas that explain or connect other points; omit anecdotes and supporting detail unless needed to understand a core idea.
3. Merge repeated ideas and keep each card focused on one independently useful knowledge point. Do not split one idea into several cards merely to reach a target count.
4. Produce 5–8 cards when the source supports that many distinct, useful points. If it does not, produce fewer and briefly say that the source did not contain enough distinct material. Never pad the set.
5. Ground every statement in the source. Preserve qualifications, uncertainty, scope, and causal direction. Do not add outside facts, unstated explanations, or invented examples. If a helpful example cannot be drawn faithfully from the source, use a self-test question instead.

## Card format

Use this consistent Markdown structure:

### 1. <Specific title>
- **核心知识：** <One focused idea, explained clearly and briefly.>
- **例子 / 自测：** <A concise source-grounded example, or a question answerable from the source.>

Give every card a concise, informative title. Keep the core explanation to the point; the example or question should reinforce that same knowledge point, not introduce a second one. Vary examples and self-test questions as appropriate. After the cards, optionally add one brief note when the source was ambiguous, incomplete, or too short for five distinct cards.
