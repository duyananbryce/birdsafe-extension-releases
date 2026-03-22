# BirdSafe

English | [简体中文](#简体中文) | [繁體中文](#繁體中文)

![BirdSafe](https://prod-files-secure.s3.us-west-2.amazonaws.com/a87fb0df-84b0-4f94-84c7-07029748c235/6e6e8ebf-f1f1-4ead-983a-490cd3c7552c/Frame_1.svg)

A local-first Chrome extension for backing up and managing your Twitter/X bookmarks and likes.

BirdSafe intercepts Twitter's native API responses to capture your saved content, including bookmarks, likes, threads, and media, then stores everything in a local IndexedDB database that you control. No data leaves your browser unless you explicitly enable cloud features.

## Download

- Latest release: [GitHub Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases)
- Current package: [BirdSafe-extension-v2026.03.22.zip](https://github.com/duyananbryce/birdsafe-extension-releases/releases/download/v2026.03.22/BirdSafe-extension-v2026.03.22.zip)

## Install

1. Download the latest `BirdSafe-extension-*.zip` package from [Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases).
2. Unzip it locally.
3. Open `chrome://extensions` in a Chromium-based browser.
4. Enable `Developer mode`.
5. Click `Load unpacked`.
6. Select the extracted `dist` folder.

## Features

### Core

- Local-first storage with IndexedDB via Dexie.js
- Network interception of Twitter/X GraphQL responses
- Smart incremental sync to reduce duplicate fetches
- Deep sync mode for historical backfill
- Silent backfill for long text, thread context, profiles, and thumbnails
- Rate-limit aware request queue with automatic cooldown on HTTP 429

### Browse and Organize

- Waterfall, table, and gallery view modes
- Full-text local search across tweet text and author names
- Advanced filters by media type, date range, and source
- Folders, stars, and archive workflows
- Batch operations for move, archive, and folder assignment
- Random mode for resurfacing older saves
- Tweet detail modal with full text, media preview, and manual refresh

![Browse](https://prod-files-secure.s3.us-west-2.amazonaws.com/a87fb0df-84b0-4f94-84c7-07029748c235/0ec847a4-dbba-40d0-b0bc-aff20e7fa805/HapiGo_2026-03-22_12-18-39.png)

### Dashboard

- Stats cards for total saves, bookmarks, likes, and linked authors
- Activity heatmap
- Trend chart for recent save activity
- Top authors leaderboard with one-click filtering

![Dashboard](https://prod-files-secure.s3.us-west-2.amazonaws.com/a87fb0df-84b0-4f94-84c7-07029748c235/f6f75308-73af-431f-8b99-b817a6d73cfb/HapiGo_2026-03-22_12-18-29.png)

### Account Monitor

- Public timeline capture for any `@handle` or profile URL
- Noise cleaning for reply-thread-heavy timelines
- Per-account export to JSON, CSV, and Excel

### Cloud Features

Optional cloud features require login.

- Encrypted cloud backup with restore points
- Real-time media mirroring to Cloudflare R2
- Notion sync with validation, resume checkpoints, retries, and long-content splitting

![Cloud Backup](https://prod-files-secure.s3.us-west-2.amazonaws.com/a87fb0df-84b0-4f94-84c7-07029748c235/7dd7b062-e87c-42e9-b643-1cf5679d3547/HapiGo_2026-03-22_12-18-05.png)
![Notion Sync](https://prod-files-secure.s3.us-west-2.amazonaws.com/a87fb0df-84b0-4f94-84c7-07029748c235/c5a626b3-826c-4729-b524-f3bebb03243e/HapiGo_2026-03-22_12-18-14.png)

## Privacy and Security

![Privacy](https://prod-files-secure.s3.us-west-2.amazonaws.com/a87fb0df-84b0-4f94-84c7-07029748c235/25ef264e-94a2-469e-8a9d-e409dda6df75/HapiGo_2026-03-22_12-17-56.png)

- Local-first by design: tweet content, media cache, and metadata stay in the browser unless cloud features are enabled
- Credentials stay local: `ct0` and `auth_token` cookies are used only for local request assembly
- Minimal permissions: the extension only requests permissions it actively uses
- Cloud encryption: cloud backup data is encrypted before upload

## Notes

- This is a release distribution repository, not a public source repository.
- Release assets are provided for installation and update delivery.
- All rights reserved unless explicitly stated otherwise.

---

## 简体中文

<details>
<summary>展开简体中文说明</summary>

### 简介

一款本地优先的 Chrome 浏览器扩展，用于备份和管理你的 Twitter/X 书签与喜欢。

BirdSafe 通过拦截 Twitter 原生 API 响应来捕获你收藏的内容，包括书签、喜欢、推文串和媒体，并全部存储在你可控的本地 IndexedDB 数据库中。除非你主动启用云端功能，否则数据不会离开你的浏览器。

### 下载与安装

1. 前往 [Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases) 下载最新 `BirdSafe-extension-*.zip`
2. 解压到本地
3. 打开 `chrome://extensions`
4. 启用“开发者模式”
5. 点击“加载已解压的扩展程序”
6. 选择解压后的 `dist` 文件夹

### 功能特性

- 本地优先存储，基于 IndexedDB / Dexie.js
- 拦截 Twitter/X GraphQL 响应，捕获书签、喜欢、推文串与媒体
- 智能增量同步与深度同步模式
- 静默补全长推文、上下文、资料与缩略图
- 瀑布流、表格、图库三种视图
- 全文搜索、高级筛选、文件夹、星标、归档、批量操作
- 仪表盘统计、热力图、趋势图、作者榜单
- 账号监控、导出 JSON / CSV / Excel
- 可选云端功能：加密备份、媒体镜像、Notion 同步

### 隐私与安全

- 本地优先设计，未启用云端功能时数据不会上传
- `ct0` 与 `auth_token` 仅用于本地请求组装
- 仅申请实际使用的最小权限
- 云端备份启用时，上传前先加密

</details>

## 繁體中文

<details>
<summary>展開繁體中文說明</summary>

### 簡介

一款本地優先的 Chrome 瀏覽器擴充功能，用於備份和管理你的 Twitter/X 書籤與喜歡。

BirdSafe 透過攔截 Twitter 原生 API 回應來擷取你收藏的內容，包括書籤、喜歡、推文串和媒體，並全部儲存在你可控的本地 IndexedDB 資料庫中。除非你主動啟用雲端功能，否則資料不會離開你的瀏覽器。

### 下載與安裝

1. 前往 [Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases) 下載最新 `BirdSafe-extension-*.zip`
2. 解壓到本地
3. 開啟 `chrome://extensions`
4. 啟用「開發人員模式」
5. 點擊「載入未封裝項目」
6. 選擇解壓後的 `dist` 資料夾

### 功能特性

- 本地優先儲存，基於 IndexedDB / Dexie.js
- 攔截 Twitter/X GraphQL 回應，擷取書籤、喜歡、推文串與媒體
- 智慧增量同步與深度同步模式
- 靜默補全長推文、上下文、資料與縮圖
- 瀑布流、表格、圖庫三種檢視
- 全文搜尋、進階篩選、資料夾、星標、封存、批次操作
- 儀表板統計、熱力圖、趨勢圖、作者榜單
- 帳號監控、匯出 JSON / CSV / Excel
- 可選雲端功能：加密備份、媒體鏡像、Notion 同步

### 隱私與安全

- 本地優先設計，未啟用雲端功能時資料不會上傳
- `ct0` 與 `auth_token` 僅用於本地請求組裝
- 僅申請實際使用的最小權限
- 雲端備份啟用時，上傳前先加密

</details>
