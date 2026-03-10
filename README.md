# 🚀 联盟网站部署指南

> 这是一个基于GitHub Pages的自动化联盟营销网站，使用Jekyll构建。

## 📦 已生成的文件

```
affiliate-site/
├── _config.yml          # 网站配置（请填写你的联盟ID）
├── _layouts/
│   └── default.html    # 页面模板
├── _posts/             # 5篇示例评测文章
│   ├── 2025-01-01-best-ai-writing-tools.md
│   ├── 2025-01-01-ai-coding-assistants.md
│   ├── 2025-01-01-free-vs-paid-ai.md
│   ├── 2025-01-01-ai-video-tools.md
│   └── 2025-01-01-small-business-ai.md
├── assets/
│   └── css/
│       └── style.css  # 样式文件
├── index.html          # 首页
└── about.md           # 关于页面（可选）
```

## 🛠️ 5分钟部署步骤

### 第1步：创建GitHub仓库

1. 登录GitHub（https://github.com）
2. 点击右上角 `+` → `New repository`
3. 填写：
   - **Repository name**: `affiliate-site`
   - **Public** (必须公开才能免费托管)
   - ✅ `Add a README file`
4. 点击 `Create repository`

### 第2步：上传网站文件

进入刚创建的仓库（`https://github.com/YANSU7/affiliate-site`）：

1. 点击 `Add file` → `Upload files`
2. 拖拽整个 `affiliate-site/` 文件夹内容到窗口
3. 填写 `Commit message`: `Initial commit with affiliate site`
4. 点击 `Commit changes`

### 第3步：启用GitHub Pages

1. 在仓库页面点击 `Settings` (顶部选项卡)
2. 左侧选择 `Pages`
3. 在 `Build and deployment` 下：
   - **Source**: 选择 `Deploy from a branch`
   - **Branch**: 选择 `main` → `/root` (默认)
4. 点击 `Save`

### 第4步：等待上线

- 保存后页面会显示：`Your site is published at https://yansu7.github.io/affiliate-site/`
- 首次部署需要1-3分钟
- 之后访问该URL即可看到网站

---

## 🔧 配置联盟链接

编辑 `_config.yml`，替换以下内容为你的真实联盟ID：

```yaml
affiliate_amazon_tag: YOUR_AMAZON_TAG   # 例如: johndoe-20
affiliate_taobao_id: YOUR_TAOBAO_ID     # 淘宝客ID
affiliate_jd_id: YOUR_JD_ID             # 京东联盟ID
```

然后在所有文章链接中使用 `{{ site.affiliate_amazon_tag }}` 变量。

---

## 📝 后续添加文章

1. 在本地编辑 `_posts/` 中的markdown文件
2. 新建文章命名格式：`YYYY-MM-DD-文章标题.md`
3. Front matter示例：

```markdown
---
layout: post
title: "你的文章标题"
date: 2025-01-02 10:00:00 +0800
categories: ai-tools
---
文章内容...
```

4. 推送后GitHub Pages会自动重建

---

## 🛡️ 关于合规

- 网站包含联盟链接，建议在页面底部添加「免责声明」
- 本模板已包含 `disclaimer.md` 页面链接
- 各联盟平台规则不同，请遵守其推广政策

---

## ❓ 问题？

联系机器人助手，或在仓库提交Issue。

祝躺赚愉快！💰