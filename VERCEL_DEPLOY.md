# 🚀 Vercel 部署指南

## 方法1：一键导入（最简单，推荐）

### 步骤：

1. **点击下面的按钮直接部署**：

   [![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/xianliangwang6-lgtm/xianliangwang6-lgtm.github.io)

2. **或者访问**：
   ```
   https://vercel.com/new/clone?repository-url=https://github.com/xianliangwang6-lgtm/xianliangwang6-lgtm.github.io
   ```

3. **登录 Vercel**（如果还没有账号，用 GitHub 账号快速注册）

4. **点击 "Deploy"** 按钮

5. **等待部署完成**（通常30秒-1分钟）

6. **获得网址**，例如：
   ```
   https://your-project-name.vercel.app/reader.html
   ```

---

## 方法2：通过 Vercel 网站导入

### 步骤：

1. **访问** [vercel.com](https://vercel.com)

2. **登录账号**（可以用 GitHub 账号登录）

3. **点击 "New Project"** 或 "Add New..." → "Project"

4. **导入 Git 仓库**：
   - 选择 "Import Git Repository"
   - 找到并选择 `xianliangwang6-lgtm/xianliangwang6-lgtm.github.io`
   - 点击 "Import"

5. **配置项目**（保持默认即可）：
   - Project Name: 可以自定义
   - Framework Preset: Other
   - Root Directory: ./
   - Build Command: (留空)
   - Output Directory: (留空)

6. **点击 "Deploy"**

7. **等待部署完成**

8. **访问你的网站**：
   ```
   https://[你的项目名].vercel.app/reader.html
   ```

---

## 方法3：使用 Vercel CLI（开发者方式）

### 前提：安装 Node.js

### 步骤：

```bash
# 1. 安装 Vercel CLI
npm install -g vercel

# 2. 登录
vercel login

# 3. 在项目目录运行
cd /path/to/your/project
vercel

# 4. 按照提示操作
# - Set up and deploy? Yes
# - Which scope? (选择你的账号)
# - Link to existing project? No
# - What's your project's name? (输入项目名或回车使用默认)
# - In which directory is your code located? ./
# - Want to override the settings? No

# 5. 部署完成后会显示网址
```

---

## 🎉 部署后

部署成功后，你会获得两个网址：

1. **主域名**：`https://your-project.vercel.app`
2. **朗读器页面**：`https://your-project.vercel.app/reader.html`

### 功能：

✅ 自动 HTTPS  
✅ 全球 CDN 加速  
✅ 每次 git push 自动部署  
✅ 免费使用  
✅ 自定义域名（可选）  

---

## 📝 自定义域名（可选）

如果你有自己的域名：

1. 进入 Vercel 项目设置
2. 点击 "Domains"
3. 添加你的域名
4. 按照提示设置 DNS 记录
5. 完成！

---

## ⚡ 常见问题

**Q: 部署需要多久？**  
A: 通常 30 秒到 1 分钟

**Q: 是否免费？**  
A: 个人项目完全免费，有每月带宽限制（100GB，足够使用）

**Q: 如何更新网站？**  
A: 直接 git push 到 main 分支，Vercel 会自动重新部署

**Q: 可以删除吗？**  
A: 可以，在 Vercel 项目设置中点击 "Delete Project"

---

## 🆘 需要帮助？

- Vercel 文档: https://vercel.com/docs
- Vercel 支持: https://vercel.com/support

---

**提示**: 部署完成后，记得把网址分享出来！🎉
