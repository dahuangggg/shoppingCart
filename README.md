# vue-cart

[中文](#中文) | [English](#english)

---

## 中文

基于 Vue 3 + Vue Router 的购物车单页学习示例，用于练习 Vue 组件拆分与路由。

### 项目状态

早期学习项目，已不再维护。

### 功能

- 模拟登录页（`/login`）：提交表单后直接跳转到商品页，不做账号校验
- 商品页（`/products`）：按 iPhone / iPad / MacBook 分类展示商品，可加入购物车并增减数量
- 购物车列表：实时显示已选商品的名称、图片、数量和小计
- 总价计算，点击「结账」跳转到结账页（`/checkout`），显示订单总价
- 根路径 `/` 自动重定向到 `/login`
- 商品数据写死在前端，无后端

### 技术栈

- Vue 3
- Vue Router 4
- Vite 4（`@vitejs/plugin-vue`）
- npm

### 本地运行

```sh
npm install      # 安装依赖
npm run dev      # 启动开发服务器（热更新）
npm run build    # 构建生产版本到 dist/
npm run preview  # 本地预览构建结果
```

Vite 配置参考：[Vite Configuration Reference](https://vitejs.dev/config/)

### 目录结构

```
.
├── index.html           # 页面入口
├── vite.config.js       # Vite 配置（@ 指向 src）
├── public/              # 静态资源（favicon）
└── src/
    ├── main.js          # 创建应用并挂载路由
    ├── App.vue          # 根组件：页头 + router-view
    ├── router/index.js  # 路由定义
    ├── components/      # Login / ProductsPage / ProductList / Cart / Total / Checkout / MyHeader
    └── assets/          # 商品图片与全局样式
```

---

## English

A Vue 3 + Vue Router single-page shopping cart example, built to practice Vue components and routing.

### Status

Early learning project, no longer maintained.

### Features

- Mock login page (`/login`): submitting the form goes straight to the products page, with no credential check
- Products page (`/products`): items grouped into iPhone / iPad / MacBook; add to cart and adjust quantity
- Cart list: shows name, image, quantity and subtotal of selected items
- Running total; the "结账" (Checkout) button opens `/checkout`, which shows the order total
- Root path `/` redirects to `/login`
- Product data is hard-coded in the frontend; there is no backend

### Tech Stack

- Vue 3
- Vue Router 4
- Vite 4 (`@vitejs/plugin-vue`)
- npm

### Getting Started

```sh
npm install      # install dependencies
npm run dev      # start the dev server with hot reload
npm run build    # production build into dist/
npm run preview  # preview the production build locally
```

Vite config reference: [Vite Configuration Reference](https://vitejs.dev/config/)

### Directory Structure

```
.
├── index.html           # HTML entry
├── vite.config.js       # Vite config (@ alias -> src)
├── public/              # static assets (favicon)
└── src/
    ├── main.js          # creates the app and installs the router
    ├── App.vue          # root component: header + router-view
    ├── router/index.js  # route definitions
    ├── components/      # Login / ProductsPage / ProductList / Cart / Total / Checkout / MyHeader
    └── assets/          # product images and global CSS
```
