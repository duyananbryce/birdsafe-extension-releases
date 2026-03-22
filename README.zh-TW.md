# BirdSafe

[English](./README.md) | [简体中文](./README.zh-CN.md) | 繁體中文

![BirdSafe](./assets/logo.svg)

一款本地優先的 Chrome 瀏覽器擴充功能，用於備份和管理你的 Twitter/X 書籤與喜歡。

BirdSafe 透過攔截 Twitter 原生 API 回應來擷取你收藏的內容，包括書籤、喜歡、推文串和媒體，並全部儲存在你可控的本地 IndexedDB 資料庫中。除非你主動啟用雲端功能，否則資料不會離開你的瀏覽器。

## 下載

- 最新版本：[GitHub Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases)
- 目前安裝包：[BirdSafe-extension-v2026.03.22.zip](https://github.com/duyananbryce/birdsafe-extension-releases/releases/download/v2026.03.22/BirdSafe-extension-v2026.03.22.zip)

## 安裝

1. 從 [Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases) 下載最新 `BirdSafe-extension-*.zip`
2. 解壓到本地
3. 開啟 `chrome://extensions`
4. 啟用「開發人員模式」
5. 點擊「載入未封裝項目」
6. 選擇解壓後的 `dist` 資料夾

## 功能特性

### 核心能力

- 本地優先儲存，基於 IndexedDB / Dexie.js
- 攔截 Twitter/X GraphQL 回應，擷取書籤、喜歡、推文串與媒體
- 智慧增量同步與深度同步模式
- 靜默補全長推文、上下文、資料與縮圖
- 頻率感知請求佇列，遇到 429 自動冷卻

### 瀏覽與整理

- 瀑布流、表格、圖庫三種檢視
- 全文搜尋、進階篩選、資料夾、星標、封存、批次操作
- 隨機模式重新發現舊收藏
- 推文詳情彈窗支援全文、媒體預覽和手動重新整理

![瀏覽](./assets/view-waterfall.png)

### 儀表板

- 總收藏、書籤、喜歡、作者等統計卡片
- 活躍熱力圖
- 趨勢圖
- 作者榜單與一鍵過濾

![儀表板](./assets/feature-dashboard.png)

### 帳號監控

- 擷取任意 `@handle` 或公開個人頁時間線
- 清理回覆雜訊
- 依帳號匯出 JSON / CSV / Excel

### 雲端功能

需要登入後使用。

- 加密雲端備份
- 媒體鏡像到 Cloudflare R2
- Notion 同步，支援校驗、續傳、重試和長內容拆分

![雲端備份](./assets/auto-backup.png)
![同步](./assets/feature-sync.png)

## 隱私與安全

- 本地優先設計，未啟用雲端功能時資料不會上傳
- `ct0` 與 `auth_token` 僅用於本地請求組裝
- 僅申請實際使用的最小權限
- 雲端備份啟用時，上傳前先加密

## 說明

- 這是發布倉庫，不是公開原始碼倉庫
- 倉庫主要用於提供安裝包和版本更新
- 除非另行聲明，否則保留所有權利
