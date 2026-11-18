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

## Google Search Console 提交指引

1. 访问 https://search.google.com/search-console/welcome ，登录自己的 Google 账号，选择右侧的 **网址前缀 (URL prefix)**。
2. 填入完整网址 `https://celeniadorney76-design.github.io/jianwei-stickers-demo/`，包括路径末尾斜线。不要选择需要验证整个 `github.io` 域名的「网域」模式。
3. 选择“HTML 标记”方式，获取专属于账号的 `<meta name="google-site-verification" content="...">`；将标签交给仓库维护者写入首页 `<head>`，并在 GitHub Pages 更新后点击「验证」。
4. 验证成功后，在「站点地图」填写 `sitemap.xml` 并提交。
5. 在「网址检查」输入主页完整网址；若未编入索引，可按官方流程测试实时网址和请求编入索引。

**注意：** 站点地图已公开，但未代替账号完成 Search Console 的所有权验证；提交也不保证被搜索收录。验证标签来自个人账号，不要事先填写假标签。确认 Google Search Console 显示“成功”后才算提交成功。


## 见微·冷脸吐槽篇（2026-11-18）

新增 6 张 AI 辅助原创表情，从本次对话中生成的高清 PNG 制作了 320×320 WebP 网页版，保留原有演示图与通用 Twemoji；并非将所有表情限定为同一种嫌弃脸风格。

- `JW_DISDAIN`：我先不评价（`stickers/jianwei/jw_meme_01.webp`）
- `JW_SAW_IT`：我看到了（`stickers/jianwei/jw_meme_02.webp`）
- `JW_LOGBOOK`：写进观察日志（`stickers/jianwei/jw_meme_03.webp`）
- `JW_OUT_OF_CATEGORY`：超出常规分类（`stickers/jianwei/jw_meme_04.webp`）
- `JW_ABSURD_BUT_POSSIBLE`：离谱但能做（`stickers/jianwei/jw_meme_05.webp`）
- `JW_BUILD_FIRST`：先做一版（`stickers/jianwei/jw_meme_06.webp`）

网页版图片用于浏览、复制和保存，原始高清 PNG 在创作对话中另存备份。允许个人非商业聊天分享；商业使用或重新打包销售需获得站点维护者授权。请注意 AI 辅助创作与本仓库 MIT 代码许可证是不同的授权事项。
