# 實體 AI 與硬體

[回首頁](../README.md)

ESP32、機器人等實體裝置

### [esp32-iphone-agent](https://github.com/onehumanbeing/esp32-iphone-agent)

用 7 美元的 ESP32 讓 AI 操作實體 iPhone

![esp32-iphone-agent 的 GitHub 預覽](https://opengraph.githubassets.com/1/onehumanbeing/esp32-iphone-agent)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 4,120 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

用約 7 美元的 ESP32 讓 AI 操作實體 iPhone

### [Microduck：4 隻小雙足機器人聊天（Grok 儀表板）](https://github.com/pollen-robotics/microduck)

開源小型雙足機器人，影片儀表板是後製

![Microduck：4 隻小雙足機器人聊天（Grok 儀表板） 的 GitHub 預覽](https://opengraph.githubassets.com/1/pollen-robotics/microduck)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 後製包裝 | 13.2k | 截圖（DeepRepo.ai） |

機器人是真的：Pollen Robotics × Hugging Face 的 Microduck，25 cm／800 g、15 顆馬達，MuJoCo＋PPO 訓練的 RL 策略匯出 ONNX 上機，預購 $399；軟體 Apache-2.0（microduck_rl 的 3D 模型為 CC BY-NC-SA 4.0）。官方能力是走路、滑輪、撿東西、跌倒爬起，四種聲紋對話和「Grok Robot Brain Engine」數位分身儀表板查無出處，應是後製的視覺包裝。另有 apirrone 的 Open Duck Mini（4,605 星、Apache-2.0）外型相近，兩者關係待確認

### [Edge0：手機／筆電跑 35B MoE 模型（SSD 串流專家權重）](https://github.com/Edge0-AI/Edge0) ⚠️

不把整個模型載入記憶體，而是用到哪些專家權重才從 SSD 讀，讓 35B MoE 模型在約 3 GB 記憶體裡跑

![Edge0-AI/Edge0 的 GitHub 預覽](https://opengraph.githubassets.com/1/Edge0-AI/Edge0)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| ⚠️ 引流・可信度中高 | 8.8k | [影片 38](https://www.facebook.com/share/r/1CcD2Vgk2Y/) ⚠️ |

GitHunt 上傳的 38 秒影片，內容是捲動 README 加 AI 語音旁白，沒有實機示範；片尾說「Comment EDGE and I'll send you the repo link」導流。機制：SSD 專家卸載（記憶體峰值取決於當下啟用的專家，不是總參數量）；Prerouter（訓練過的預測頭先猜下一步路由，讓讀取和運算重疊，解碼速度最多 +59%）；Recover-LoRA（int4 基底加蒸餾 LoRA 轉接器，補回量化損失）。模型：Edge0-35B-A3B-preview（基於 Qwen3.6-35B-A3B）、Edge0-8B-A1B-preview。平台：Python／MLX、macOS、iOS、Android、Windows（Vulkan）。有 arXiv 論文 2609.18063。README 基準：35B 記憶體峰值約 2.9 GB，Mac mini M4 Pro 24 GB 上約 15–18 tok/s。Apache-2.0，2026-09-08 建立。可信度：中高，repo、論文與模型都是真的；但文案說 2.5 GB，和 README 基準的 2.9 GB 不一致，速度也取決於 SSD 讀取速度，旁白說「人形機器人公司在用」查無佐證。配樂：低音量的電子／ambient synth。無 GIF 片段（只是捲動 README）。面試：記憶體瓶頸可以用「串流 + 預測預取」解決，這是把系統設計的 cache／prefetch 思路搬到模型推論上
