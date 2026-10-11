# 出土文物比對室

上傳出土文物照片，由 Gemini 讀出照片上的字樣與器物特徵，再**只用研究資料庫裡的文獻**比對，整理出可能的品名、年代、出土地點與字樣解讀，每句都標出處。

網站：https://cherylhsu222.github.io/artifact-compare/

## 使用前需要

1. **資料庫密碼**：文獻全文已加密（`corpus.enc.json`），請向研究者索取密碼。
2. **自己的 Gemini API Key**：在 [Google AI Studio](https://aistudio.google.com/apikey) 建立。費用算在你自己的 Google 帳號；有 Google AI Pro 訂閱的人可以用每月附贈的 Google Cloud 額度支付。網站內「設定」有完整步驟。

API Key 與密碼都只存在你自己的瀏覽器。比對紀錄（標本櫃）也存在瀏覽器裡，可以匯出成檔案交換。

## 檔案

- `index.html`：整個網站（單一檔案）
- `corpus.enc.json`：加密後的文獻全文（AES-GCM，金鑰由密碼經 PBKDF2 產生）
