# Markdown 实时预览并复制粘贴到 Word

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-single%20file-orange.svg)](index.html)

一个**零依赖构建**的单文件网页工具：左侧编辑 Markdown，右侧实时预览，渲染后的富文本可直接复制，再粘贴到 Microsoft Word，并保留标题、列表、表格、代码块等格式。

页面只把渲染结果放进剪贴板。Word 文档由粘贴的那一端保存，这个页面不写出 `.docx` 文件。

## ✨ 特性

- **单文件应用**：所有功能集成在一个 HTML 文件中，无需安装、无需构建
- **开箱即用**：浏览器直接打开 `index.html` 即可使用
- **实时预览**：编辑 Markdown 即时渲染
- **GFM 支持**：GitHub 风格 Markdown（表格、删除线、任务列表等）
- **粘贴友好**：输出富文本，复制到 Word 保持排版格式
- 唯一外部依赖：marked.js（通过 CDN 加载）

## 🗂 项目结构

```
.
├── index.html    # 工具本体，也是 GitHub Pages 入口
├── explain.md    # 技术实现文档（架构与实现细节）
├── .nojekyll     # 让 Pages 按静态文件发布，不经 Jekyll 处理
├── LICENSE
└── README.md
```

## 🚀 使用方法

### 本地打开

用浏览器打开 `index.html`（原先的 `transformer.html` 已改成这个文件名，方便作为 Pages 入口）：

1. 在左侧文本框输入 Markdown
2. 右侧实时查看渲染效果
3. 点击「复制富文本」，或选中预览区后复制（`⌘/Ctrl + C`）
4. 粘贴到 Word 文档中，格式由 Word 保留

### 在线使用（GitHub Pages）

开启 Pages 后的站点地址：

<https://fishlmg.github.io/markdown-to-word-tool/>

1. 打开仓库 **Settings → Pages**
2. **Build and deployment** 的 Source 选择 **Deploy from a branch**
3. Branch 选择 **main**，文件夹选择 **/ (root)**，保存
4. 等部署完成后再访问上面的地址。入口是根目录的 `index.html`；`.nojekyll` 用来跳过 Jekyll

仓库 About 里的 Description 和 Website 存在 GitHub 设置中，不会随 README 自动更新。Pages 部署成功后，在仓库主页 About 里填写：

- **Description：** `Markdown 实时预览并复制粘贴到 Word 的单文件网页工具`
- **Website：** `https://fishlmg.github.io/markdown-to-word-tool/`

Website 在 Pages 生效前先留空。填上之前，上面的链接还打不开。

## 🛠 技术实现

- **HTML5**：语义化标签、响应式 Flexbox 布局
- **CSS3**：内联样式、现代排版
- **JavaScript ES6+**：事件驱动、异步渲染
- **marked.js**：Markdown 解析引擎（CDN 引入）

详细的架构设计与实现思路见 [explain.md](explain.md)。

## 📄 许可证

[MIT License](LICENSE)
