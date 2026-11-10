# 扩展隐私政策

这个仓库集中维护多个浏览器扩展的隐私页面。每个扩展使用独立且稳定的产品编号（AppId），不会覆盖其他扩展的页面。

## 现有页面

- [留白 · 网站屏蔽](https://sudieszoka.github.io/privacy/meng_liubai_ppd/)：`docs/meng_liubai_ppd/index.html`

## 添加其他扩展

1. 为新扩展确定独立 AppId，并保存在该扩展的 `manifest.json` 的 `author` 字段中。
2. 根据该扩展真实的数据处理行为编写隐私政策，保存到 `docs/<AppId>/index.html`。
3. 在 `docs/index.html` 中添加对应入口。
4. 提交后验证 `https://sudieszoka.github.io/privacy/<AppId>/` 可公开访问，并核对内容。

GitHub Pages 的发布来源为 `main` 分支的 `/docs`。仅保存公开的隐私页面，不上传扩展源码、用户数据、Token、SDK 密钥或带个人配置的技能目录。

开发者联系邮箱：hzaulpl@gmail.com
