<div align="center">

<img src="docs/poster.png" alt="星露谷食堂 Stardew Canteen" width="100%">

# 星露谷食堂 · Stardew Canteen

**张嘴就能吃。两个人，一个摄像头，三十秒，看谁更能吃。**<br>
*Open your mouth to eat. Two players, one webcam, thirty seconds.*

[![在线试玩 Play Now](https://img.shields.io/badge/在线试玩-Play_Now-e8a33d?style=for-the-badge)](https://SimoneScoop.github.io/stardew-canteen/)
[![Deploy](https://github.com/SimoneScoop/stardew-canteen/actions/workflows/deploy.yml/badge.svg)](https://github.com/SimoneScoop/stardew-canteen/actions/workflows/deploy.yml)
[![License: MIT](https://img.shields.io/badge/code-MIT-blue.svg)](LICENSE)

[中文](#中文) | [English](#english)

<img src="docs/demo.gif" alt="游戏演示 Gameplay demo" width="720">

<sub>《星露谷物语》非官方同人作品 / Unofficial fan game, not affiliated with ConcernedApe</sub>

</div>

---

## 中文

### 这是什么

一款用脸玩的双人对战小游戏。美食和怪物从天而降，你左右移动脑袋去接，**张开嘴就能吃**。吃到星之果实和粉红蛋糕加分，误吞史莱姆和樱桃炸弹扣分。三十秒后，得分高的人获胜。

不用手柄，不用键盘，也不用注册账号。打开网页，允许摄像头，喊上旁边的人就能开局。

### 玩法

| 操作 | 说明 |
|---|---|
| **移动** | 左右移动你的脸，头像会跟着走 |
| **吃** | 张嘴。只有张着嘴碰到的东西才会被吃掉 |
| **双人** | 两人并排坐在镜头前，左边是 1P，右边是 2P |
| **时长** | 每局 30 秒，中途可以暂停 |

**掉落物**

- 🍰 **14 种美食**，+25 到 +500 分。星之果实最值钱，五彩碎片和魔法糖冰棍紧随其后
- 🟢 **18 种怪物**，−30 到 −150 分。史莱姆、蝙蝠、岩石蟹、影子野蛮人……闭嘴躲开
- 💣 **樱桃炸弹**，−200 分，千万别吃

**三档难度**

| 难度 | 节奏 |
|---|---|
| 拾荒者 | 悠闲的采集时光，下落慢 |
| 农场主 | 标准节奏 |
| 齐先生的挑战 | 极限反应测试，下落快 |

**四种餐次**：早饭、午饭、晚饭、下午茶的掉落密度各不相同。午饭最密集，适合抢食；下午茶最稀疏，适合慢慢挑。

每局结束后，爷爷的幽灵会根据你的表现留下一句评语，当次的对战结果会记入"社区中心记录"。

### 开玩之前

- **设备**：带摄像头的电脑，推荐使用新版 Chrome 或 Edge
- **光线**：脸要照亮，逆光会影响识别
- **位置**：两人都要完整出现在画面里，彼此别挡住
- **首次加载**：需要下载人脸识别模型（几 MB），请稍等几秒

### 隐私

人脸识别由 [MediaPipe](https://developers.google.com/mediapipe) 在**你的浏览器本地**完成。摄像头画面不会上传到任何服务器，本项目也没有后端。首次打开时，浏览器会从 Google 和 jsDelivr 的 CDN 下载识别模型与运行文件；游戏画面中的星露谷素材从 Stardew Valley Wiki 加载。

### 本地运行

需要 [Node.js](https://nodejs.org/) 18 或更高版本。

```bash
git clone https://github.com/SimoneScoop/stardew-canteen.git
cd stardew-canteen
npm install
npm run dev
```

打开 <http://localhost:3000> 即可。不需要任何 API Key。

> 摄像头只能在 `localhost` 或 HTTPS 页面下调用。用局域网 IP 在手机上访问开发服务器时，浏览器会拒绝开启摄像头。

### 部署自己的一份

1. Fork 本仓库
2. 进入仓库的 **Settings → Pages**，把 **Source** 设为 **GitHub Actions**
3. 推送任意提交到 `main` 分支，或在 **Actions** 页手动运行 *Deploy to GitHub Pages*
4. 部署完成后，访问 `https://<你的用户名>.github.io/stardew-canteen/`

### 技术栈

React 19、TypeScript、Vite、MediaPipe Face Landmarker、Canvas 2D、Web Audio API、Tailwind CSS

音效和背景音乐由 Web Audio API 实时合成，仓库里没有任何音频文件。

### 免责声明

本项目是《星露谷物语》（Stardew Valley）的**非官方粉丝同人作品**，仅供非商业的学习与娱乐用途，与 ConcernedApe LLC 无任何关联，也未获其认可。

游戏中出现的角色、物品、怪物名称及美术素材，权利均归 ConcernedApe LLC 所有。**本仓库不包含这些素材**，游戏运行时从 [Stardew Valley Wiki](https://stardewvalleywiki.com/) 在线加载。如权利人认为不妥，请通过 Issue 联系，我会及时处理。

喜欢星露谷的话，请[支持正版](https://www.stardewvalley.net/)。

### 协议

源代码以 [MIT](LICENSE) 协议开源。该协议不涵盖上述《星露谷物语》相关素材。

---

## English

### What is it

A two-player party game you play with your face. Food and monsters fall from the sky. Move your head to line up, then **open your mouth to eat**. Stardrops and Pink Cakes score points; swallow a Slime or a Cherry Bomb and you lose them. Highest score after thirty seconds wins.

No controller, no keyboard, no sign-up. Open the page, allow the camera, grab a friend.

### How to play

| Action | How |
|---|---|
| **Move** | Move your face left and right; your avatar follows |
| **Eat** | Open your mouth. Items only count if your mouth is open when you touch them |
| **Two players** | Sit side by side in front of the camera. Left is P1, right is P2 |
| **Length** | 30 seconds per round, with pause |

**What falls**

- 🍰 **14 foods**, +25 to +500. The Stardrop is worth the most
- 🟢 **18 monsters**, −30 to −150. Slimes, bats, rock crabs, shadow brutes… keep your mouth shut
- 💣 **Cherry Bomb**, −200. Do not eat

**Three difficulties**

| Difficulty | Pace |
|---|---|
| Forager (拾荒者) | Relaxed, slow drops |
| Farmer (农场主) | Standard |
| Mr. Qi's Challenge (齐先生的挑战) | Fast. A reflex test |

**Four meals**: Breakfast, Lunch, Dinner and Afternoon Tea each set a different drop density. Lunch is the busiest; Afternoon Tea is the calmest.

After each round, Grandpa's ghost comments on your performance, and the result is added to the session's match history.

### Before you play

- **Device**: a computer with a webcam; a recent Chrome or Edge is recommended
- **Lighting**: light your face from the front; backlight hurts tracking
- **Framing**: both players fully in frame, not blocking each other
- **First load**: the face model (a few MB) downloads on your first visit

### Privacy

Face tracking runs **locally in your browser** with [MediaPipe](https://developers.google.com/mediapipe). Camera frames never leave your device, and the project has no backend. On first load the browser fetches the model and runtime files from Google's and jsDelivr's CDNs; in-game Stardew Valley artwork is loaded from the Stardew Valley Wiki.

### Run locally

Requires [Node.js](https://nodejs.org/) 18+.

```bash
git clone https://github.com/SimoneScoop/stardew-canteen.git
cd stardew-canteen
npm install
npm run dev
```

Then open <http://localhost:3000>. No API key needed.

> Browsers only allow camera access on `localhost` or HTTPS, so opening the dev server from a phone via your LAN IP won't work.

### Deploy your own copy

1. Fork this repository
2. Go to **Settings → Pages** and set **Source** to **GitHub Actions**
3. Push to `main`, or run *Deploy to GitHub Pages* manually from the **Actions** tab
4. Visit `https://<your-username>.github.io/stardew-canteen/`

### Tech stack

React 19, TypeScript, Vite, MediaPipe Face Landmarker, Canvas 2D, Web Audio API, Tailwind CSS

All sound effects and music are synthesized live with the Web Audio API; the repo contains no audio files.

### Disclaimer

This is an **unofficial fan project** based on Stardew Valley, made for non-commercial learning and entertainment. It is not affiliated with or endorsed by ConcernedApe LLC.

All character, item and monster names and artwork belong to ConcernedApe LLC. **This repository contains none of those assets**; the game loads them at runtime from the [Stardew Valley Wiki](https://stardewvalleywiki.com/). If you are a rights holder and have concerns, please open an issue and I will respond promptly.

If you enjoy Stardew Valley, please [support the official game](https://www.stardewvalley.net/).

### License

Source code is released under the [MIT License](LICENSE). The license does not cover the Stardew Valley materials described above.
