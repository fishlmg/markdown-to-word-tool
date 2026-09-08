# Markdown 转 Word 粘贴工具

单文件 HTML 实现的 Markdown 编辑器：左侧编辑 Markdown，右侧实时预览，渲染后的富文本可直接复制粘贴到 Word，保持标题、列表、表格等格式。

## 特点

- 纯前端单文件，无需构建，浏览器直接打开
- 唯一外部依赖：[marked.js](https://marked.js.org/)（CDN 加载）
- 支持 GitHub 风格 Markdown（GFM）

## 使用

直接用浏览器打开 `transformer.html` 即可。

## 文件结构

```
├── transformer.html   # 工具本体（HTML + CSS + JS）
└── explain.md         # 技术实现文档
```
