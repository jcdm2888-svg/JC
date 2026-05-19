# Douyin Creator Learning Map

## Source

- Creator page: `https://www.douyin.com/user/MS4wLjABAAAA7tSXpu5Pa3OrxsJ_I-OLy6TfTKxw13--Q08DN9eL2ro?from_tab_name=main&vid=7624791405625494794`
- Creator identified from page text: `And1`
- Method: webpage watching screenshots only; no video download, no unofficial download, no bypass.
- Latest verified batch: `20260515_111458`

## Storage

- Web screenshots: `D:\1AI工程文件\1样片\真人AI样片\CODEX测试\视频教学记忆库\06_网页观看测试\douyin_MS4wLjABAAAA7tSX_影视学习\20260515_111458`
- Analysis notes: `D:\1AI工程文件\1样片\真人AI样片\CODEX测试\视频教学记忆库\02_逐镜分析\douyin_MS4wLjABAAAA7tSX_影视学习\20260515_111458`
- Script: `D:\1AI工程文件\1样片\真人AI样片\CODEX测试\tools\douyin_creator_web_learning.py`

## Screening Result

Eighteen film-related videos were selected from the creator page. All selected playback pages were blocked by the Douyin login overlay during automated sampling, so this batch is a verified topic index and repeatable learning pipeline, not completed frame-level learning.

Selected topics:

1. `电影人之眼——构图和焦段对情绪的影响`
2. `电影布光：罗杰迪金斯在《007》开头的灯光设计拉片`
3. `电影人之眼——如何使镜头更有表现力`
4. `大师镜头：低成本拍大片的100个高级技巧 1 出场`
5. `大师镜头 2 追逐：低成本拍大片的100个高级技巧`
6. `电影布光的四个步骤：《使女的故事》`
7. `电影镜头介绍：ARRI SP`
8. `《艺伎回忆录》为什么是最好的电影摄影教科书`
9. `韦斯·安德森的六个电影构图技巧`
10. `韦斯·安德森的色彩美学`
11. `今敏的转场美学`
12. `从摄影角度看 MV《太阳之子》`
13. `《芳华》为什么这么美：美术概念`
14. `近几年摄影最优秀的电影：《诗人》`
15. `那些电影摄影：斯托拉罗《末代皇帝》`
16. `如何拍出电影质感的夜景画面`
17. `用反光板拍微电影`
18. `如何拍出电影质感的夜景`

## Resume Command

Run this after logging in through the visible Edge window:

```powershell
& "C:\Users\EDY\AppData\Local\Programs\Python\Python312\python.exe" "D:\1AI工程文件\1样片\真人AI样片\CODEX测试\tools\douyin_creator_web_learning.py" --url "https://www.douyin.com/user/MS4wLjABAAAA7tSXpu5Pa3OrxsJ_I-OLy6TfTKxw13--Q08DN9eL2ro?from_tab_name=main&vid=7624791405625494794" --headed --manual-login-wait 120 --scrolls 8 --max-selected 18 --samples 6 --interval 2
```

After a successful logged-in run, update `advanced_cinema_lighting_camera.md` with only non-redundant, executable rules extracted from actual video frames.

