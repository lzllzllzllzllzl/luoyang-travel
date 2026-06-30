# 洛阳旅行 · luoyang-travel

一个基于 GitHub Pages 的洛阳旅行指南项目，包含交互式地图、行程与交通指南、酒店选择指南，在线访问：

**https://lzllzllzllzllzl.github.io/luoyang-travel/**

---

## 项目简介

本项目用于记录与展示洛阳旅行的实用信息，覆盖：

- **洛阳交互地图**（`index.html`）：基于 Leaflet 的交互地图，展示景点、路线、图例等。
- **洛阳行程交通指南**（`洛阳行程交通指南.md`）：行程规划、交通方式等。
- **洛阳酒店选择指南**（`洛阳酒店选择指南.md`）：酒店区域、推荐理由等。

源码即网页，打开 `index.html` 即可本地预览，部署到 GitHub Pages 后即可在线访问。

---

## 从零到线上：全过程记录

### 1. 创建仓库

- 在 GitHub 上创建一个公开的仓库，并把旅行相关的 HTML / Markdown 文件上传到 `main` 分支。

### 2. 想清楚用「用户级」还是「项目级」Pages

- **User Page（用户级）**：仓库必须叫 `<用户名>.github.io`，每个账号只能有一个，访问地址是 `https://<用户名>.github.io`。
- **Project Page（项目级）**：任意仓库都能开启，访问地址是 `https://<用户名>.github.io/<仓库名>/`。

### 3. 调整仓库命名与入口

- 确认仓库名为 `luoyang-travel`（不要使用 `<用户名>.github.io` 命名），这样：
  - 项目页地址：`https://lzllzllzllzllzl.github.io/luoyang-travel/`
  - 顶级的 `lzllzllzllzllzl.github.io` 位置留给以后别的站点使用。
- 把原本的页面入口文件改名，让 GitHub Pages 能直接找到默认主页：
  - `git mv 洛阳旅行交互地图.html index.html`
  - `git commit`
  - `git push origin main`

### 4. 启用 GitHub Pages

在仓库设置里：

1. 打开 **Settings → Pages**。
2. **Build and deployment → Source** 选 **Deploy from a branch**。
3. **Branch** 选 `main`，**folder** 选 **`/(root)`**。
4. 保存，等待 1-2 分钟，访问 `https://lzllzllzllzllzl.github.io/luoyang-travel/` 即可。

### 5. 最终结果

- 交互地图：<https://lzllzllzllzllzl.github.io/luoyang-travel/>
- 行程交通指南：<https://lzllzllzllzllzl.github.io/luoyang-travel/洛阳行程交通指南.md>
- 酒店选择指南：<https://lzllzllzllzllzl.github.io/luoyang-travel/洛阳酒店选择指南.md>

---

## 文件说明

| 文件 | 说明 |
| --- | --- |
| `index.html` | 洛阳交互地图主页 |
| `洛阳行程交通指南.md` | 行程与交通 Markdown 文档，GitHub 在线渲染 |
| `洛阳酒店选择指南.md` | 酒店推荐 Markdown 文档 |

---

## 关于 GitHub Pages 类型的补充说明

- 每个 GitHub 账号只能有一个 **User Page**（仓库名必须是 `<用户名>.github.io`）。
- 但可以有任意多个 **Project Page**，每个仓库启用 Pages 后都可以通过 `https://<用户名>.github.io/<仓库名>/` 访问，互不冲突。

如果有多个项目想各自拥有独立网页，用 **Project Page** 是最省心的做法。只有当你有一个「主站 / 个人门户」的时候，再把 User Page 用在那个最重要的仓库上即可。

---

*Last updated: 2026-06-30*
