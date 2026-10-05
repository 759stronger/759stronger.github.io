# 石连勇个人主页

石连勇的个人主页，介绍个人背景、AI 应用与 C++ 开发方向，以及 Reactor、Qt 音乐播放器和 atrain CLI 三个项目。网站采用静态 HTML 与 SVG，无需安装前端依赖。atrain CLI 处于开发阶段，源码整理中。

在线地址：[https://759stronger.github.io](https://759stronger.github.io)。已于 2026-10-05 完成 GitHub Pages 部署与公网页面访问验收。默认分支为 `main`，发布源为根目录，后续网站提交由 Pages 自动部署。

## 文件

- `index.html`：个人主页，包含个人介绍与项目展示。
- `.nojekyll`：空文件，放在发布源根目录，关闭默认的 Jekyll 构建。
- `README.md`：项目与部署说明。
- `assets/`：项目结构示意图与站点图标，部署时保留目录结构。

## 本地预览

在浏览器中打开 `index.html` 可进行基础预览。如本机已安装 Python，也可在本目录运行 `python -m http.server 8000 --bind 127.0.0.1`，再访问 `http://localhost:8000`。本地 J 盘路径和 localhost 地址只能用于本机预览，不能当作公网作品集链接。

## GitHub Pages 部署

1. 在账号 `759stronger` 下创建或确认仓库 `759stronger.github.io`，使用 GitHub Free 时仓库需为 Public。
2. 将本目录的网站文件提交到仓库 `main` 分支根目录，确保 `index.html` 与 `.nojekyll` 位于同一发布源根目录。
3. 在仓库 **Settings → Pages → Build and deployment** 中，将 **Source** 设置为 **Deploy from a branch**，选择 **main** 与 **/(root)**，然后保存。
4. 等待 GitHub 的 Pages 部署任务完成，从 Pages 设置中的 **Visit site** 打开页面，检查首页、移动端布局和项目链接，再确认上述目标地址可公开访问。

本页面不需要自定义构建流程或额外的 workflow 文件。分支发布由 GitHub 的 Pages 部署流程执行。部署方式依据：[创建 GitHub Pages 站点](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)与[配置发布源](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。

## 更新页面

个人介绍与项目内容位于 `index.html`，结构图和图标位于 `assets/`。保留资源目录结构，在本地预览后提交到 `main`，GitHub Pages 会自动发布更新。
