# Selection Workflow

This workflow defines what "review every skill" means in production: inspect the full inventory, decide relevance, then load only the source skills needed for the current task.

## Mandatory Pass

1. Read `skill_inventory.md`.
2. For each listed skill, classify it as:
   - `required`: needed to complete the user's current deliverable.
   - `optional`: useful only if the user asks for extra depth or a specific artifact.
   - `irrelevant`: not needed for this task.
3. Load `SKILL.md` only for `required` skills and for any `optional` skill that becomes necessary.
4. When a selected skill has references, load only the reference files named by that skill for the current task.

## Default Priority

Use this order unless the user request clearly starts later in the workflow:

1. `file-reference`, `text-splitter`, `text-truncator`, or `novel-truncator` for source handling.
2. `story-*`, `character-*`, `plot-*`, and `drama-analyzer` for story understanding.
3. `drama-planner`, `drama-creator`, `shanyin-screenwriting-master`, `knowledge-query`, or `web-search` for planning and development.
4. `novel-evaluator`, `story-outline-evaluator`, `drama-evaluator`, `script-evaluator`, `ip-evaluator`, or `score-analyzer` for evaluation.
5. `shortdrama-production-memory`, `seedance-storyboard`, and `.system/imagegen` for visual/video production.
6. `result-integrator`, `output-formatter`, and optionally `mind-map-generator` for final packaging.

## Scenario Routing

| User Task | Required Skills | Optional Skills |
| --- | --- | --- |
| 根据剧本做竖屏短剧分镜和 Seedance 提示词 | `file-reference`, `drama-analyzer`, `shortdrama-production-memory`, `seedance-storyboard` | `character-profile`, `character-relationships`, `output-formatter` |
| 评估小说能不能改短剧 | `novel-summarizer`, `story-five-elements`, `novel-evaluator`, `drama-evaluator`, `ip-evaluator` | `score-analyzer`, `web-search`, `output-formatter` |
| 整理长文本并输出综合报告 | `text-splitter` or `text-truncator`, relevant analysis skills, `result-integrator`, `output-formatter` | `mind-map-generator` |
| 从零策划短剧项目 | `story-type-analyzer`, `drama-planner`, `drama-creator` | `knowledge-query`, `web-search`, `story-outline-evaluator` |
| 写剧本、短片、长片或剧集 | `shanyin-screenwriting-master` | `drama-creator`, `story-five-elements`, `character-profile`, `plot-keypoints`, `output-formatter` |
| 制作融图首帧或视频画面提示词 | `shortdrama-production-memory` | `.system/imagegen`, `seedance-storyboard` |
| 维护 skill 或创建新 skill | `.system/skill-creator` | `.system/skill-installer`, `.system/plugin-creator` |

## Production Constraints

- Keep source boundaries strict: provided script, shot script, character references, scene references, and prop references are the only creative source unless the user asks for invention.
- Preserve dialogue and inner monologue exactly when the source provides them.
- Do not use `同上`, `同前`, or omitted descriptions in production prompts.
- For video tasks, preserve spatial continuity, action causality, character staging, lighting motivation, and edit-point clarity.
- Use current web search only when the output depends on recent market, platform, legal, model, pricing, or product facts.

## Reporting Selection

For complex tasks, include a short routing note:

`本次总集已过技能索引，选用：A（原因）、B（原因）、C（原因）。`

For simple production output, keep the routing note to one sentence or omit it if the user asked only for the deliverable.
