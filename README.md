# BirdSafe

English | [简体中文](./README.zh-CN.md) | [繁體中文](./README.zh-TW.md)

![BirdSafe](./assets/notion/logo.svg)

**A local-first Chrome extension for backing up and managing your Twitter/X bookmarks and likes.**

Your bookmarks and likes on Twitter/X can vanish at any time: deleted tweets, suspended accounts, or algorithm changes. BirdSafe keeps a permanent, searchable local copy that you fully control. No data leaves your browser unless you choose to enable cloud features.

[Website](https://birdsafe.nan0.in) · [Documentation](https://birdsafe.nan0.in/docs) · [Changelog](https://birdsafe.nan0.in/changelog)

---

## Features

### Sync & Backup

- **One-click sync**: Pull all your bookmarks and likes with a single click. Smart incremental sync picks up where you left off.
- **Deep sync**: Force a full historical pull when standard sync misses older content.
- **Background auto-complete**: Automatically patches missing full-text, reply context, thread chains, author profiles, and video thumbnails.
- **Rate-limit safe**: Built-in request pacing with automatic cooldown, so your account stays safe.

### Browse & Organize

- **Three view modes**: Waterfall, table, and gallery with adaptive column layout.
- **Full-text search**: Instant local keyword search across tweet text and author names.
- **Advanced filters**: Filter by media type, date range, and source (`bookmark` / `like`).
- **Folders, stars, archive**: Organize content into custom folders, star important items, or archive what you do not need right now.
- **Batch operations**: Multi-select for bulk move, archive, or folder assignment.
- **Random mode**: Resurface forgotten saves with a stable-seed shuffle.
- **Tweet detail view**: Full-text view, inline video playback, image lightbox, and thread chain visualization.

![Browse](./assets/notion/browse.png)

### Dashboard

- **Stats cards**: Total saves, bookmarks, likes, and linked authors at a glance.
- **Activity heatmap**: Year-by-year contribution-style heatmap.
- **Trend chart**: `7 / 14 / 30-day` new-content trend line.
- **Top authors**: Leaderboard with one-click filter to their content.

![Dashboard](./assets/notion/dashboard.png)

### Cloud Features (Optional, requires login)

- **Encrypted cloud backup**: Manual or automatic backup with version history for point-in-time restore.
- **Real-time media mirroring**: Cached images and videos are uploaded to the cloud, so originals survive even if deleted on Twitter.
- **Notion sync**: Sync your archive to a Notion database with field validation, checkpoint resume, and automatic content splitting.

![Cloud Backup](./assets/notion/cloud-backup.png)
![Notion Sync](./assets/notion/notion-sync.png)

---

## Getting Started

1. Install BirdSafe from the [Chrome Web Store](#) (coming soon).
2. Make sure you are logged into [x.com](https://x.com) in the same browser.
3. Click the BirdSafe icon in the toolbar to open the panel.
4. Hit **Sync** to start pulling your bookmarks and likes.

That's it. Your data is now stored locally in your browser with no account required for core features.

---

## Privacy & Security

![Privacy](./assets/notion/privacy.png)

- **Local-first by design.** All content is stored in your browser. Nothing is uploaded unless you enable cloud features.
- **Your credentials stay local.** Authentication cookies are used exclusively for assembling local API requests. They are never sent to any third-party server.
- **Minimal permissions.** The extension only requests the permissions it actively uses. No broad host access beyond `x.com` / `twitter.com`.
- **Cloud encryption.** When cloud backup is enabled, data is encrypted before upload.

For more details, see our [Privacy Policy](https://birdsafe.nan0.in/privacy), [Terms of Service](https://birdsafe.nan0.in/terms), and [Security Audit](https://birdsafe.nan0.in/security-audit).

---

## Plans

| | **Free** | **Pro** |
| --- | --- | --- |
| Local archive | Up to 1,500 tweets | Unlimited |
| Search & filter | Basic | Full |
| View modes | Waterfall, table, gallery | Waterfall, table, gallery |
| Export | Markdown / JSON | Markdown / JSON |
| Encrypted cloud backup | - | 1 GB |
| Notion sync | - | Included |
| Local media cache | - | Full HD originals |

[View full pricing details](https://birdsafe.nan0.in/#pricing)

---

## Links

- [Official Website](https://birdsafe.nan0.in)
- [Documentation](https://birdsafe.nan0.in/docs)
- [Changelog](https://birdsafe.nan0.in/changelog)
- [Privacy Policy](https://birdsafe.nan0.in/privacy)
- [Terms of Service](https://birdsafe.nan0.in/terms)
- [Security Audit](https://birdsafe.nan0.in/security-audit)

---

## License

BirdSafe is proprietary software. All rights reserved. See [Terms of Service](https://birdsafe.nan0.in/terms) for usage terms.
