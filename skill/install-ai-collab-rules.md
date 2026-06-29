---
name: install-ai-collab-rules
description: 一键安装 AI 协作规范（AI_ENTRY.md + DECISIONS.md + COLLAB.md + SESSION_HANDOFF.md），适用于多 AI 协同的项目
---

# Install AI Collaboration Rules

Install the four-file AI collaboration protocol (AI_ENTRY.md + DECISIONS.md + COLLAB.md + SESSION_HANDOFF.md) into the current project.

## Usage

```
/install-ai-collab-rules <project-name> [language:zh|en]
```

## Steps

1. Read the templates from `docs/ai-collab-patterns/`
2. For each template, replace placeholders (【project-name】, 【path】, etc.) with actual project values
3. Write `AI_ENTRY.md` to project root
4. Write `DECISIONS.md` to project root  
5. Write `COLLAB.md` to project root
6. Write `SESSION_HANDOFF.md` to project root
7. Verify files are created

## Rules  

- Preserve the project name, tech stack, and directory structure from real project analysis
- Keep the three core principles: SoT priority, decision records, cost confirmation
- Don't add rules that are specific to IAIBench (T/V axis, C2.3, etc.)
- Default to Chinese language unless `en` is specified
