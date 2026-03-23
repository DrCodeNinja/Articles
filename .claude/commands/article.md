---
description: Create an article document from provided content
allowed-tools: [Write, Read, Glob, Bash(ls:*)]
---

# Create Article

Create a well-structured article document from the provided content.

## Input

The user will provide content after the `/article` command: $ARGUMENTS

## Instructions

1. Read the provided content carefully
2. Determine the best, descriptive file name for the article based on its content:
   - Use kebab-case (e.g., `getting-started-with-docker.md`)
   - Keep it concise but descriptive (3-6 words)
   - The name should clearly reflect the article's main topic
3. Check the current working directory for existing files to avoid name conflicts
4. Create the article as a `.md` file in the current working directory with:
   - A clear, engaging title (H1)
   - Well-organized sections with appropriate headings
   - Clean markdown formatting
   - The content provided by the user, structured into logical sections
   - Make the article visually attractive and engaging (see Styling Rules below)
5. Tell the user the file name you chose and why

## Styling Rules (Make Articles Attractive)

- Add relevant emojis to **section headings** to make them visually appealing (e.g., `## 🚀 Getting Started`, `## 📦 Installation`)
- Add an emoji to the **main title (H1)** as well
- Use emojis in **bullet points** where appropriate to highlight key concepts (e.g., `* ✅ Easy to use`, `* ⚡ Fast performance`)
- Use **bold** and *italic* text to emphasize important terms and concepts
- Add horizontal rules (`---`) between major sections for visual separation
- Use blockquotes (`>`) for important tips, notes, or key takeaways
- Keep emoji usage tasteful and relevant — don't overdo it, aim for 1 emoji per heading and selective use in lists
- Choose emojis that match the topic/context (e.g., 🔧 for setup, 📊 for monitoring, 🌐 for web/cloud, 🗄️ for databases)

## Footer

Always add the following footer at the very end of every article (after the conclusion):

```
---

## ⭐ Found This Helpful?

If you found this article helpful, please give this repository a star on GitHub! It helps others discover these articles too.

[![GitHub Stars](https://img.shields.io/github/stars/DrCodeNinja/Articles?style=social)](https://github.com/DrCodeNinja/Articles)

👉 [**Star this repository**](https://github.com/DrCodeNinja/Articles) — your support means a lot! 🙌
```

## General Rules

- Do NOT change the meaning or intent of the user's content
- DO improve structure, formatting, and readability
- If the content is already well-structured, preserve its structure while adding the styling enhancements
- Always include the footer section at the end of every article
- Save the file in the current working directory (E:/My/Articles)
