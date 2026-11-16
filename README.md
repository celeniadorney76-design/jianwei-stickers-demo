# Jianwei Stickers · 免安装书签脚本实验 v0.2

面向 ChatGPT Plus / Free 等网页用户的单表情渲染验证。不是完整插件，也不能修改 ChatGPT 官方 Android App。

## 为什么有这个实验

GitHub Pages 演示图片在手机浏览器可直接打开，但 ChatGPT Android App 的外部图片嵌入实验未通过。为了避免用户安装其他软件，我们先测试 **Android Chrome 的 bookmarklet（书签脚本）**。

## 快速使用

1. 打开 https://celeniadorney76-design.github.io/jianwei-stickers-demo/
2. 复制书签脚本，并按网页指示保存成 Chrome 的书签 URL。
3. 在 Chrome 网页版 chatgpt.com 打开对话。
4. 地址栏键入「见微表情」，点**带书签图标的联想结果**来运行脚本。
5. 请助手输出 `[JW_HAPPY]`，观察是否被替换为图片。

## 技术原理与隐私

脚本扫描 DOM 属性 `[data-message-author-role="assistant"]` 之下的文本节点，找到 `[JW_HAPPY]` 并替换成本地 DOM 中的 `img` 元素。MutationObserver 监听新回复。刷新页面需重新运行。此脚本无 API 请求上传聊天内容，仅浏览器直接加载图片 URL。GitHub Pages 会接收到普通的图片请求（例如网络地址）。

仅修改当前网页显示，不更改实际消息。不是原生贴纸发送。如果 ChatGPT 更改网页结构，选择器可能失效。

## 文件

- `bookmarklet.js` — 可读的核心 JavaScript 代码（网站模拟测试自动运行）
- `bookmarklet.txt` — 可复制的完整 `javascript:` 书签网址
- `index.html` — 手机版试验说明和模拟助手消息
- `stickers/jw_happy.png` — 演示缩略图
- `stickers.json` — 表情索引

## 版权

本项目代码按仓库 LICENSE（MIT）授权；见微演示图及角色形象不包含在 MIT 代码授权中。完整私人角色包不会上传这里。

## 进度

- [x] GitHub Pages 已部署
- [x] 演示图可在手机浏览器打开
- [ ] 安卓 Chrome 书签脚本在 ChatGPT 页面实测
- [ ] 支持多表情及用户自定义表情包
- [ ] 长期稳定的一键安装方案
