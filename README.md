# 智能朗读器 🎙️

一个功能强大的文本转语音（TTS）在线工具，支持多种声音、速度调节和实时控制。

## 🌐 在线访问

- **Vercel**: 即将部署
- **GitHub Pages**: [https://xianliangwang6-lgtm.github.io/reader.html](https://xianliangwang6-lgtm.github.io/reader.html)

## ✨ 功能特性

- 🎤 **多种声音选择** - 自动识别系统语音，支持男女声
- ⚡ **速度调节** - 0.5x 到 2.0x 灵活调整
- 🎵 **音调控制** - 自定义声音高低
- 🔊 **音量控制** - 0-100% 自由调节
- ⏯️ **完整控制** - 播放、暂停、继续、停止
- 📊 **进度显示** - 实时显示朗读进度
- ⌨️ **快捷键** - 键盘快捷键支持
- 📱 **响应式设计** - 完美支持手机和平板

## 🚀 快速开始

### 在线使用

直接访问 [reader.html](reader.html) 即可使用。

### 本地使用

1. 下载 `reader.html` 文件
2. 用浏览器打开
3. 开始使用！

## 🛠️ 技术栈

- HTML5
- CSS3
- JavaScript (ES6+)
- Web Speech API

## 📦 部署到 Vercel

### 方法1：通过 Vercel 网站（推荐）

1. 访问 [vercel.com](https://vercel.com)
2. 点击 "New Project"
3. 导入此 GitHub 仓库
4. 点击 "Deploy"
5. 完成！

### 方法2：通过 Vercel CLI

```bash
# 安装 Vercel CLI
npm install -g vercel

# 在项目目录中运行
vercel

# 按照提示完成部署
```

## 🌐 其他部署平台

### Netlify
```bash
# 拖拽部署
访问 https://app.netlify.com/drop
拖入 reader.html 文件
```

### Cloudflare Pages
1. 访问 [pages.cloudflare.com](https://pages.cloudflare.com)
2. 连接 GitHub 仓库
3. 一键部署

## 📝 使用说明

1. **输入文字** - 在文本框中输入要朗读的内容
2. **选择声音** - 从下拉菜单选择男声或女声
3. **调整参数** - 设置速度、音调、音量
4. **开始朗读** - 点击"开始朗读"按钮
5. **控制播放** - 使用暂停、继续、停止按钮

### 键盘快捷键

- `Ctrl/Cmd + Enter` - 开始朗读
- `Space` - 暂停/继续（焦点不在文本框时）
- `Esc` - 停止朗读

## 🌍 浏览器兼容性

- Chrome/Edge 33+
- Firefox 49+
- Safari 7+
- Opera 21+

## 📄 许可证

MIT License

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

---

**注意**: 此项目使用 Web Speech API，需要浏览器支持。不同操作系统和浏览器提供的语音库可能不同。
