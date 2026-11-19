# Pocket Kit · 小工具箱

这是浸月的独立 iPhone 小工具箱（PWA）项目，和个人主页分开维护。

## 在线地址

启用 GitHub Pages 后，访问：
https://jin66yue-arch.github.io/toolbox/

## 功能

- 待办清单
- 目标倒计时
- 随手记
- 文本统计与整理
- 本地数据导出
- PWA 安装与离线缓存

## 文件结构

```text
toolbox/
├── index.html
├── manifest.json
├── sw.js
├── icons/
│   └── icon.svg
└── README.md
```

## 使用说明

- 使用静态 HTML、CSS 和 JavaScript，无需构建步骤。
- 任务、笔记和倒计时保存在当前浏览器的本地存储中，不会自动同步到其他设备。
- 清除浏览器网站数据或更换设备，可能导致本地数据丢失；重要内容请使用导出功能备份。
- 首次在线打开后，Service Worker 会缓存应用资源，以便后续离线访问。
- 如果更新后仍显示旧版本，可尝试刷新页面；缓存版本可在 `sw.js` 中调整。
