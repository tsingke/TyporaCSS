# TyporaCSS：一款好看好用的样式主题
本项目是一款为 Typora 编辑器量身打造的专业级 Markdown 主题，注重阅读体验、排版美感与代码展示，适用于日常写作、技术文档、科研笔记等多种场景。

---
项目地址：[https://github.com/tsingke/TyporaCSS](https://github.com/tsingke/TyporaCSS)

## 主题特点

- 简洁现代的设计风格，排版舒适，阅读友好
- 栅格化内容区，保持页面居中且宽度适中（约 860px）
- 全局采用 CSS 变量，方便自定义主题色和暗色模式扩展
- 多层级标题样式清晰，主标题具备横条背景与左侧高亮标识
- 支持代码高亮、自动行号、语言徽标与滚动条美化
- 表格、引用、列表等 Markdown 元素风格统一
- 兼容 Obsidian 编辑器的 Live Preview 显示效果

---

## 安装方法

1. **定位 Typora 主题目录：**

   - macOS: `~/Library/Application Support/abnerworks.Typora/themes/`
   - Windows: `%APPDATA%\Typora\themes\`
   - Linux: `~/.config/Typora/themes/`

2. **下载本主题文件：**

   克隆项目或直接下载 `TyporaCSS` 文件：

3. **拷贝主题文件：**

   将 `TyporaCSS.css` 复制至 Typora 的主题目录中。

4. **在 Typora 中启用主题：**

   打开 Typora → 偏好设置 → 外观 → 主题 → 选择 `TyporaCSS`。

5. **重启 Typora**

---

## 主题预览 (作品：PSO 算法科普范例)

<img width="418" height="511" alt="image" src="https://github.com/user-attachments/assets/dc406ece-72df-461b-84ec-f895011e8374" />


---

## 高级定制

### 自定义颜色方案

本主题使用 `:root` 中定义的 CSS 变量集中管理颜色配置，便于修改：

```css
:root {
  --heading-bg: #38a38b;
  --heading-accent: #f2c94c;
  --text-accent: #38a38b;
  --code-bg: #f7f7f7;
  ...
}
```

### 支持暗色模式（可选）

可添加如下代码实现根据系统偏好自动切换暗色风格：

```css title:css
@media (prefers-color-scheme: dark) {
  :root {
    --background: #1e1e1e;
    --text-color: #eeeeee;
    ...
  }
}
```

---

## 常见问题

- 若主题不生效，请确保 `.css` 文件已复制到正确的目录并在 Typora 中选中该主题；
- Obsidian 用户需确认所使用模式为 " 阅读视图 " 或 " 实时预览 "；
- 如出现代码行号错位，可能与 Markdown 渲染器不一致有关；
- 可扩展添加多语言徽标、数学公式样式优化、甚至支持自定义字体加载。

---

## 许可证

本项目使用 MIT 开源许可证，允许自由修改与分发。请在引用或二次开发时保留作者信息@**氢客探道**。

---
