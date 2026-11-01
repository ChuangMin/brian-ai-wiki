# 3D／動畫與 DCC

中文 | [English](../en/docs/dcc-animation.md)

[回首頁](../README.md)

Blender 等 DCC 外掛、運鏡、程序化動畫、遊戲生成

### [blender-skills](https://github.com/EL4CTEO/blender-skills)

讓 agent 操作 Blender 工作流程的 skill

![blender-skills 的 GitHub 預覽](https://opengraph.githubassets.com/1/EL4CTEO/blender-skills)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 598 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

給 agent 用的 Blender 工作流程 skill

### [rossark-motion-skill](https://github.com/rossark0/rossark-motion-skill)

把 SVG 轉成 60fps 動畫的 skill

![rossark-motion-skill 的 GitHub 預覽](https://opengraph.githubassets.com/1/rossark0/rossark-motion-skill)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 575 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

把 SVG 做成 60fps 動畫

### [Blender 魚群沿曲線游動](https://www.facebook.com/reel/1433262628273189)

用 Bezier 曲線路徑做出大量魚群游動動畫

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 4](https://www.facebook.com/reel/1433262628273189) |

一條 BezierCurve 當路徑，讓大量發光平面魚沿著曲線游，示範用路徑加物件實例化做出複雜群體動畫

![大量發光平面魚沿 Bezier 路徑游動並轉向俯衝，暖色加法混合發光；可用 Three.js InstancedMesh + CatmullRom 曲線取點 + additive blending 重現](../assets/gifs/v04-blender-fish-swarm-curve.gif)

大量發光平面魚沿 Bezier 路徑游動並轉向俯衝，暖色加法混合發光；可用 Three.js InstancedMesh + CatmullRom 曲線取點 + additive blending 重現

### [自動化垂直港口動畫](https://www.facebook.com/reel/1665373244995510)

3D 等角港口物流動畫，搭配同步儀表板

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 5](https://www.facebook.com/reel/1665373244995510) |

等角視角 3D 動態設計：15 個貨櫃經輸送帶、配重升降機、旋轉橋、蜘蛛吊臂跨三層運送，搭配即時儀表板（已出貨數、運送中、完成率、升降機高度）同步跳動；看起來是 Blender／C4D 渲染加後製，不是 AI 生成。作者 @marlenuii

![等角視角 3D 多層港口：貨櫃經輸送帶與升降機移動，上方儀表板數字（出貨數／完成率）同步遞增；可用 Three.js OrthographicCamera 等角 + GSAP 時間軸同步 DOM 數字](../assets/gifs/v05-isometric-port-dashboard.gif)

等角視角 3D 多層港口：貨櫃經輸送帶與升降機移動，上方儀表板數字（出貨數／完成率）同步遞增；可用 Three.js OrthographicCamera 等角 + GSAP 時間軸同步 DOM 數字

### [video-to-game](https://github.com/lovisdotio/video-to-game)

從影片設計稿自動生成可玩 Three.js 遊戲的 skill

![video-to-game 的 GitHub 預覽](https://opengraph.githubassets.com/1/lovisdotio/video-to-game)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 278 | [影片 6](https://www.facebook.com/reel/1118797844231418) |

OdinLovis 的 agent skill：先用影片模型生成遊戲畫面當設計稿，agent 逐格分析，再用 fal 生成圖片、3D 模型、音效，寫成單一 HTML 的 Three.js 遊戲，最後自己玩並錄下精彩片段驗收。31 款遊戲平均每款約 6 美元，MIT 授權

![AI 生成的 Three.js 遊戲實機畫面（第三人稱飛行／跑酷場景）與旁邊程式碼並排；參考低多邊形場景、相機跟隨與天空霧化](../assets/gifs/v06-video-to-game-threejs.gif)

AI 生成的 Three.js 遊戲實機畫面（第三人稱飛行／跑酷場景）與旁邊程式碼並排；參考低多邊形場景、相機跟隨與天空霧化

### [VirtuCamera：手機手持運鏡驅動 AI 動畫](https://virtucamera.com/)

用手機手持運鏡控制 3D 攝影機，再生成 AI 影片

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 10](https://www.facebook.com/reel/2599932377114150) |

手機 App 透過 Wi-Fi 連 Blender（也支援 Maya、Houdini、C4D、3ds Max、Nuke），把手機的移動即時變成 3D 攝影機動作，滑桿可即時推拉焦距；先用簡單 3D 角色手持拍好運鏡，再當控制層生成寫實 AI 影片，不用靠抽卡賭運鏡。App $19.99 買斷，Pro $9.99/月

![三段直式分屏：手機手持控制 Blender 攝影機 → 簡易 3D 角色鏡頭 → 生成的寫實 AI 影片，同一運鏡同步；參考同步分屏敘事版型](../assets/gifs/v10-virtucamera-phone-mocap.gif)

三段直式分屏：手機手持控制 Blender 攝影機 → 簡易 3D 角色鏡頭 → 生成的寫實 AI 影片，同一運鏡同步；參考同步分屏敘事版型

### [Spider Walker：多足生物程序化走路](https://github.com/iltaen/spider_walker)

自動產生多足生物走路動畫的 Blender 外掛

![Spider Walker：多足生物程序化走路 的 GitHub 預覽](https://opengraph.githubassets.com/1/iltaen/spider_walker)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 63 | [影片 11](https://www.facebook.com/reel/1442232340569116) |

免費 Blender 外掛（Blender 3.2）：設好骨架、中心骨與各腳 IK 控制器，只要移動身體，腳就會依步態順序自動跟上、預測前進方向，並用射線貼合不平地形；滿意後一鍵 bake 成關鍵影格。作者註明程式部分由 AI 撰寫重構；MIT。配樂：純演奏的 synthwave／賽博龐克電子樂，無法辨識曲名

![Blender 機械蜘蛛移動身體時各腳依步態順序 IK 自動抬腳落地、貼合地形；可用 Three.js CCDIKSolver 或 2D 兩節 IK + 步態相位重現](../assets/gifs/v11-spider-walker-procedural.gif)

Blender 機械蜘蛛移動身體時各腳依步態順序 IK 自動抬腳落地、貼合地形；可用 Three.js CCDIKSolver 或 2D 兩節 IK + 步態相位重現
