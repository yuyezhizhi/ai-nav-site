# AI 导航站点

一个简洁、酷炫的 AI 工具导航网站，纯静态页面，无需后端。

## 🚀 快速开始

### 本地预览

**方式一：直接打开**
```bash
cd ai-nav-site
open index.html
# 或双击 index.html 文件
```

**方式二：使用 Python 服务器**
```bash
cd ai-nav-site
python3 -m http.server 8080
# 访问 http://localhost:8080
```

**方式三：使用 VS Code Live Server**
- 安装 Live Server 扩展
- 右键 index.html → "Open with Live Server"

## 📁 项目结构

```
ai-nav-site/
├── index.html      # 主页面（所有代码都在这一个文件里）
├── tools.json      # AI 工具数据
├── update_tools.py # 数据更新脚本
└── README.md       # 说明文档
```

## ✨ 功能特性

- 🎨 **酷炫界面** - 暗色主题 + 毛玻璃效果 + 渐变动画
- 🔍 **实时搜索** - 输入即搜索，快速找到工具
- 📂 **分类筛选** - 按类别浏览（对话、图像、视频、编程等）
- 🔥 **热门推荐** - 置顶展示最热门的 AI 工具
- 📱 **响应式设计** - 完美支持手机、平板、电脑
- ⚡ **纯静态** - 无需后端，直接部署

## 🎯 工具分类

| 分类 | 图标 | 说明 |
|------|------|------|
| 对话助手 | 🤖 | ChatGPT、Claude 等 AI 对话工具 |
| 图像生成 | 🎨 | Midjourney、Stable Diffusion 等 |
| 视频制作 | 🎬 | Runway、Pika 等 AI 视频工具 |
| 音频处理 | 🎵 | Suno、ElevenLabs 等 |
| 编程开发 | 💻 | GitHub Copilot、Cursor 等 |
| 办公效率 | 📊 | Gamma、Notion AI 等 |
| AI 搜索 | 🔍 | Perplexity 等 AI 搜索引擎 |
| 学习教育 | 📚 | Duolingo 等 AI 学习工具 |

## 🔧 数据管理

### 手动添加工具

编辑 `tools.json` 文件，添加新的工具条目：

```json
{
  "name": "工具名称",
  "url": "https://example.com",
  "category": "chatbot",
  "description": "工具描述",
  "icon": "🤖",
  "hot": false,
  "tags": ["标签1", "标签2"]
}
```

### 自动更新

```bash
python3 update_tools.py
```

## 🚀 部署

### Vercel

```bash
npm i -g vercel
cd ai-nav-site
vercel
```

### GitHub Pages

1. 将 `index.html` 和 `tools.json` 推送到 GitHub 仓库
2. 进入 Settings → Pages
3. 选择 Source: main branch

### Netlify

直接拖拽 `ai-nav-site` 文件夹到 Netlify 部署区域。

### 任意静态托管

只需要两个文件：
- `index.html`
- `tools.json`

## 📈 后续计划

- [ ] 添加更多 AI 工具
- [ ] 增加工具评分功能
- [ ] 添加工具对比功能
- [ ] 支持用户提交新工具
- [ ] 添加每日推荐

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

## 📄 License

MIT License
