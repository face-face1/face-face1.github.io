It was exiting to explore a exactly new world.
## 文件说明
- `index.html`：主页，包含 PDF（iframe）和 EPUB（epub.js）预览按钮示例。
- `books/`：存放书籍文件（PDF/EPUB）。请把你的文件上传到该目录。

## 快速部署（推荐仓库名）
建议仓库名称： `face-face1.github.io`（将根据你的 GitHub 用户名自动部署为 https://face-face1.github.io）

### 通过命令行部署
1. 在 GitHub 上新建仓库 `face-face1.github.io`（Public）。
2. 本地初始化并推送：
```bash
# 假设已在项目目录（包含 index.html）下
git init
git add .
git commit -m "Init GitHub Pages site with book preview"
git branch -M main
git remote add origin https://github.com/face-face1/face-face1.github.io.git
git push -u origin main
```
3. 等几分钟后访问： `https://face-face1.github.io`

### 通过 GitHub 网页上传
1. 在仓库页面点击 Add file → Upload files，把 `index.html` 和 `books/` 上传。
2. Commit 后等待几分钟，通过 `https://face-face1.github.io` 访问。

## 使用方法
- 把你的 PDF/EPUB 文件放到 `books/` 目录（文件名不要包含空格更好）。
- 修改 `index.html` 中按钮所用的路径为你的文件路径，或直接在页面中添加更多按钮。
- 访问你的 GitHub Pages 地址并点击“预览”按钮即可在线查看。

## 注意事项与替代方案
- 单文件限制：GitHub 对单文件上传有约 100 MB 限制（通过 git push 或网页上传都适用）。如果你的书籍大于 100 MB，请使用下列方法之一：
  - 把文件上传到 Internet Archive（https://archive.org）：免费、支持大文件并能生成稳定直链。上传后把 archive 的下载链接填到 `index.html` 的按钮中。
  - 使用第三方云盘（Google Drive / Dropbox），将文件设为公开并获得可直接访问的直链（注意带宽限制）。
  - 使用 Git LFS：可以上传大文件但免费配额有限，不推荐大量免费存储。
- 私密访问：GitHub Pages 是公开托管。若需要受限访问，需要用带认证的服务器或私有存储方案（不在本模板范围内）。
- EPUB 兼容性：epub.js 能渲染大多数 EPUB，但部分带复杂 CSS 的 EPUB 可能样式显示不完全一致。

## 如果你需要我帮忙
- 我可以把这个模板直接打包为仓库文件结构并给出你完整的 push 命令（也可以直接帮你生成并说明每一步）。
- 如果你把一份公开的文件 URL（或把文件上传到仓库并告诉我路径），我可以帮你修改 `index.html` 以便直接预览该文件。
- 如果你的文件过大（>100MB），我可以指导你如何把文件上传到 Internet Archive 并给出示例链接写法。
