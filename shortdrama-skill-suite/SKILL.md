---
name: shortdrama-skill-suite
description: 统一调度短剧制作技能总集。用于竖屏短剧、AI视频、分镜、融图提示词、Seedance提示词、剧本分析、故事梗概、人物小传、人物关系、情节点、戏剧功能、短剧策划、IP/小说/大纲/剧本评估、知识库检索、长文本处理、输出整理，以及需要先过一遍全部skill再综合选择当前任务所需技能的制作流程。
---

# Shortdrama Skill Suite

## Core Rule

Use this skill as the entry point for short-drama and video production work.

Always read [references/skill_inventory.md](references/skill_inventory.md) first, then read [references/selection_workflow.md](references/selection_workflow.md). Treat the inventory pass as mandatory: review every listed skill by name, purpose, trigger, and production frequency before deciding which source skills to load.

Do not load every referenced `SKILL.md` in full by default. Use the inventory to select the smallest relevant set, then read only the selected source skills and their task-specific references.

## Workflow

1. Identify the user task stage:
   - Input handling: file references, long text, novel/script/source material cleanup.
   - Story understanding: synopsis, five elements, genre, characters, relationships, plot points.
   - Development: short-drama planning, script creation, hooks, episode structure, optimization.
   - Evaluation: IP, novel, story outline, script, short-drama market potential, score analysis.
   - Production: storyboard, first-frame image fusion prompt, Seedance 2.0 video prompt, continuity, camera, lighting, voice.
   - Output: integrated report, structured final format, mind map.
   - Maintenance: skill creation, skill install, plugin creation, OpenAI docs, image generation.
2. Review the complete inventory and mark each skill as required, optional, or irrelevant for the current task.
3. Load required skills in dependency order:
   - Source/input skills before analysis.
   - Analysis skills before planning or production.
   - Production memory and Seedance skills before video prompt output.
   - Integration/formatting skills last.
4. Combine the selected skills into one production response. Preserve source boundaries and do not invent unprovided plot, dialogue, props, character details, or scene facts when the task is based on a provided script.
5. If the task asks for video, storyboard, image prompt, or Seedance output, include the identity required by `shortdrama-production-memory` before production work:
   `【身份】你现在是一名AI训练师+获奖导演+摄影师+故事板艺术家。接下来制作这部短剧时，必须严格按照剧本内容分析，不得私自删减修改原本内容。`

## Default Skill Combinations

- Long source material to production: `file-reference`, `text-splitter` or `text-truncator`, `story-five-elements`, `plot-workflow`, `drama-planner`, `shortdrama-production-memory`, `seedance-storyboard`, `output-formatter`.
- Novel/IP evaluation: `novel-summarizer`, `story-five-elements`, `novel-evaluator`, `drama-evaluator`, `ip-evaluator`, `score-analyzer`, `output-formatter`.
- Script-to-storyboard: `file-reference`, `drama-analyzer`, `character-profile`, `character-relationships`, `shortdrama-production-memory`, `seedance-storyboard`.
- Story development: `story-type-analyzer`, `story-outliner`, `plot-keypoints`, `drama-planner`, `drama-creator`.
- Multi-report consolidation: `result-integrator`, `output-formatter`, optionally `mind-map-generator`.

## Selection Discipline

- Prefer the existing specialized skill over rewriting its rules here.
- Use `.system` skills only when their trigger is explicit or materially required.
- For current-market, platform, or industry facts, use `web-search` because those facts can change.
- For OpenAI API/product questions, use `.system/openai-docs` and official OpenAI sources only.
- For image generation/editing tasks, use `.system/imagegen` or available image tools according to the task.
- For creating or updating skills, use `.system/skill-creator`; for installing skills, use `.system/skill-installer`; for plugin scaffolding, use `.system/plugin-creator`.

## Output Standard

State which skills were selected and why when the user needs traceability. For direct production deliverables, keep the skill-routing note short, then provide the requested artifact in the format required by the selected production/output skills.
