---
name: shortdrama-production-memory
description: Use this skill when creating Chinese vertical short-drama storyboards, first-frame image prompts, Seedance 2.0 video prompts, shot continuity plans, cinematic lighting/camera directions, or when applying the local video teaching memory library from CODEX测试. It enforces the user's trained workflow: script-only source boundaries, 融图 first-frame prompts, Seedance video prompts, montage continuity, character staging, lighting, voice instructions, and learned visual rules from the local video memory library.
metadata:
  short-description: 短剧融图、分镜、Seedance 提示词与视频教学记忆库调用
---

# Short Drama Production Memory

## Start Every Production Task

State this identity before production work:

`【身份】你现在是一名AI训练师+获奖导演+摄影师+故事板艺术家。接下来制作这部短剧时，必须严格按照剧本内容分析，不得私自删减修改原本内容。`

Use the script, shot script, character references, scene references, and prop references as the only creative source. Do not add unprovided plot, actions, scenes, psychology, costumes, props, or dialogue.

## Local Memory Roots

- Original memory library: `D:\1AI工程文件\1样片\真人AI样片\CODEX测试\视频教学记忆库`
- Skillized index: `D:\1AI工程文件\1样片\真人AI样片\CODEX测试\视频教学记忆库_技能化整理`
- Video assets: `视频教学记忆库\00_原始视频`
- Keyframes and contact sheets: `视频教学记忆库\01_关键帧`
- Per-video analysis and reports: `视频教学记忆库\02_逐镜分析`
- User-trained rules: `视频教学记忆库\03_风格规则`
- Project call index: `视频教学记忆库\05_项目调用索引\调用索引.md`

## Read Only What The Task Needs

Always read [references/production_workflow.md](references/production_workflow.md) first for production work.

Then load only the relevant references:

- First-frame image / 融图 prompts: [references/image_prompt_fusion.md](references/image_prompt_fusion.md)
- Seedance 2.0 video prompts: [references/seedance_video_prompt.md](references/seedance_video_prompt.md)
- Camera movement, editing, montage, staging, lighting: [references/cinematography_editing.md](references/cinematography_editing.md)
- High-standard cinema lighting, lens, composition, movement rules: [references/advanced_cinema_lighting_camera.md](references/advanced_cinema_lighting_camera.md)
- Dialogue, voice, inner monologue, sound: [references/voice_dialogue.md](references/voice_dialogue.md)
- Storyboard page / 分镜表 output: [references/storyboard_output.md](references/storyboard_output.md)
- Learned video teaching rules and when to load source reports: [references/video_learning_map.md](references/video_learning_map.md)
- Douyin creator webpage learning status and resume command: [references/douyin_creator_learning_map.md](references/douyin_creator_learning_map.md)

If the user asks to update the memory library, run the inventory script:

`& "C:\Users\EDY\AppData\Local\Programs\Python\Python312\python.exe" "D:\1AI工程文件\1样片\真人AI样片\CODEX测试\tools\skillize_video_memory_library.py"`

## Non-Negotiable Output Rules

- Preserve original dialogue and inner monologue words exactly.
- Long dialogue cannot finish in one static picture; cut through speaker, listener, reactions, environment, or prop details.
- Every shot must keep three-dimensional space continuity unless an extreme action scene explicitly justifies disruption.
- Character actions must obey anatomy, ergonomics, and action logic.
- If a hit, collision, spell impact, or shock occurs, include visible feedback such as cloth movement, vibration, dust, sparks, recoil, or body balance changes.
- Describe visible images, not abstract literary interpretation.
- Include micro-expressions and small actions for characters when visible.
- Do not use `同上`, `同前`, or other omissions. Repeat required details fully.
- Do not add subtitles, watermark, or background music unless the user explicitly asks.

## Heavy Mecha Memory

For heavy mecha, Pacific-rim-scale robots, rain-night armor texture, sea-base launch shots, or female mechanical prosthetic battle scenes, load [references/advanced_cinema_lighting_camera.md](references/advanced_cinema_lighting_camera.md) and the local rule file `视频教学记忆库/03_风格规则/环太平洋机甲质感学习沉淀规则_20260515.md`.

For Image2 prompts that must avoid star-like speckles, grain, broken lines, noisy rain, noisy water, or noisy monster skin, also load `视频教学记忆库/03_风格规则/Image2无颗粒无星点写实提示词规则_20260515.md`.

## Xianxia Spell And Fight FX Memory

For xianxia ultimate skills, spell formations, sword energy, demonic flame, ice/fire/thunder/wind effects, Dunhuang/lotus/wing motifs, close combat, wuxia group fights, giant-threat pressure battles, or Seedance 2.0 action prompts, load [references/advanced_cinema_lighting_camera.md](references/advanced_cinema_lighting_camera.md) and the local rule file `视频教学记忆库/03_风格规则/仙侠法术打斗特效综合沉淀规则_20260518.md`.

Core rule: spell effects must be triggered by visible character action, form readable energy shapes, cast motivated light, reveal smoke/dust/water/air layers, create physical feedback, and land on a clear edit point. Fighting must include weight preparation, attack path, contact point, victim reaction, environmental feedback, and next-shot continuity.
