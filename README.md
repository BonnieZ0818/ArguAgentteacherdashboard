# ArguAgent — Teacher Dashboard Preview

全英文界面原型，可直接通过 GitHub Pages 发布，无需安装依赖或执行构建。

## 文件

- `index.html`：完整网页入口，包括样式、示例数据及交互。
- `.nojekyll`：让 GitHub Pages 直接发布静态文件。

## 上传和上线

1. 新建 GitHub 仓库。
2. 将本文件夹内的文件上传至仓库根目录。确保 `index.html` 直接位于根目录，而非多套一层文件夹。
3. 进入仓库的 **Settings → Pages**。
4. 在 **Build and deployment** 中选择 **Deploy from a branch**。
5. 选择 **main** 和 **/(root)**，点击 **Save**。
6. 等待部署完成，打开 Pages 页面显示的网址。

GitHub 官方说明：https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 功能

- 切换 With / Without AI summary。
- 切换 During / After。
- 横向小组卡片与所选小组的作答区。
- 弹窗阅读讨论、initial answers 和 final answers；支持切换小组。
- 标记原话并写教师备注。
- 两种条件共享原始材料及标记功能；AI 总结仅在有 AI 条件出现。

## 使用范围

这是固定虚构数据的设计演示，不是真实 AI 服务，不会自动回放学生消息。
网页没有服务器、参与者数据库或研究日志收集功能。不要把界面内的标记功能视为研究数据提交。

导出保留了沙盒 iframe 与 Content Security Policy。浏览器支持时，导出层使用本地状态回退；请勿依赖本地浏览器状态作为数据备份。

## 修改

`index.html` 是保留沙盒的打包版本。若需调整设计，建议修改原始可视化片段后重新导出，而非直接改写 iframe 的编码内容。
