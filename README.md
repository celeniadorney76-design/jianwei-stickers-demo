# 见微表情档案馆 · Jianwei Stickers

这是已部署在 GitHub Pages 的公开表情图库，任何人都可以通过网页浏览和复制链接，无需安装、账号或自行部署。

**图库：** https://celeniadorney76-design.github.io/jianwei-stickers-demo/
**AI 索引：** https://celeniadorney76-design.github.io/jianwei-stickers-demo/stickers.json

## 使用方式
- 打开首页，按关键词、来源、情绪筛选。可点击原图，选择保存，或尝试复制图片到系统剪贴板。
- 某些移动浏览器不支持“复制图片”，此时会退回复制图片直链。
- 支持访问公开网址的 AI 可读取 `stickers.json`，通过 `label`、`mood`、`tags` 选择表情，从 `url` 获取原图地址。
- AI 能读取索引 **不等于** 每个聊天客户端都允许直接显示该图片；这取决于平台。

## JSON 结构
`stickers.json` 包含 `schema`、`version`、`homepage` 和 `stickers` 数组。
每个条目包含稳定 `id`、`label`、`category`、`mood`、`tags`、`description`、`file`、完整 `url`、`license`、`source` 和 `attribution`。
新增图片后往数组增加一条即可；请保持 ID 唯一，尽量不修改既有图片直链。

## 授权
站点使用已有的 `stickers/jw_happy.png` 演示图，以及 12 张从 [Twemoji](https://github.com/jdecked/twemoji) 提取的原始 SVG。
Twemoji 图像使用 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)，详情见 [ATTRIBUTION.md](./ATTRIBUTION.md)。
**见微演示图没有获得公开再利用许可，且不在 Twemoji 授权范围。**
原仓库 MIT LICENSE 仅适用于代码，不代表所有图片都可商业使用。请勿无授权批量搬运他人的表情包。

## 原实验保留
- [安卓网页书签脚本 v0.2](./legacy-bookmarklet.html)
- [PNG/GIF 直链加载测试](./media-test.html)

本网站是纯静态资源展示，不修改 ChatGPT 安卓 App 或其他聊天软件。
