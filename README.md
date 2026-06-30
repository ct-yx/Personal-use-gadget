# LumeKit Tools｜离线浏览器工具箱

**LumeKit Tools** 是一个隐私优先的纯前端工具集合，面向 PDF、二维码、文本、图片与 Android APK/XAPK 等日常处理场景。所有工具均以静态 HTML/CSS/JavaScript 实现，可直接在浏览器中运行，文件默认只在本地处理，不需要上传服务器。

> 🌐 在线访问：<https://ct-yx.github.io/Personal-use-gadget/>

## 核心特点

- **离线优先**：页面加载后即可在浏览器本地完成主要处理流程。
- **隐私友好**：PDF、图片、文本、APK/XAPK 等文件不上传到服务器。
- **无需安装**：不需要客户端、不需要后端服务，打开网页即可使用。
- **跨平台**：支持桌面端与移动端现代浏览器。
- **高颜值界面**：统一采用发光玻璃网格工具风，适合长期维护和扩展。

## 工具列表

### PDF 工具

| 工具 | 说明 | 在线页面 |
|---|---|---|
| **PDF 合并工具** | 浏览器本地合并多个 PDF，支持拖拽排序、页数与大小预览。 | [pdf-merger.html](https://ct-yx.github.io/Personal-use-gadget/pdf-merger.html) |
| **PDF 页面重排工具** | 支持一页两张、一页四张、横向/纵向布局，适合打印排版。 | [PDFchange.html](https://ct-yx.github.io/Personal-use-gadget/PDFchange.html) |

### 文本与电子书工具

| 工具 | 说明 | 在线页面 |
|---|---|---|
| **对话提取与语料压缩工具** | 聊天记录筛选、相似去重、表情移除和 AI 语料清洗。 | [chat-filter-tool.html](https://ct-yx.github.io/Personal-use-gadget/chat-filter-tool.html) |
| **大文件分割工具** | 按字符数或字节大小切割大文本、日志和数据文件。 | [Partition1.0.html](https://ct-yx.github.io/Personal-use-gadget/Partition1.0.html) |
| **Markdown 转 EPUB 合成器** | 多 Markdown 文件合并为 EPUB，支持章节、目录和封面。 | [txt-epub-manger.html](https://ct-yx.github.io/Personal-use-gadget/txt-epub-manger.html) |
| **TXT 章节整理工具** | 小说、网文和长文本的章节识别、清洗与格式规范化。 | [章节整理工具.html](https://ct-yx.github.io/Personal-use-gadget/%E7%AB%A0%E8%8A%82%E6%95%B4%E7%90%86%E5%B7%A5%E5%85%B7.html) |

### 图片与二维码工具

| 工具 | 说明 | 在线页面 |
|---|---|---|
| **长截图切割工具** | 将长截图自动切割成 9:16 手机截图，支持 ZIP 批量下载。 | [split-screenshot.html](https://ct-yx.github.io/Personal-use-gadget/split-screenshot.html) |
| **二维码生成与解码工具** | 生成二维码、识别二维码图片，并支持摄像头扫码。 | [qr-tool.html](https://ct-yx.github.io/Personal-use-gadget/qr-tool.html) |

### Android 与实用工具

| 工具 | 说明 | 在线页面 |
|---|---|---|
| **XAPK 转 APK 离线转换签名工具** | 本地解析 XAPK/APKPure 包、清理旧签名、重打包并进行 APK v1 签名。 | [xapk-apk-converter.html](https://ct-yx.github.io/Personal-use-gadget/xapk-apk-converter.html) |
| **HOTSPOT KEY** | 基于每日时间窗口的动态密码生成器，支持复制和倒计时。 | [hotspot_key.html](https://ct-yx.github.io/Personal-use-gadget/hotspot_key.html) |

## 使用方式

### 在线使用

访问 GitHub Pages：

```text
https://ct-yx.github.io/Personal-use-gadget/
```

### 本地使用

```bash
git clone https://github.com/ct-yx/Personal-use-gadget.git
cd Personal-use-gadget
```

然后直接用浏览器打开任意 `.html` 文件。

## 搜索关键词

离线工具箱、浏览器工具箱、纯前端工具、本地 PDF 合并、PDF 页面重排、二维码生成、二维码解码、XAPK 转 APK、APK 离线签名、文本整理、聊天记录清洗、Markdown 转 EPUB、长截图切割、文件分割。

## 技术栈

- HTML / CSS / JavaScript
- Web Crypto API
- IndexedDB
- PDF.js / pdf-lib
- JSZip
- QRCode / jsQR
- GitHub Pages

## 隐私说明

本项目的核心目标是让常见文件处理尽可能在浏览器本地完成。除页面资源加载外，工具本身不会主动上传用户选择的 PDF、图片、文本、APK/XAPK 等文件。

## License

MIT
