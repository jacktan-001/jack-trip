# Jack Trip · 多人旅行协作网页

多人旅行协作单页应用（SPA）。基于功能清单（桌面 `多人旅行协作网页功能清单.docx`）实现，包含首页看板、行程规划、多人记账与自动结算、攻略收藏、成员权限、物品清单、投票决策、地图路线 8 大模块。

技术栈：Vite 6 + React 19 + TypeScript + Tailwind CSS v4。数据通过浏览器 `localStorage` 持久化，内置「日本关西之旅」5 人示例数据。

## 部署说明（Cloudflare Pages 静态直出）

本仓库根目录为构建产物（`dist/` 内容），Cloudflare 以「静态 / 无构建」模式直接托管根目录 `index.html`，并依赖 `_redirects` 实现 SPA 深链回退：

```
/* /index.html 200
```

## 本地开发 / 重新构建

源码位于本地 Jack Trip 工作区：

```bash
npm install
npm run dev        # 本地预览
npm run build      # 产物输出到 dist/
```

将 `dist/` 内容重新推送到本仓库根目录即可更新线上站点。如需改为「源码构建」模式，可将完整 Vite 项目源码推送至分支，并在 Cloudflare 设置：构建命令 `npm run build`，输出目录 `dist`。
