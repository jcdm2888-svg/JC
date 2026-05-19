# Seedance 2.0 视频提示词规则

All video prompts are for Seedance 2.0 unless the user says otherwise.

## Required Top-Level Format

【出现角色】
【场景】
【道具】
【画面色彩】（全局统一）
【画面描述】

## Shot Segment Format

For each shot:

`镜头 1 持续时间：X秒`

Each internal picture segment must follow:

`【景别|构图|光源光影|镜头运动|机位|景深】画面动作描述。【台词】... 配音指令：角色｜声源｜状态（身体/情绪/目标）｜语气特点（音量/语速/气息/尾音/情绪色彩）：...【音效】...`

End each shot or shot group with:

`镜头运动顺序：...→...→...`

## Dialogue and Inner Voice

- Do not alter any original dialogue, narration, or inner monologue.
- If the source marks OS, V.O., inner monologue, or psychological language, write: `当前角色的内心语言，不要张嘴说话`.
- If no dialogue or voice appears, write:
  `【台词】无 配音指令：无｜无｜状态（无）｜语气特点（无）：无`
- Do not add background music.
- Do not add subtitles.

## Motion Description

For every internal picture transition, start with the transition method, such as:

- 切镜
- 快速摇镜
- 慢推
- 跟拍
- 甩镜
- 拉镜
- 移镜
- 升降
- 环绕

Each segment must define both:

- camera movement
- subject action

Avoid abstract words. Write concrete visible actions and results.

