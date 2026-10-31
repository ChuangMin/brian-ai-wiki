# 成本與取捨

[回首頁](../README.md)

token 成本、指令輸出壓縮、agent 與傳統工具的成本對比

### [TokenEconomizer](https://github.com/microsoft/TokenEconomizer)

用過往經驗降低 agent token 成本的研究工具

![TokenEconomizer 的 GitHub 預覽](https://opengraph.githubassets.com/1/microsoft/TokenEconomizer)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 1,349 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

微軟研究院用過去經驗降低 agent 成本，SWE-Bench 成本降 18–31%（README 自述）

### [Claude Code vs Blender 成本梗](https://www.facebook.com/reel/1867596277567322)

用鸚鵡螺動畫諷刺 agent 生 3D 的 token 成本

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫 | — | [影片 2](https://www.facebook.com/reel/1867596277567322) |

同一段機械鸚鵡螺 3D 動畫，Claude Code 計數器跳到 512 美元，Blender 只要 14 美元，諷刺用 agent 生複雜動畫的 token 成本

### [Claude Code vs Blender：機械變色龍](https://www.facebook.com/reel/1413855857399181)

同系列成本對比動畫，主角換成機械變色龍

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫 | — | [影片 8](https://www.facebook.com/reel/1413855857399181) |

同影片 2 的對戰版型（左 Claude Code、右 Blender，金額計數器 512 美元 vs 14 美元），主角換成機械變色龍：雙眼各自轉動、沿樹枝走六步、伸出伸縮舌頭、鱗片波浪變色。底部附完整 prompt，作者 @marlenuii

### Claude Code vs Blender：ORBITAL X-02 火箭

同系列成本對比動畫，主角換成重型火箭

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫 | — | 截圖（DeepRepo.ai） |

同 @marlenuii 那系列對戰版型：重型火箭（陶瓷白燃料槽、雙助推器、14 個噴嘴、整流罩打開放出金箔衛星與太陽能板、分節再組回）左 Claude Code 184.70 美元、右 Blender 9.65 美元，約 19 倍。文案主張「AI 定義概念與結構、程式碼負責重複、Blender 負責執行」；畫面下方俄文註明金額是為影片設定的，不是實測成本

### [RTK（Rust Token Killer）](https://github.com/rtk-ai/rtk)

先壓縮指令輸出再交給 agent，省下大量 token 的 CLI 代理

![RTK（Rust Token Killer） 的 GitHub 預覽](https://opengraph.githubassets.com/1/rtk-ai/rtk)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 85.1k | Brian 推薦清單 2026-10-31 |

rtk-ai 的單一 Rust 執行檔：攔截 agent 執行的 shell 指令（ls、grep、git status／diff／log、cargo test、pytest、docker ps 等 100+ 種），把輸出壓縮後才進 LLM 上下文，例如測試只留失敗、git log 只留雜湊與標題，宣稱常見開發指令省 60–90% token、額外延遲 < 10 ms。README 自己說明省的是 bash 輸出，不等於帳單同比例下降，token 數是 bytes/4 估算。安裝：`brew install rtk`（或官方 install.sh），再 `rtk init -g` 接上 Claude Code（`--codex`、`--agent cursor` 等）；`rtk gain` 看節省統計。授權：GitHub 標 Apache-2.0，README 寫完整版是 Apache-2.0＋BUSL-1.1，純 Apache 版叫 rtk-oss；crates.io 上另有同名的不相干套件。面試：成本治理要量化，先量測哪些上下文是雜訊，再用工具過濾，同時保留失敗資訊不影響品質
