# 融图提示词规则

融图 means creating the first-frame image for a video segment, not a process animation.

## Required Field Order

Use this format unless the user provides a stricter one:

【人物】
【人物关系】
【场景】
【时代背景】
【空间类型】
【空间尺度】
【道具】
【主体】
【主体层次】
【画面色彩】
【光源光影】
【材质质感】
【明暗层次】
【构图】
【人物神态】
【人物视线】
【人物面部身体打光效果】
【视觉重点】
【时间】
【天气】
【机位高度】
【视角设定】
【景深设定】
【镜头参数】
【前景】
【场景边界】
【氛围】
【景别】
【风格】
【人物动作】

## Field Rules

- Hide 【前景】 unless 【景别】 is 中景 or 近景.
- When used, foreground must be a valid element from the current scene, blurred, and not competing with the subject.
- 【画面色彩】 must define one dominant color and 2-3 auxiliary colors. Auxiliary colors cannot overpower the dominant color.
- 【光源光影】 must specify usable light types: main light, fill light, side light, rim light, back light, and how they land on face/body.
- Never use flat lighting. Build strong light-dark contrast around the subject and visual focus.
- Add: `主体人物的边缘锐利，要和背景明显拉开。`
- Main character face must be clear. Overall image clarity must be highest.
- In 【构图】, specify screen position, distance to lens, up/down/left/right, facing direction, body posture, micro-expression, and composition method.
- Main characters should not always stand centered. Use varied composition: center, thirds, symmetry, leading lines, frame, foreground, negative space, fill, triangle, golden spiral, overhead, tilted composition.
- People, props, troops, and scene elements should be staggered and natural, not neatly lined up unless the script requires formation.

## Character Expression

Do not write only "angry", "sad", or "nervous". Describe visible facial state:

- brows
- eyelids
- pupils/eyeline
- jaw
- lips
- breath
- shoulders/hands
- small movement

