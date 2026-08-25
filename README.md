# 个人网站

## 如何使用

### 1. 修改内容

- **首页** `index.html`：修改头像（替换 `assets/img/avatar.jpg`）、姓名、简介、链接
- **简历** `resume.html`：简历页支持**中/英**切换（顶部「中文 / English」按钮），中文与英文内容分别在页面内切换
- **作品集** `portfolio.html`：修改项目卡片、截图（放到 `assets/img/`）、链接

### 2. 替换资源

- 替换 `assets/img/avatar.jpg` 为你的头像
- 替换 `assets/img/project1.jpg` ~ `project4.jpg` 为项目截图
- `assets/files/resume_zh.pdf`：中文完整简历
- `assets/files/resume_en.pdf`：英文完整简历

### 3. 部署到 GitHub Pages

# 在 website 目录下初始化 git
git init
git add .
git commit -m "Initial commit"

# 创建 GitHub 仓库（例如 PandaShock.github.io）
# 然后推送
git remote add origin https://github.com/PandaShock/PandaShock.github.io.git
git branch -M main
git push -u origin main

推送后，打开 GitHub 仓库 Settings > Pages，将 Source 设为 `main` 分支根目录（或 `/docs` 如果放 docs 目录下），保存后稍等片刻即可通过 `https://PandaShock.github.io` 访问。

### 4. 本地预览

直接用浏览器打开 `index.html` 即可预览。图片链接使用了 `https://placehold.co` 占位图服务，无网络时会显示空白（不影响功能）。

## 目录结构

```
website/
├── index.html           # 首页
├── resume.html          # 简历
├── portfolio.html       # 作品集
└── assets/
    ├── css/
    │   └── style.css    # 样式
    ├── img/             # 放图片（头像、项目截图）
    └── files/           # 放文件（简历 PDF）
```
