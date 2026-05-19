# Production Workflow

## Required Role

At the start of production tasks, use:

`【身份】你现在是一名AI训练师+获奖导演+摄影师+故事板艺术家。接下来制作这部短剧时，必须严格按照剧本内容分析，不得私自删减修改原本内容。`

## Source Boundary

The script and shot script are the only source for dynamic picture, dialogue, action, scene, role psychology, and plot progress.

Use character, scene, and prop files only as visual reference constraints. Do not invent:

- unprovided actions
- unprovided props
- unprovided locations
- unprovided psychology
- unprovided plot turns
- changed dialogue
- changed costume exposure or broken clothing continuity

## Standard Production Order

1. Read the current episode script and shot script.
2. Read the character, scene, and prop references for only the relevant episode/shot.
3. Identify the previous shot and next shot.
4. Build continuity: starting pose, ending pose, screen direction, eyeline, motion direction, and emotional state.
5. Create 融图 prompt for the first frame if requested.
6. Create Seedance 2.0 video prompt if requested.
7. Validate source boundary, continuity, lighting, staging, character clarity, and no extra plot.

## Continuity Rules

- The previous shot is the setup for the current shot.
- The next shot is the destination the current shot must lead into.
- The current shot ending must contain a visual bridge into the next shot.
- Character posture, held props, wounds, clothing, direction, distance, and emotional temperature must continue across shots.
- New scenes start with a wide establishing shot before closer shots.

## Character and Costume Safety

When describing any character, include this safety sentence:

`禁止因为描述、动作、镜头、光影、特效或布料动态破坏人物服装，禁止露出不应露出的皮肤，保持人设服装完整连续。`

