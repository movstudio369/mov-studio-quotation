# MOV STUDIO Wedding & Proposal Quotation Tool

MOV STUDIO 内部使用的单文件报价工具，可建立 Wedding Quotation 和 Proposal Quotation。

## 功能

- 中文 / English 切换
- 客户与项目资料填写
- Wedding / Proposal package selection
- Add-on、数量、单价、自定义收费与 discount
- 自动计算 Grand Total
- Quotation preview
- Copy Quotation，适合贴到 WhatsApp
- Print / Save as PDF
- Quotation No. 自动递增
- 使用浏览器 localStorage 自动保存当前报价
- Responsive layout，适用于 iPhone、iPad、Android 和桌面浏览器

所有 CSS 和 JavaScript 都包含在 `index.html`，没有后端或外部 library。

## GitHub Pages 部署步骤

1. 登录 [GitHub](https://github.com/)，点击 **New repository**。
2. 输入 repository 名称，例如 `mov-studio-quotation`。
3. Repository visibility 选择 **Public**，然后点击 **Create repository**。
4. 在新 repository 页面点击 **Add file > Upload files**。
5. 上传本项目的 `index.html` 和 `README.md`，然后点击 **Commit changes**。
6. 打开 repository 的 **Settings > Pages**。
7. 在 **Build and deployment** 的 Source 选择 **Deploy from a branch**。
8. Branch 选择 `main`，Folder 选择 `/ (root)`，然后点击 **Save**。
9. 等待 GitHub 完成部署。页面会显示网站网址，格式通常是：

   `https://你的GitHub用户名.github.io/mov-studio-quotation/`

以后更新工具时，重新上传并覆盖 `index.html`，GitHub Pages 会自动重新部署。

## 手机与 iPad 使用

- 请使用 GitHub Pages 的 `https://` 网站网址，不要使用 Google Drive 预览。
- iPhone / iPad 建议使用 Safari；Android 建议使用 Chrome。
- Copy Quotation 会优先使用 Clipboard API；浏览器不支持时会自动尝试传统复制或显示可手动复制的文字。
- iPhone / iPad 需要 PDF 时，点击 **Print / Save as PDF**，然后在系统打印画面使用分享或存储功能保存 PDF。
- Android 可在打印画面选择 **Save as PDF**。

## 资料保存说明

报价资料保存在当前设备与浏览器的 localStorage 中，不会上传到 GitHub，也不会自动同步到其他设备。

请不要使用无痕 / Private Browsing 模式保存重要报价。清除浏览器网站资料也会删除已保存的当前报价。

## 项目文件

- `index.html`：GitHub Pages 主应用
- `README.md`：部署与使用说明
