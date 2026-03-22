# BirdSafe

[English](./README.md) | 简体中文 | [繁體中文](./README.zh-TW.md)

![BirdSafe](./assets/logo.svg)

一款本地优先的 Chrome 浏览器扩展，用于备份和管理你的 Twitter/X 书签与喜欢。

BirdSafe 通过拦截 Twitter 原生 API 响应来捕获你收藏的内容，包括书签、喜欢、推文串和媒体，并全部存储在你可控的本地 IndexedDB 数据库中。除非你主动启用云端功能，否则数据不会离开你的浏览器。

## 下载

- 最新版本：[GitHub Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases)
- 当前安装包：[BirdSafe-extension-v2026.03.22.zip](https://github.com/duyananbryce/birdsafe-extension-releases/releases/download/v2026.03.22/BirdSafe-extension-v2026.03.22.zip)

## 安装

1. 从 [Releases](https://github.com/duyananbryce/birdsafe-extension-releases/releases) 下载最新 `BirdSafe-extension-*.zip`
2. 解压到本地
3. 打开 `chrome://extensions`
4. 启用“开发者模式”
5. 点击“加载已解压的扩展程序”
6. 选择解压后的 `dist` 文件夹

## 功能特性

### 核心能力

- 本地优先存储，基于 IndexedDB / Dexie.js
- 拦截 Twitter/X GraphQL 响应，捕获书签、喜欢、推文串与媒体
- 智能增量同步与深度同步模式
- 静默补全长推文、上下文、资料与缩略图
- 频率感知请求队列，遇到 429 自动冷却

### 浏览与整理

- 瀑布流、表格、图库三种视图
- 全文搜索、高级筛选、文件夹、星标、归档、批量操作
- 随机模式重新发现旧收藏
- 推文详情弹窗支持全文、媒体预览和手动刷新

![浏览](./assets/view-waterfall.png)

### 仪表盘

- 总收藏、书签、喜欢、作者等统计卡片
- 活跃热力图
- 趋势图
- 作者榜单与一键过滤

![仪表盘](./assets/feature-dashboard.png)

### 账号监控

- 采集任意 `@handle` 或公开主页时间线
- 清理回复噪音
- 按账号导出 JSON / CSV / Excel

### 云端功能

需要登录后使用。

- 加密云端备份
- 媒体镜像到 Cloudflare R2
- Notion 同步，支持校验、续传、重试和长内容拆分

![云备份](./assets/auto-backup.png)
![同步](./assets/feature-sync.png)

## 隐私与安全

- 本地优先设计，未启用云端功能时数据不会上传
- `ct0` 与 `auth_token` 仅用于本地请求组装
- 仅申请实际使用的最小权限
- 云端备份启用时，上传前先加密

## 说明

- 这是发布仓库，不是公开源码仓库
- 仓库主要用于提供安装包和版本更新
- 除非另行声明，否则保留所有权利
