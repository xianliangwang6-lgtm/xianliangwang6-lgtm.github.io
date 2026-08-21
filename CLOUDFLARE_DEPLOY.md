# ☁️ Cloudflare Pages 部署指南

Cloudflare Pages 提供全球最快的 CDN 和无限流量，完全免费！

---

## 🚀 方法1：通过网页界面（推荐）

### 步骤：

#### 1. 访问 Cloudflare Pages
```
https://pages.cloudflare.com/
```

#### 2. 登录/注册
- 如果没有账号，点击 "Sign up" 注册（免费）
- 可以使用邮箱注册
- 或者用 GitHub/Google 账号快速登录

#### 3. 创建项目
- 点击 "Create a project"
- 选择 "Connect to Git"

#### 4. 连接 GitHub
- 点击 "Connect GitHub"
- 授权 Cloudflare 访问你的 GitHub
- 选择仓库：`xianliangwang6-lgtm/xianliangwang6-lgtm.github.io`

#### 5. 配置构建设置
```
Project name: smart-text-reader (或你喜欢的名字)
Production branch: main
Build command: (留空)
Build output directory: /
Root directory: /
```

#### 6. 点击 "Save and Deploy"

#### 7. 等待部署完成
- 通常需要 1-2 分钟
- 部署成功后会显示网址

#### 8. 获得网址
你会得到两个域名：
```
https://smart-text-reader.pages.dev
https://smart-text-reader-xxx.pages.dev (预览域名)
```

访问：
```
https://smart-text-reader.pages.dev/reader.html
```

---

## 🎯 方法2：使用 Wrangler CLI

### 前提条件
- 安装 Node.js
- 有 Cloudflare 账号

### 步骤：

```bash
# 1. 安装 Wrangler
npm install -g wrangler

# 2. 登录 Cloudflare
wrangler login

# 3. 创建 Pages 项目
wrangler pages project create smart-text-reader

# 4. 部署
wrangler pages deploy . --project-name=smart-text-reader

# 完成！
```

---

## 📊 部署后的功能

### ✅ 你将获得：

1. **超快速度**
   - 全球 300+ 数据中心
   - 自动选择最近的服务器
   - 世界最快的 CDN

2. **无限流量**
   - 没有带宽限制
   - 没有请求次数限制
   - 完全免费

3. **自动部署**
   - 每次 `git push` 自动更新
   - 预览每个 PR 的效果
   - 回滚到任何历史版本

4. **安全功能**
   - 自动 HTTPS
   - DDoS 防护
   - Web 应用防火墙（可选）

5. **自定义域名**
   - 免费绑定你的域名
   - 自动 SSL 证书
   - 支持多个域名

---

## 🔗 重要链接

**Cloudflare Pages 控制台**：
```
https://dash.cloudflare.com/?to=/:account/pages
```

**文档**：
```
https://developers.cloudflare.com/pages/
```

---

## 🎨 自定义域名设置

### 如果你有自己的域名：

1. 在 Cloudflare Pages 项目设置中
2. 点击 "Custom domains"
3. 点击 "Set up a custom domain"
4. 输入你的域名（例如：reader.yourdomain.com）
5. 按照提示添加 DNS 记录：
   ```
   CNAME  reader  smart-text-reader.pages.dev
   ```
6. 等待 DNS 生效（通常几分钟）
7. 完成！

---

## 📈 性能优化

### 已配置的优化：

✅ **缓存策略**（`_headers` 文件）
- HTML: 1小时缓存
- 静态资源: 1年缓存

✅ **安全头部**
- X-Frame-Options
- X-Content-Type-Options
- CSP (Content Security Policy)

✅ **路由优化**（`_redirects` 文件）
- `/reader` 重定向到 `/reader.html`

---

## 🔄 自动部署流程

部署完成后，每次你：
1. 修改代码
2. `git commit`
3. `git push`

Cloudflare 会自动：
1. 检测到更新
2. 构建新版本
3. 部署到全球
4. 清除缓存
5. 更新完成！

**全程自动，无需手动操作！**

---

## 📱 预览部署

每个 Pull Request 都会自动创建预览环境：
```
https://xxx-yyy.smart-text-reader.pages.dev
```

可以在合并前测试变更！

---

## 💰 费用

**完全免费！**

免费额度：
- ✅ 无限请求
- ✅ 无限带宽
- ✅ 500 次构建/月
- ✅ 1 个并发构建

对于个人项目绰绰有余！

---

## ⚡ 速度对比

Cloudflare Pages 是世界上最快的静态托管服务：

```
全球平均响应时间：
Cloudflare Pages: ~10-30ms  ⚡⚡⚡⚡⚡
Vercel:          ~50-100ms ⚡⚡⚡⚡
Netlify:         ~60-120ms ⚡⚡⚡⚡
GitHub Pages:    ~100-200ms ⚡⚡⚡
```

---

## 🛠️ 故障排除

### 问题：部署失败
**解决**：检查 Git 仓库是否公开，或确保授权了 Cloudflare

### 问题：404 错误
**解决**：确保文件名正确，路径为 `/reader.html`

### 问题：自定义域名不工作
**解决**：等待 DNS 传播（最多 24 小时）

---

## 📞 获取帮助

- Cloudflare 文档: https://developers.cloudflare.com/pages/
- 社区论坛: https://community.cloudflare.com/
- Discord: https://discord.cloudflare.com/

---

## 🎉 下一步

部署成功后：

1. **分享你的网站**
   ```
   https://smart-text-reader.pages.dev/reader.html
   ```

2. **绑定自定义域名**（可选）

3. **设置网站分析**（免费）
   - Cloudflare Web Analytics
   - 隐私友好，无需 Cookie

4. **启用更多功能**
   - Cloudflare Workers（边缘计算）
   - Cloudflare Images（图片优化）
   - Cloudflare Stream（视频）

---

**提示**：部署完成后记得测试所有功能，确保朗读器工作正常！🎤
