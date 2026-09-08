# Markdown 转 Word 粘贴工具

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-single%20file-orange.svg)]()

一个**零依赖构建**的单文件网页工具：左侧编辑 Markdown，右侧实时预览，渲染后的富文本可直接复制粘贴到 Microsoft Word，并保留标题、列表、表格、代码块等格式。

## ✨ 特性

- **单文件应用**：所有功能集成在一个 HTML 文件中，无需安装、无需构建
- **开箱即用**：浏览器直接打开 `transformer.html` 即可使用
- **实时预览**：编辑 Markdown 即时渲染
- **GFM 支持**：GitHub 风格 Markdown（表格、删除线、任务列表等）
- **粘贴友好**：输出富文本，复制到 Word 保持排版格式
- 唯一外部依赖：marked.js（通过 CDN 加载）

## 🗂 项目结构

```
.
├── transformer.html   # 工具本体（HTML 结构 + CSS 样式 + JS 逻辑）
└── explain.md         # 技术实现文档（架构与实现细节）
```

## 🚀 使用方法

直接用浏览器打开 `transformer.html`：

1. 在左侧文本框输入 Markdown
2. 右侧实时查看渲染效果
3. 选中预览区内容复制（`⌘/Ctrl + C`）
4. 粘贴到 Word 文档中，格式自动保留

## 🛠 技术实现

- **HTML5**：语义化标签、响应式 Flexbox 布局
- **CSS3**：内联样式、现代排版
- **JavaScript ES6+**：事件驱动、异步渲染
- **marked.js**：Markdown 解析引擎（CDN 引入）

详细的架构设计与实现思路见 [explain.md](explain.md)。

## 📄 许可证

[MIT License](LICENSE)
