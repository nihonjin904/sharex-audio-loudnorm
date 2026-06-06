# 🎙️ ShareX Audio Loudnorm & Watcher

此專案是專門為 **ShareX 螢幕錄影** 後置處理設計的自動化音訊響度優化與監控工具。

---

## 📖 背景與原理

在使用 ShareX 錄製遊戲、教學或會議影片時，常常會遇到錄製音量過小、或音量起伏過大的問題。

本工具提供以下自動化音訊處理解決方案：
- **Bilibili 自動響度標準化**：調用 FFmpeg 的 `loudnorm` 與 `dynaudnorm` 濾鏡，自動將錄製好的 MP4/MKV 影片音軌進行符合 Bilibili / YouTube 響度標準的無損增益優化。
- **自動化檔案監聽（Watcher）**：透過 PowerShell 背景檔案監控服務，在 ShareX 完成錄製並生成影片的瞬間，自動偵測、觸發音訊優化，並自動將產出的標準化影片整理至指定資料夾。

---

## 🔒 程式碼保護說明

為了保障核心自動化邏輯的安全性，本專案的實體代碼已進行 **AES-256 高強度加密保護**，僅開放 `README.md` 架構設計展示。

- **解密密碼**：如果您是受邀評估作品集的朋友、面試官，或者在解壓時需要密碼，請直接聯繫作者取得授權密碼。
- **密碼遺失處理**：密碼已固化儲存在本地設定中，如果您遺失了密碼，請隨時聯繫作者索取。

---

## 📥 直達下載與安裝

你可以直接點選下方連結下載已加密打包的執行工具：

👉 [**點我下載 ShareX Audio Loudnorm Tool (ZIP)**](https://github.com/nihonjin904/sharex-audio-loudnorm/raw/master/sharex_audio_loudnorm_release.zip)

### 使用方法：
1. 下載後使用解密密碼解壓。
2. 依據需求配置 `sharex-watcher-v2.ps1` 內部的 ShareX 儲存路徑。
3. 執行 Watcher，即可開啟全自動的背景錄製響度優化流程。
