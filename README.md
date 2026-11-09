# 在厦大的一周 · XMUM 生活模拟器

本游戏由ChatGPT 6.1Sol-Light生成，已整理为可直接发布的 GitHub Pages 版本。游戏、3D引擎、样式、场景、手机与合成音乐均在 `index.html` 内，无需安装依赖或运行构建命令。

## 文件

- `index.html`：完整游戏，入口必须保持这个小写文件名。
- `.nojekyll`：让 Pages 按静态文件发布。
- `LICENSE-THREE.txt`：内嵌 Three.js 的 MIT 许可；HTML中也保留了声明。
- `README.md`：本说明。

只上传这四个文件。不要上传原来的整个工作目录、浏览器存档 JSON 或其他私人文件。游戏包含你描述的校园与宿舍生活设定；选择公开仓库后，游戏内容和代码都可被他人查看。此包不包含真实姓名或你的浏览器游玩记录。

## 第一次上传：只用网页操作

建议用电脑浏览器完成，手机后续直接打开游戏链接即可。

### 1. 下载并解压

解压 `XMUM-GitHub-Pages上传包.zip`。进入解压后的文件夹，找到 `index.html` 等四个文件。上传的是文件本身，不是ZIP，也不是外层文件夹。

### 2. 新建仓库

1. 登录 https://github.com 。没有账号先注册，并验证邮箱。
2. 打开 https://github.com/new 。
3. Owner 选自己的账号，Repository name 填 `xmum-life`。
4. Visibility 选 **Public**。按 GitHub 当前文档，免费个人账号的 Pages 使用公开仓库；这是公开发布游戏。
5. 勾选 **Add a README file**（新界面可能显示 Add README → On），其他项目保留默认。
6. 点 **Create repository**。

### 3. 上传文件

1. 仓库的 **Code** 页面，点击 **Add file → Upload files**。
2. 将解压得到的四个文件拖入上传框，或点击 **choose your files** 选择文件。
3. 文件清单里应直接显示 `index.html`，不能是 `XMUM-GitHub-Pages/index.html`。外层文件夹不要一起拖进去。
4. 同名 README 会更新为本说明，属于正常情况。
5. Commit message 可填写 `Upload XMUM game`。
6. 选择提交到 `main`（**Commit directly to the main branch**），点 **Commit changes**。有些界面还会再弹确认框，再确认提交即可。
7. 回到仓库文件列表，检查最外层可以看到 `index.html`。

如果新建的是空仓库、没有 Add file 按钮，可点击页面中 **uploading an existing file** 进入上传页。

### 4. 开启 GitHub Pages

1. 点击仓库上方的 **Settings**。这是仓库设置，不是头像菜单里的账号设置。
2. 左侧找到 **Pages**。
3. 找到 **Build and deployment**。
4. **Source** 选择 **Deploy from a branch**。
5. **Branch** 选择 **main**。
6. 旁边的文件夹选择 **/ (root)**。
7. 点击 **Save**。

不需要填写 Custom domain，不需要购买域名，不需要选择自定义 GitHub Actions 工作流。

### 5. 获取并打开游戏链接

等待首次部署完成，刷新 **Settings → Pages**。页面出现 **Your site is live at ...** 或 **Visit site** 时，打开它提供的地址。

普通项目仓库的链接格式通常是：

`https://你的GitHub用户名.github.io/xmum-life/`

这是格式示例，请复制 Pages 页面实际给出的地址，不要照抄中文占位符。仓库如果用了别的名字，地址最后一段也会不同。

仓库地址 `github.com/用户名/xmum-life` 是代码页；直接点击仓库里的 index.html 也只会看见源代码。真正游玩请打开 **Pages 的 github.io 链接**。

### 6. 检查后分享

打开游戏 → 开始一天 → 做一点活动 → 退出页面 → 用同一浏览器重新打开同一链接 → 点“继续上次的生活”。确认正常后，把 Pages 链接发给家人。

## 以后如何更新

拿到新版后，在同一个仓库的 **Add file → Upload files** 上传新的 `index.html`，保留文件名和位置，提交即可。Pages 会重新部署，不必再创建仓库。部署完成后刷新网页；电脑可用 Ctrl+F5 强制刷新。

同一浏览器、同一 Pages 地址的兼容存档会保留。首次从原私人试玩站或离线文件换到 GitHub Pages，需要先在旧版暂停菜单→存档与备份复制文本，再到新网址导入。不同网址、不同设备和不同浏览器不会自动同步；清理浏览器数据也可能清掉存档。

## 常见问题

- **上传ZIP后没有游戏：** GitHub不会自动把上传的ZIP解压成网站。先在电脑解压，再上传里面的文件。
- **打开后显示代码：** 你打开了仓库的代码页。到 Settings → Pages 点 Visit site。
- **404：** 等待部署结束，检查 Source=Deploy from a branch、Branch=main、Folder=/(root)，并确认最外层是小写 index.html。不要用 dist 文件夹或其他外层目录套住它。
- **Pages没有main可选：** 先提交游戏文件，让main分支存在，再回到设置。
- **部署失败：** 打开仓库 Actions，查看 pages-build-deployment 的结果。若账号邮箱尚未验证，先完成验证。仓库的组织策略或权限限制需按页面提示处理。
- **存档没跟过来：** 旧地址与新地址是不同网站，需要导出/导入。不要把存档JSON提交到公开仓库。
- **大陆网络打不开或慢：** 此包没有运行时外部依赖，但GitHub Pages本身的可达性仍取决于网络。未验证其在中国大陆各运营商的稳定性；若不稳定，同一个index.html也可以改放国内静态托管。

## 当前玩法

电脑 WASD 移动、E 互动；手机用触屏摇杆。靠近建筑可互动，不需要进特定圆圈。长辈友好模式可按“继续生活”前进。一天约五分钟，一周七天；每日重玩会清空当天及之后的记录，并先提示后果。

手机包含微信快捷回复、父母与外婆一起视频、外卖、音乐、通知和备忘录。可中断任务保留部分进度；取外卖后能选择是否继续原活动。论文相关时间含会议每周最多14小时。游戏指标仅为模拟。

## 官方操作参考

- 创建 Pages：https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- 设置发布分支：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- 网页上传文件：https://docs.github.com/en/repositories/working-with-files/managing-files/adding-a-file-to-a-repository

说明核对日期：2026年11月10日。GitHub界面与套餐可能变化，以平台当前页面为准。
