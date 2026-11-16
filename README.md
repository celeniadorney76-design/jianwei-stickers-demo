# Jianwei Stickers · Public Demo 0.1

手机优先的 ChatGPT 表情调用技术验证项目。当前**只有一张低分辨率演示表情**，不是完整角色包或已完成的插件。

## 测试目标

1. 通过 GitHub Pages 给演示图片提供固定 HTTPS 地址。
2. 检查 ChatGPT Android App 能否读取指定公开图片网址。
3. 区分“网络图片能被搜索并展示”和“助手能主动从自建图库发指定表情”。

**上述第 2、3 项尚待验证；请勿将其宣传为已实现的主动表情功能。**

## 文件

- `index.html` — 手机适配的单图实验网页
- `stickers/jw_happy.png` — 64×64 演示缩略图
- `stickers.json` — 表情 ID 和资源索引

## 开启 GitHub Pages

在仓库 Settings → Pages → Build and deployment 中选 Deploy from a branch、main、/(root)，保存即可。

仓库需要公开才能通过公共 GitHub Pages 面向所有用户访问（免费计划）。只要发布成功，网页预计路径：

`https://celeniadorney76-design.github.io/jianwei-stickers-demo/`

图片路径：

`https://celeniadorney76-design.github.io/jianwei-stickers-demo/stickers/jw_happy.png`

**这两个地址在 Pages 正式启用之前都不可视为已上线。**

## 开源与素材

代码按 MIT 许可发布。见微演示图、角色形象及未来角色包**不包含在 MIT 授权范围内**；完整私人资源包不会加入本仓库。任何其他用户可以自行导入自己的角色资源。

本仓库不会存储聊天记录，不需要 API Key。
