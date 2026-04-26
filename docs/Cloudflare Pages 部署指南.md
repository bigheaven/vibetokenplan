# Cloudflare Pages 部署指南（vibetokenplan.com）

> 适用于：vibetokenplan.com  
> 平台：Cloudflare Pages  
> 目标：快速上线静态网站（AI coding 工具对比站）

---

# 1. 概述

本项目使用 Cloudflare Pages 进行部署。

Cloudflare Pages 是一个静态网站托管平台，可以通过 GitHub 自动部署前端项目。

---

# 2. 部署架构

```text
GitHub Repository → Cloudflare Pages → vibetokenplan.com
```

---

# 3. 前置条件

在部署之前，需要准备：

* GitHub 账号
* Cloudflare 账号
* 已创建的 GitHub 项目（本网站代码）
* 已购买域名：vibetokenplan.com

---

# 4. GitHub 仓库要求

## 4.1 仓库类型

推荐使用：

* Public（推荐）
* Private（可选）

## 4.2 项目结构（静态站）

```text
/
  index.html
  /pages
  /assets
  style.css
```

---

# 5. Cloudflare Pages 部署步骤

## Step 1：进入 Cloudflare Pages

进入：

Cloudflare Dashboard → Pages

---

## Step 2：创建项目

点击：

> Create a project

---

## Step 3：连接 GitHub

选择：

> Connect to GitHub

并授权 Cloudflare 访问你的仓库。

---

## Step 4：选择仓库

选择你的项目仓库，例如：

* vibetokenplan

---

## Step 5：构建配置

### 如果是纯静态 HTML 项目：

```text
Framework preset: None
Build command: (留空)
Output folder: /
```

---

### 如果使用 Vite / React：

```text
Build command: npm run build
Output folder: dist
```

---

## Step 6：部署

点击：

> Deploy

等待 10～30 秒部署完成。

---

# 6. 绑定自定义域名

## Step 1：进入 Pages 设置

进入：

Pages → Custom domains

---

## Step 2：添加域名

输入：

```text
vibetokenplan.com
```

---

## Step 3：自动 DNS 配置

如果域名在 Cloudflare：

* 系统会自动配置 DNS

如果不在：

* 按提示手动添加 CNAME 记录

---

# 7. HTTPS & CDN

Cloudflare 会自动提供：

* HTTPS（SSL 自动开启）
* 全球 CDN 加速
* DDoS 防护

无需额外配置。

---

# 8. 推荐架构（本项目）

## 技术栈

* 前端：HTML / Vite / Next.js（任选）
* 部署：Cloudflare Pages
* DNS：Cloudflare

---

## 推荐原因

* 免费部署
* SEO 友好
* 全球访问快
* 适合内容型网站

---

# 9. 项目定位提醒

本网站定位：

> AI Coding 工具决策与对比平台

目标工具包括：

* GitHub Copilot
* Cursor
* Claude Code

---

# 10. 注意事项

## ❌ 不建议

* 一开始做复杂后端
* 做登录系统
* 做数据库系统

---

## ✅ 推荐

* 先做内容页面
* 先做工具对比
* 先做 SEO 流量

---

# 11. 当前状态

* 域名已购买 ✔
* GitHub 项目准备中 ✔
* Cloudflare Pages 待部署 ⏳

---

# 12. 下一步计划

1. 完成首页上线
2. 添加工具对比页
3. 发布第一篇 SEO 内容
4. 开始引流测试（Google / Reddit / X）

```

---

如果你下一步要做，我可以帮你继续升级两件关键东西：

👉 ① :contentReference[oaicite:0]{index=0}  
👉 ② 或:contentReference[oaicite:1]{index=1}
```
