# Personal-use-gadget 统一风格描述

## 风格名称

**Luminous Glass Grid Utility / 发光玻璃网格工具风**

该风格来源于 `hotspot_key.html` 的极简仪表盘感，以及 `pdf-merger.html` 的暗色工业工具界面。

---

## 核心关键词

- 暗色工业感
- 等宽字体
- 细网格背景
- 玻璃拟态面板
- 低圆角矩形
- 高对比边框
- 荧光强调色
- 背景光晕与粒子
- 克制但高级的动态光效
- 信息密度适中
- 工具面板式布局
- 本地运行 / 不上传文件 的安全感表达

---

## 色彩系统

### 主色

```css
--bg: #0e0e10;
--surface: #16161a;
--surface-2: #101014;
--border: #2a2a32;
--text: #e2e2e8;
--text-dim: #7a7a8c;
```

### 强调色

```css
--accent: #e8ff47;
--accent-dim: #b8cc30;
```

强调色用于：

- 标题中的重点字
- 主按钮
- 拖拽区域 hover/active
- 进度条
- 数字/统计高亮
- 小型状态点

### 状态色

```css
--danger: #ff4757;
--success: #2ecc71;
--warn: #ffb020;
```

---

## 字体

推荐：

```css
--mono: 'Space Mono', 'DM Mono', monospace;
--sans: 'Noto Sans SC', system-ui, sans-serif;
```

使用规则：

- 标题、按钮、标签、状态、文件名：等宽字体
- 正文说明：中文无衬线字体
- 大数字/Key 展示：可使用 `Bebas Neue`

---

## 布局规则

### 页面容器

```css
max-width: 820px;
margin: 0 auto;
padding: 48px 24px 80px;
```

大型工具可扩展到：

```css
max-width: 1100px;
```

### 页面背景

统一使用细网格：

```css
body::before {
  background-image:
    linear-gradient(var(--border) 1px, transparent 1px),
    linear-gradient(90deg, var(--border) 1px, transparent 1px);
  background-size: 40px 40px;
  opacity: 0.3;
}
```

---

## 组件风格

### Header

结构建议：

```html
<div class="header">
  <div class="header-eyebrow">工具分类</div>
  <h1>工具 <span>标题</span></h1>
  <p class="header-sub">// 功能描述 · 本地处理 · 不上传服务器</p>
</div>
```

特点：

- eyebrow 使用荧光色
- h1 使用等宽粗体
- h1 中的 `<span>` 使用强调色
- 副标题使用 `//` 开头，像命令行注释

---

### 卡片 / 面板

```css
background: var(--surface);
border: 1.5px solid var(--border);
border-radius: 4px;
```

避免大圆角和强阴影，保持工具感、硬边界。

---

### 按钮

- 默认透明边框按钮
- 主按钮使用荧光色实心
- 危险按钮使用红色边框
- 按下时轻微缩放

```css
.btn {
  font-family: var(--mono);
  text-transform: uppercase;
  letter-spacing: 0.1em;
  border-radius: 4px;
}
```

---

### 输入框

```css
background: var(--bg);
border: 1.5px solid var(--border);
color: var(--text);
font-family: var(--mono);
```

聚焦时边框变为强调色。

---

### 拖拽区域

- 虚线边框
- 深色 surface 背景
- hover/dragover 时强调色边框
- 图标线条颜色跟随状态变化

---

## 动效

只使用短、克制的动效：

```css
transition: 0.15s;
animation: slideIn 0.18s ease;
```

推荐动效：

- 页面进入：轻微上移 + 淡入
- 文件项出现：轻微下落
- 按钮点击：`scale(0.97)`
- 关键数字 reveal：字距收缩

---

## 文案风格

倾向：

```text
// 多文件合并 · 拖拽排序 · 纯浏览器处理 · 不上传服务器
```

用 `·` 分隔能力，用 `//` 表示工具注释。

---

## 高级视觉效果

玻璃拟态、复杂背景粒子、光晕和微渐变是加分项，但需要服从工具可读性：

- 面板可使用 `backdrop-filter: blur(18px)`。
- 背景可叠加网格、径向光晕、扫光和少量粒子。
- 粒子应低透明度、慢速移动，不能干扰文字。
- 渐变用于背景和强调，不用于大段正文区域。
- 阴影可以带轻微荧光，但不要让边界糊掉。

## 设计边界

应避免：

- 大圆角卡片导致工具感下降
- 彩色无规则堆叠
- 动效过快或闪烁
- 文字区域对比度不足
- 表单和按钮可点击区域不明显

保留：

- 网格
- 等宽字体
- 明确边框
- 玻璃面板
- 背景光效
- 高信息密度
- 荧光强调色
- 工具面板感
