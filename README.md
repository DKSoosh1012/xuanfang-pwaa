# 選房 PWA

這是從原 Electron 專案抽出的網頁版本，保留房號抽選、模式切換、自訂房號分析與詳細分析彈窗。此資料夾可獨立部署，無須安裝 Electron 或 `node_modules`。

## 部署

將此資料夾中的應用檔案部署到支援 HTTPS 的靜態網站空間。Service Worker 與 iPhone 主畫面安裝功能需要 HTTPS；在本機開發時，`localhost` 也可使用。

## 加到 iPhone 主畫面

1. 在 iPhone 的 Safari 開啟部署網址。
2. 點選「分享」按鈕。
3. 選擇「加入主畫面」，再點「加入」。

從主畫面圖示開啟後，應用會以獨立視窗顯示；首次載入後，Service Worker 會快取頁面，供離線開啟。
