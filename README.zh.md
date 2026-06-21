<div align="center">

# 📖 AI 看书 · 划词即问

**一个免费、单文件的 PDF 阅读器，内置 AI 家教。看到不懂的地方，选中文字就地解释——不用复制粘贴，不用切换软件。**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
![无需构建](https://img.shields.io/badge/构建-无-brightgreen)
![单文件](https://img.shields.io/badge/单文件-HTML-orange)
![纯前端](https://img.shields.io/badge/100%25-纯前端-success)
![欢迎PR](https://img.shields.io/badge/PR-欢迎-ff69b4)

[English](README.md) · 中文

</div>

---

> 读一本难啃的书或论文，卡在某段看不懂？不必中断思路去开 ChatGPT 再粘贴——直接**选中它**，AI 就在侧栏用大白话加例子帮你解释、翻译或总结。

## ✨ 功能

- **🖱️ 划词即问** — 选中任意文字 → **解释 · 翻译 · 总结 · 高亮 · 提问**
- **📚 书架** — 导入多本 PDF，封面 + 阅读进度一目了然
- **🔖 进度记忆 + 书签** — 自动记住读到哪；一键收藏页面
- **🖍️ 高亮 + 笔记** — 标记原文、附上笔记，集中管理
- **🔎 AI 找页** — 用大白话描述要找的内容，AI 帮你定位到对应页
- **🎯 三种提问范围** — 选中文字 / 当前页 / **整本书**
- **💬 每本书独立聊天记录** — 换书不串，下次打开还在
- **🌗 普通 / 护眼 / 深色** 三种主题
- **🌐 中英双语界面** — 一键切换
- **📱 全平台可用** — 手机、电脑，一个网址搞定

## 🔒 隐私与免费

**没有服务器。** 书、进度、高亮、聊天全部存在**你自己浏览器**里（IndexedDB），不离开你的设备。AI 用你**自己的免费 [Gemini](https://aistudio.google.com/app/apikey) Key 和额度**。所以：部署一次，多少人用都行，各用各的存储和额度，**对部署者零成本**。

## 🚀 三步部署（GitHub Pages）

1. 新建仓库（如 `ai-reader`），上传 `index.html`、`LICENSE`、`.nojekyll`。
2. **Settings → Pages → Source** 选 `Deploy from a branch` → `main` + `/ (root)`，保存。
3. 等一两分钟，得到网址 `https://<用户名>.github.io/ai-reader/`，把链接发出去即可。

同学完全不用碰 GitHub，打开链接就能用。每个人唯一的一次性步骤：在 **⚙ 设置** 里贴自己的免费 Gemini Key。

## 🔑 第一次使用

打开 **⚙ 设置** → 去 [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey) 免费拿一个 Key → 粘贴。Key 只存本机浏览器。推荐模型 `gemini-2.5-flash-lite`（免费额度最高）。

> 不想部署？也可以直接双击 `index.html`，但 Chrome 下本地文件会被禁用存储，要保留记忆请用 Firefox，或在文件夹里跑 `python -m http.server`。

## 🛠️ 技术

单个静态 HTML：原生 JS + [PDF.js](https://mozilla.github.io/pdf.js/)（CDN）+ IndexedDB + Gemini API。无需构建、无依赖、无追踪。

## 🤝 参与

欢迎提 Issue 和 PR。如果它帮你省下了几百次复制粘贴，点个 ⭐ 让更多人发现它！

## 📄 License

[MIT](LICENSE)
