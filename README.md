# 🧰 个人小工具集

随手让 AI 写的实用小工具合集 —— 全都是纯静态 HTML，打开浏览器即用，无需安装、不传服务器。

> 🌐 **在线主页：** [https://ct-yx.github.io/Personal-use-gadget](https://ct-yx.github.io/Personal-use-gadget)

---

## 📦 工具列表

### 📄 PDF 相关

| 工具 | 说明 | 链接 |
|------|------|------|
| **PDF 合成工具** | 合并多个 PDF，支持拖拽排序、实时页数统计 | [`pdf-merger.html`](./pdf-merger.html) |
| **PDF 页面重排工具** | 将 PDF 页重排为 2 合 1 / 4 合 1 布局 | [`PDFchange.html`](./PDFchange.html) |

### 📝 文本处理

| 工具 | 说明 | 链接 |
|------|------|------|
| **对话提取 · 语料压缩工具** | 聊天记录过滤、去重、语料裁剪，专为 AI 语料准备 | [`chat-filter-tool.html`](./chat-filter-tool.html) |
| **浏览器文件分割工具** | 大文本文件按字符/字节分割，智能切割点避免乱码 | [`Partition1.0.html`](./Partition1.0.html) |
| **MD → EPUB 合成器** | 多 Markdown 文件合并导出标准 EPUB 电子书 | [`txt-epub-manger.html`](./txt-epub-manger.html) |
| **TXT 智能整理专家** | 自动识别章节、清理冗余、格式化长篇文本 | [`章节整理工具.html`](./章节整理工具.html) |

### 🖼️ 图片工具

| 工具 | 说明 | 链接 |
|------|------|------|
| **长截图 9:16 分割工具** | 长截图按 9:16 比例自动切割，支持 ZIP 批量下载 | [`split-screenshot.html`](./split-screenshot.html) |

### 🔧 其他

| 工具 | 说明 | 链接 |
|------|------|------|
| **HOTSPOT KEY** | 基于时间戳的每日动态密码生成器 | [`hotspot_key.html`](./hotspot_key.html) |

---

## 🚀 使用方式

1. 克隆仓库到本地
2. 直接用浏览器打开任意 `.html` 文件
3. 或访问 [GitHub Pages 在线主页](https://ct-yx.github.io/Personal-use-gadget)

所有数据均在本地浏览器处理，**不会上传到任何服务器** 🛡️

---

## 🛠️ 技术栈

- 纯 HTML / CSS / JavaScript
- [pdf-lib](https://pdf-lib.org/) — PDF 操作
- [jszip](https://stuk.github.io/jszip/) — 打包下载
- [marked](https://marked.js.org/) — Markdown 渲染

---

## 📄 License

MIT
