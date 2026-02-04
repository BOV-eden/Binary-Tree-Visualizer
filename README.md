# 🌳 Infinity Tree: 可视化二叉搜索树引擎

> **"简约而不简单。"**
> 一个基于 Web 的、支持无限画布与手势交互的二叉搜索树（BST）可视化工具。

本项目是我在学习数据结构期间，为了深入理解 BST 算法逻辑，**与 AI 结对编程**（Pair Programming）完成的单文件可视化引擎。它从最初的静态图演示，迭代至目前支持**无限视口缩放**、**级联拖拽**和**全平台适配**的最终版本。

## ✨ 核心特性 (Features)

### 🎨 极致交互体验
* **♾️ 无限画布 (Infinite Canvas)**：突破屏幕限制，支持超大规模树结构的展示。
* **🔍 自由缩放 (Zoom & Pan)**：
    * 桌面端：鼠标滚轮缩放、拖拽空白处平移。
    * 移动端：双指捏合（Pinch）缩放、单指平移。
* **👆 级联拖拽 (Subtree Dragging)**：物理手感极佳的交互体验。拖动任意父节点，其整棵子树会像刚体一样跟随移动，保持相对结构不变。
* **📱 完美移动端适配**：针对 iOS/Android 优化，支持 `100dvh` 动态视口，适配刘海屏与底部安全区，拒绝误触。

### 🧠 算法可视化
* **动态构建**：输入数值自动按 BST 规则插入，并智能计算节点初始坐标，避免重叠。
* **四种遍历演示**：
    * 前序 (Pre-order)
    * 中序 (In-order)
    * 后序 (Post-order)
    * 层序 (Level-order / BFS)
* **沉浸式查找**：高亮显示查找路径，镜头自动跟随节点移动 (Auto-Focus)。

### 💎 清爽 UI 设计 (Light Tech Theme)
* **极简主义**：采用“科技白”配色，搭配点阵背景 (Dot Grid)。
* **细节打磨**：节点采用 Apple 风格渐变蓝，配合 SVG 动态连线，视觉清晰锐利。

## 🛠️ 技术栈 (Tech Stack)

* **HTML5 / CSS3**: Flexbox 布局, CSS Variables, Backdrop Filter (毛玻璃效果)。
* **JavaScript (ES6+)**: 原生实现，**无任何第三方库依赖** (No jQuery, No React/Vue)。
* **SVG**: 使用 `vector-effect` 和动态坐标计算，实现高性能的贝塞尔曲线连接。

## 🚀 快速开始 (Quick Start)

本项目为**单文件应用 (Single File Component)**，部署极简：

1.  **下载**：克隆仓库或下载 `index.html`。
2.  **运行**：双击 `index.html` 在浏览器打开即可。
3.  **体验**：推荐在手机端打开 GitHub Pages 链接，体验丝滑的触控交互。


## 📝 开发日志

* **v1.0**: 静态 HTML/CSS 布局还原。
* **v2.0**: 引入 JS 类与递归逻辑，实现基础 BST 插入与查找。
* **v3.0**: 增加节点拖拽功能。
* **v4.0**: 实现“级联拖拽”算法 (Subtree movement)。
* **v5.0**: 引入“无限画布”与坐标系变换，解决节点溢出问题。
* **v6.0**: 移动端深度适配 (Touch Events + Viewport Fixes)。
* **v7.0 (Current)**: UI 重构为“清爽白”主题，修复 SVG 渲染层级问题。

---
*Created with ❤️ & ☕ by BOV-eden & Gemini, 2026.*
