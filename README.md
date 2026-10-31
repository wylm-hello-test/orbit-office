# ORBIT · 星球办公室 / ORBIT · Planet Office

> 一个完全虚构、离线可交互的 2.5D 星球办公室 DEMO。不是实时监控，不是 Three.js / WebGL，也不是任何真实团队的监控屏。
>
> A fully fictional, offline, interactive 2.5D planet-office DEMO. It is not real-time monitoring, not Three.js / WebGL, and not a monitor for any real team.

---

## 中文介绍

### 这是什么

ORBIT 把一间“办公室”画成一片星空：行星是空间，席位是巡航舰、测绘卫星和中继信标。你可以点选星体和角色、搜索席位、在手机上打开底部抽屉看详情，还可以播放一段 60 秒的 DEMO 故事。

- **版本**：v1.1.2-office
- **形态**：2.5D，原生 HTML / CSS / JavaScript，单文件自包含
- **内容**：43 个虚构席位、8 颗星体、3 名故事演员
- **故事**：60 秒，需点击播放；支持播放 / 暂停 / 重置，循环是显式选项，页面隐藏时自动暂停
- **依赖**：生产运行零第三方依赖，零构建依赖，无后端、无数据库、无环境变量、无令牌、无网络请求

### 怎么看

最简单：直接在浏览器里打开 `index.html`。

也可以用本地静态服务预览（仅本机，不是公网）：

```bash
python3 -m http.server 8000 --bind 127.0.0.1 --directory .
```

然后访问 `http://127.0.0.1:8000/`。

### 这个库里有什么

| 文件 | 说明 |
| --- | --- |
| `index.html` | 唯一可公开的 DEMO 本体，33,887 字节，SHA256 见下 |
| `manifest.json` | 版本与隐私声明 |
| `README.md` | 本介绍（中英文） |

`index.html` 的 SHA256：

```
665bcb00da6034867e78e5b1b7baf6096b464b398ca02f0b3eebe650909ce159
```

### 边界与声明（请先读这段）

- **全部虚构**：角色、代号、席位、故事、状态全部是 DEMO 编造的，不对应任何真实的人、席位或任务。
- **不是实时数据**：页面里的数字、状态、求助、完成等都是 DEMO 剧情，不代表任何真实系统的未读、待回、逾期或完成情况。
- **不写回任何东西**：点选、搜索、播放故事都只改本页显示，不会修改任何真实数据、状态或任务。
- **故意没有放进来的东西**：内部历史数据、真实快照、测试、截图证据、回滚旧版和开发脚本不在这个公开库里。按项目本身的公开边界，只有 `dist/`（也就是这里的 `index.html` + `manifest.json`）可以公开，根目录和内部历史数据不得公开。

### 适合谁

适合想看“星球办公室”这种视觉形式、想直接打开一个单文件 DEMO 体验交互的人。不适合把它当成监控、考勤、任务看板或任何真实运营工具来用。

---

## English Introduction

### What is this

ORBIT turns an "office" into a starfield: planets are spaces, and seats are cruising ships, survey satellites, and relay beacons. You can click planets and characters, search seats, open a bottom drawer for details on mobile, and play a 60-second DEMO story.

- **Version**: v1.1.2-office
- **Form**: 2.5D, vanilla HTML / CSS / JavaScript, a single self-contained file
- **Content**: 43 fictional seats, 8 planets, 3 story characters
- **Story**: 60 seconds, click to play; supports play / pause / reset, looping is an explicit option, and playback pauses automatically when the page is hidden
- **Dependencies**: zero third-party dependencies at runtime, zero build dependencies, no backend, no database, no environment variables, no tokens, no network requests

### How to view it

Simplest: open `index.html` directly in a browser.

Or preview it with a local static server (localhost only, not a public URL):

```bash
python3 -m http.server 8000 --bind 127.0.0.1 --directory .
```

Then visit `http://127.0.0.1:8000/`.

### What is in this repository

| File | Description |
| --- | --- |
| `index.html` | The only publicly releasable DEMO itself, 33,887 bytes, SHA256 below |
| `manifest.json` | Version and privacy statement |
| `README.md` | This introduction, in Chinese and English |

SHA256 of `index.html`:

```
665bcb00da6034867e78e5b1b7baf6096b464b398ca02f0b3eebe650909ce159
```

### Boundaries and disclaimers (please read this first)

- **Fully fictional**: every character, codename, seat, story, and status is invented for the DEMO. Nothing here corresponds to a real person, seat, or task.
- **Not real-time data**: numbers, statuses, help requests, and completions on the page are DEMO plot, not unread counts, pending replies, overdue items, or completions from any real system.
- **Nothing is written back**: clicking, searching, and playing the story only change what this page shows. They do not modify any real data, status, or task.
- **Deliberately not included**: internal history data, real snapshots, tests, evidence screenshots, rollback versions, and development scripts are not in this public repository. Under the project's own public boundary, only `dist/` — here, `index.html` plus `manifest.json` — may be published; the repository root and internal history data must not be published.

### Who is it for

For anyone who wants to see the "planet office" visual form and try an interactive single-file DEMO right away. It is not a monitor, attendance tool, task board, or any real operations tool.
