# Jack Trip · 多人旅行协作

多人旅行协作网页应用，支持行程规划、成员管理、费用分摊与清单协作。
纯前端单页应用（SPA），无后端依赖，数据保存在浏览器本地。

## 技术栈
- Vite 6 + React 19 + TypeScript
- Tailwind CSS v4
- react-router-dom v6
- lucide-react 图标

## 本地开发
```bash
npm install
npm run dev
```

## 构建
```bash
npm run build   # 输出到 dist/
```

## 部署
静态站点，部署至 Cloudflare Pages（仓库根目录直出，构建命令为空，输出目录 `/`）。
线上地址：https://jack-trip.pages.dev

## 功能模块
- 行程（Itinerary）：多日行程与地点编排
- 成员（Members）：同行成员与权限管理
- 费用（Expenses）：支出记录与按成员分摊
- 清单（Checklist）：出行物品与任务协作
- 主题切换：浅色 / 深色
- 离线优先：数据存于浏览器本地存储
