# BirdSafe

[English](./README.md) | 简体中文 | [繁體中文](./README.zh-TW.md)

![BirdSafe](./assets/notion/logo.svg)

**一款本地优先的 Chrome 浏览器扩展，用于备份和管理你的 Twitter/X 书签与喜欢。**

你在 Twitter/X 上的书签和喜欢随时可能消失，可能是因为博主删帖、账号被封或算法调整。BirdSafe 在你的浏览器中保留一份永久、可搜索的本地副本，完全由你掌控。除非你主动启用云端功能，否则数据不会离开你的浏览器。

[官网](https://birdsafe.nan0.in) · [使用文档](https://birdsafe.nan0.in/docs) · [更新日志](https://birdsafe.nan0.in/changelog)

---

## 功能特性

### 同步与备份

- **一键同步**：点击一次，拉取全部书签和喜欢。智能增量同步，断点续传。
- **深度同步**：常规同步遗漏较早内容时，可强制执行完整历史拉取。
- **后台自动补全**：自动修补缺失的长推文全文、回复上下文、推文串、作者资料和视频封面。
- **安全节流**：内置请求频控与自动冷却机制，保障账号安全。

### 浏览与整理

- **三种视图模式**：瀑布流、表格、图库，自适应列宽布局。
- **全文搜索**：按推文内容和作者名称即时本地检索。
- **高级筛选**：按媒体类型、时间范围、来源（书签 / 喜欢）过滤。
- **文件夹、星标、归档**：自定义文件夹整理内容，星标重要内容，归档暂不需要的内容。
- **批量操作**：多选后批量移动、归档或分配文件夹。
- **随机模式**：重新发现被遗忘的收藏。
- **推文详情弹窗**：全文查看、内嵌视频播放、图片灯箱、推文串可视化。

![瀑布流](./assets/notion/zh-waterfall.png)
![表格视图](./assets/notion/zh-table.png)
![画廊视图](./assets/notion/zh-gallery.png)

### 仪表盘

- **统计卡片**：总收藏数、书签数、喜欢数、关联作者数一目了然。
- **活跃热力图**：按年切换的贡献热力图。
- **趋势图**：7 / 14 / 30 天新增趋势折线图。
- **作者榜单**：排行榜，点击可直接按作者过滤内容。

![仪表盘](./assets/notion/zh-dashboard.png)

### 云端功能（可选，需登录）

- **加密云备份**：手动或自动备份，支持按版本恢复。
- **实时媒体镜像**：图片和视频异步上传至云端，即使原推被删除也能保留原始媒体。
- **Notion 同步**：同步到 Notion 数据库，支持字段校验、断点续传、长内容自动拆分。

![自动备份](./assets/notion/zh-auto-backup.png)

---

## 快速上手

1. 从 [Chrome Web Store](#)（即将上线）安装 BirdSafe。
2. 确保在同一浏览器中已登录 [x.com](https://x.com)。
3. 点击工具栏中的 BirdSafe 图标打开面板。
4. 点击 **同步** 开始拉取你的书签和喜欢。

就这么简单。数据存储在你的浏览器本地，核心功能无需注册账号。

---

## 隐私与安全

![自定义设置](./assets/notion/zh-settings.png)

- **本地优先设计。** 所有内容存储在浏览器中，除非你启用云端功能，否则不会上传任何数据。
- **凭据不外传。** 认证 Cookie 仅用于在本地组装 API 请求，绝不会发送到任何第三方服务器。
- **最小权限。** 扩展仅申请实际使用的权限，宿主权限仅限 `x.com` / `twitter.com`。
- **云端加密。** 启用云备份时，数据在上传前会进行加密。

详情请参阅 [隐私政策](https://birdsafe.nan0.in/privacy)、[服务条款](https://birdsafe.nan0.in/terms) 和 [安全审计](https://birdsafe.nan0.in/security-audit)。

---

## 版本方案

| | **免费版** | **Pro 版** |
| --- | --- | --- |
| 本地存档 | 最多 1,500 条 | 无限制 |
| 搜索与筛选 | 基础 | 完整 |
| 视图模式 | 瀑布流、表格、图库 | 瀑布流、表格、图库 |
| 导出 | Markdown / JSON | Markdown / JSON |
| 加密云备份 | - | 1 GB |
| Notion 同步 | - | 包含 |
| 本地媒体缓存 | - | 高清原图全量缓存 |

[查看完整定价方案](https://birdsafe.nan0.in/#pricing)

---

## 相关链接

- [官方网站](https://birdsafe.nan0.in)
- [使用文档](https://birdsafe.nan0.in/docs)
- [更新日志](https://birdsafe.nan0.in/changelog)
- [隐私政策](https://birdsafe.nan0.in/privacy)
- [服务条款](https://birdsafe.nan0.in/terms)
- [安全审计](https://birdsafe.nan0.in/security-audit)

---

## 许可证

BirdSafe 为专有软件，保留所有权利。使用条款详见 [服务条款](https://birdsafe.nan0.in/terms)。
