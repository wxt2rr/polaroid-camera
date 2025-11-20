# 📸 Web AR Polaroid Camera

一个基于 Web 的拟物化 AR 立拍得相机。

这个项目完全运行在浏览器中，利用 MediaPipe 实现人脸追踪，结合 CSS3 高级动画模拟真实的拍立得“显影”与“出片”体验。

> 💡 **Credit / 灵感来源**
>
> 本项目的创意与交互灵感来源于 X (Twitter) 用户 **[@ann_nnng](https://x.com/ann_nnng)** 的精彩想法。
> Idea inspired by @ann_nnng.

## ✨ 功能特性 (Features)

* **📷 拟物化设计**: 纯 CSS 实现的复古相机质感，包含呼吸灯快门、菲涅尔闪光灯纹理及磨砂机身细节。
* **🐶 AR 面部贴纸**: 集成 Google MediaPipe Face Mesh，支持实时面部追踪，自动佩戴 Emoji (🐶/🐱) 头像。
* **🎞️ 真实出片动画**: 还原立拍得相机“吐照片”的物理动画效果，照片生成后缓慢滑出。
* **✍️ 个性化编辑**: 支持自定义照片底部的签名文案。
* **💾 智能保存**:
    * 支持**拖拽**照片在桌面上整理布局。
    * 支持**单张下载**（自动扶正照片角度）。
    * 支持**整张桌面保存**，留住此刻的回忆。

## 🛠️ 技术栈 (Tech Stack)

* **Core**: 原生 HTML5 / CSS3 / JavaScript (无框架依赖)
* **AR Engine**: [MediaPipe Face Mesh](https://developers.google.com/mediapipe)
* **Screenshot**: [html2canvas](https://html2canvas.hertzen.com/)

## 🚀 快速开始 (Quick Start)

由于项目需要调用摄像头权限 (Camera API)，**不能**直接双击 HTML 文件打开，必须在本地服务器环境下运行。

### 方法 1: 使用 VS Code (推荐)
1.  克隆或下载本项目。
2.  安装 VS Code 插件 **Live Server**。
3.  右键点击 `index.html`，选择 "Open with Live Server"。

### 方法 2: 使用 Python
如果你安装了 Python，可以在项目根目录下运行：
```bash
python -m http.server