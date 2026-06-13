# 🚀 GitHub Pages 部署指南

## 前提条件
- ✅ 已安装 Git (v2.54)
- ✅ 代码已提交到本地仓库 (74个文件)
- ✅ 你有 GitHub 账号

---

## 第一步：在 GitHub 创建仓库

1. 打开 https://github.com/new
2. **Repository name** 填：`portfolio` （或你喜欢的名字）
3. 选 **Public**（公开）
4. ❌ **不要**勾选 "Add a README file"
5. 点击 **Create repository**

---

## 第二步：推送代码到 GitHub

创建后 GitHub 会显示一个页面，找到 **"…or push an existing repository from the command line"** 这段。

在终端（你当前用的这个就行）中依次执行：

```bash
cd "D:/作品集"

# 添加远程仓库（把 YOUR_USERNAME 换成你的 GitHub 用户名）
git remote add origin https://github.com/YOUR_USERNAME/portfolio.git

# 推送代码
git branch -M main
git push -u origin main
```

> 💡 如果弹窗要求登录 GitHub，选 "Sign in with your browser"。

---

## 第三步：开启 GitHub Pages

1. 打开你的仓库页面：`https://github.com/YOUR_USERNAME/portfolio`
2. 点 **Settings** → 左侧 **Pages**
3. **Branch** 选 `main`，文件夹选 `/ (root)`，点 **Save**
4. 等待 1-2 分钟，页面会显示：
   > ✅ Your site is live at `https://YOUR_USERNAME.github.io/portfolio/`

---

## 第四步：分享到飞书

1. 复制你的链接：`https://YOUR_USERNAME.github.io/portfolio/`
2. 打开飞书，粘贴链接到消息中
3. 飞书会自动生成预览卡片
4. 面试官点击即可在浏览器中打开作品集 🎉

---

## ⚠️ 可能的问题

### 图片/视频加载不出来？
中文路径在 GitHub Pages 上偶尔有兼容问题。如果出现这种情况，告诉我，我帮你改成英文路径。

### 视频文件太大推送失败？
你的视频都在 80MB 以内，GitHub 单文件限制 100MB，应该没问题。

### 想更新内容？
修改后执行：
```bash
cd "D:/作品集"
git add -A
git commit -m "更新内容"
git push
```
GitHub Pages 会自动更新，等 1 分钟刷新即可。

---

## 你的作品集链接（推送后）
```
https://YOUR_USERNAME.github.io/portfolio/
```
