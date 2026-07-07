# 🚀 部署指南：将选号助手部署到 GitHub Pages

## 方法一：手动部署（推荐，最简单）

### 第一步：创建 GitHub 仓库
1. 登录 [GitHub](https://github.com)，点击右上角 **"+"** → **"New repository"**
2. 仓库名填写：`lottery-assistant`
3. 选 **Public**（GitHub Pages 免费版需要公开仓库）
4. 不要勾选 "Add a README"（我们已有文件）
5. 点 **"Create repository"**

### 第二步：上传文件
1. 在仓库页面点击 **"uploading an existing file"** 链接
2. 把以下 **3个文件** 拖拽上传：
   - `index.html`（选号助手主文件）
   - `README.md`
   - `.nojekyll`（空文件，确保 GitHub Pages 正常渲染）
3. 提交信息写：`Initial commit`
4. 点 **"Commit changes"**

### 第三步：开启 GitHub Pages
1. 仓库页面 → 点 **"Settings"** 标签
2. 左侧菜单 → **"Pages"**
3. **Source** 选 **"Deploy from a branch"**
4. **Branch** 选 **"master"**（或"main"）→ 文件夹选 **"/ (root)"**
5. 点 **"Save"**
6. 等待约 1-2 分钟，页面会显示：
   > Your site is live at https://你的用户名.github.io/lottery-assistant/

### 第四步：iPhone 添加到主屏幕
1. Safari 打开上面的网址
2. 点底部分享按钮 → **"添加到主屏幕"**
3. 输入名称 → 添加
4. 桌面出现图标 ✅

---

## 方法二：用 GitHub Desktop（电脑操作更方便）

1. 下载安装 [GitHub Desktop](https://desktop.github.com/)
2. 登录你的 GitHub 账号
3. 点 **"Create a New Repository on your Hard Drive..."**
4. 把 `lottery-deploy` 文件夹里的文件全部拖进去
5. 写 commit 信息 → 点 **"Commit to master"**
6. 点右上角 **"Publish branch"**
7. 回到 GitHub 网页 → Settings → Pages → 开启 GitHub Pages

---

## 🔑 如需更新文件
- 修改后重新上传 `index.html` 到仓库即可
- GitHub Pages 会自动更新（约 1 分钟生效）

## 🔒 密码说明
- 默认密码：**123456**
- 如需修改密码：用文本编辑器打开 `index.html`
- 搜索 `const PASSWORD = '123456'`，把 `123456` 改成你想要的新密码
- 保存后重新上传即可

## ⚠️ 注意事项
- GitHub Pages 网址是公开的，但选号助手**不收集任何个人信息**
- 所有数据（开奖记录、推荐号码）只存在你手机浏览器本地
- 清除浏览器缓存会清空数据，建议定期用"导出数据"功能备份
