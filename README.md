# 微信公众号文章工具集 | WeChat Article Skills

[English](#english) | [中文](#chinese)

---

<div id="chinese"></div>

## 📖 项目简介

一套强大的微信公众号文章Skills工具集，涵盖 **AI写作助手（技术/产品视角）**、**文章格式化** 和 **草稿发布** 四大核心功能。帮助你高效地创作、美化和发布微信公众号文章。

## ✨ 核心工具

### 1️⃣ WeChat Product Manager Writer - AI 产品经理写作助手
从 AI 产品经理视角撰写文章。涵盖 AI 产品拆解、场景解决方案、效率提升实战、产品方法论、行业观察。

**核心特性：**
- 🤖 产品思维驱动写作
- 📊 强制生成内容结构图（信息图）
- 🎨 强制生成专业文章封面
- 🎯 实战场景导向，非纯技术教程

[📚 详细文档](./wechat-product-manager-writer/SKILL.md)

---

### 2️⃣ WeChat Tech Writer - AI 技术写作助手
基于 AI 的智能技术文章写作工具，快速生成高质量技术内容。

**核心特性：**
- 🤖 AI 辅助写作
- 📊 技术文章优化
- 🎯 SEO 关键词优化
- 📱 移动端阅读优化

[📚 详细文档](./wechat-tech-writer/SKILL.md)

---

### 3️⃣ WeChat Article Formatter - 文章格式化工具
将 Markdown 文章转换为适合微信公众号的美化 HTML，一键生成专业排版。

**核心特性：**
- 📝 完整支持 Markdown 语法
- 🎨 三套精美主题（科技风、简约风、商务风）
- 💅 专业样式，完美适配微信公众号
- 🌈 多语言代码高亮
- ⚡ 支持批量转换
- 👀 实时预览功能

[📚 详细文档](./wechat-article-formatter/README.md)

---

### 4️⃣ WeChat Draft Publisher - 草稿发布工具
自动将 HTML 格式的文章推送到微信公众号草稿箱。

**核心特性：**
- ✅ 自动获取和缓存 access_token
- ✅ 支持上传封面图片
- ✅ 智能错误处理和重试
- ✅ 命令行 + 交互式双模式
- ✅ 完整的日志输出

[📚 详细文档](./wechat-draft-publisher/README.md)

---

## 🚀 快速开始

### 克隆到你的/.Claude/skills

```bash
# 克隆项目
git clone <repository-url>
复制三个文件夹到你的/.Claude/skills目录下
cd 任意目录，启动Claude code，输入“/skills” 查看是否加载成功

```

### 典型工作流程

**全流程一句话搞定**
```bash
帮我写一篇介绍 Claude code 的文章，并且进行格式美化，然后推送到微信公众号后台
```

---

## 📂 项目结构

```
wechat_article_skills/
├── wechat-article-formatter/   # Markdown 转 HTML 工具
│   ├── scripts/                 # 转换脚本
│   ├── templates/               # CSS 主题模板
│   ├── references/              # 参考文档
│   └── README.md
│
├── wechat-draft-publisher/      # 草稿发布工具
│   ├── publisher.py             # 核心发布脚本
│   ├── config.json.example      # 配置模板
│   └── README.md
│
├── wechat-tech-writer/          # AI 写作助手
│   ├── scripts/                 # 写作脚本
│   ├── references/              # 参考资料
├── wechat-product-manager-writer/ # AI 产品经理写作助手
│   ├── scripts/                 # 绘图与生成脚本
│   ├── references/              # 风格与封面指南
│   └── SKILL.md
│
└── README.md                    # 本文件
```

---

## 💡 使用场景

### 技术博客作者
- 使用 **WeChat Tech Writer** AI 辅助生成技术内容
- 使用 **Article Formatter** 的 tech 主题美化排版
- 使用 **Draft Publisher** 一键发布

### 内容运营者
- 使用 **Article Formatter** 批量转换历史文章
- 使用 minimal 或 business 主题适配不同风格
- 自动化发布流程，提升效率

### 自媒体创作者
- 在 Markdown 中专注写作
- 一键转换为精美排版
- 快速发布到公众号

---

## 📋 系统要求

- **Python**: 3.6+
- **操作系统**: Windows / macOS / Linux
- **浏览器**: Chrome / Edge（用于预览）
- **微信公众号**: 认证的服务号或订阅号（用于 API 发布）

---

## 🔧 配置说明

### WeChat Draft Publisher 配置

创建配置文件 `~/.wechat-publisher/config.json`：

```json
{
  "appid": "wx1234567890abcdef",
  "appsecret": "your_appsecret_here"
}
```

**获取 AppID 和 AppSecret：**
1. 登录 [微信公众平台](https://mp.weixin.qq.com)
2. 进入"设置与开发" → "基本配置"
3. 查看开发者 ID 和密码

---

## 📚 文档资源

### 各工具详细文档
- [WeChat Article Formatter 完整指南](./wechat-article-formatter/README.md)
- [WeChat Draft Publisher 使用说明](./wechat-draft-publisher/README.md)
- [WeChat Tech Writer 技能文档](./wechat-tech-writer/SKILL.md)
- [WeChat Product Manager Writer 技能文档](./wechat-product-manager-writer/SKILL.md)

### 参考资料
- [微信公众平台帮助中心](https://kf.qq.com/product/weixinmp.html)
- [Markdown 语法指南](https://www.markdownguide.org/)

---

## 📝 示例文章

使用本工具集创作和发布的精选文章：

### 技术文章示例

1. **[Claude Code 零基础指南：不会写代码也能做开发？看这一篇就够了，效率翻倍！](https://mp.weixin.qq.com/s/Dx-XYcj74c2LdZOWwNS7GQ)**  

2. **[从70分钟到9分钟：微信公众号自动化Skills！提效狂魔！](https://mp.weixin.qq.com/s/iBKgEX_vfYNIe90qPi03Sw)**  

3. **[从 Chat 到 Agent：Claude Agent SDK 才是 AI 真正的生产力开关](https://mp.weixin.qq.com/s/58nZuLJGNjm6hqfGzJg-ZA)**  

4. **[Claude Skill：为什么它会取代 Dify、n8n 和 Coze？](https://mp.weixin.qq.com/s/rXl4nLI6ouJMIMfvL1iSbQ)**  

> 💡 **提示**：以上文章均使用本项目工具完成排版和发布，欢迎参考学习！

---

## 📱 关注公众号

扫描下方二维码关注我的微信公众号，获取更多优质内容：

![公众号二维码](./qrcodes/公众号.png)
> 👆 **关注公众号** - 第一时间获取最新文章和工具更新

---

## 🤝 关于作者

### 联系方式

#### 添加个人微信
扫描下方二维码添加作者微信，交流使用心得：

![个人微信二维码](./qrcodes/personal_wechat.png)
> 👆 **添加微信** - 疑问解答、技术交流，拉你入群

---

#### 加入技术交流群
扫描下方二维码加入微信群，与更多开发者交流：

![群聊二维码](./qrcodes/group_wechat.png)
> 👆 **加入群聊** - 技术讨论、问题解答、交流讨论

---

#### 赞赏支持
如果这个项目对你有帮助，欢迎赞赏支持：

![赞赏二维码](./qrcodes/appreciation.png)
> 👆 **赞赏支持** - 您的支持是我最大的动力

---

## ⚠️ 注意事项

1. **API 调用限制**
   - access_token 每日获取次数有限（2000次/天）
   - 本工具自动缓存 token，请勿频繁重置

2. **图片使用规范**
   - 微信不支持本地图片，需重新上传
   - 封面图片建议尺寸：900x500 像素
   - 图片大小不超过 2MB

3. **样式兼容性**
   - 微信编辑器对 CSS 支持有限
   - 部分高级样式可能无法显示
   - 建议使用工具提供的标准主题

---

## 🐛 故障排除

### 常见问题

**Q: 粘贴后样式丢失？**
- 使用 Chrome 或 Edge 浏览器
- 尝试全选复制而非部分复制

**Q: access_token 获取失败？**
- 检查 AppID 和 AppSecret 是否正确
- 确认公众号已认证
- 检查 IP 白名单配置

更多问题请查看各工具的详细文档或提交 Issue。

---

## 📝 更新日志

### v2.0.0 (2026-01-16)
- 🚀 新增 `WeChat Product Manager Writer` (AI 产品经理写作助手)
- 🎨 支持强制生成内容结构图与专业封面
- 📂 重构项目结构，支持四大核心功能
- 🐛 修复了一些渲染问题
- 🐛 修复了微信公众号兼容性问题

### v1.0.0 (2025-12-28)
- ✅ 发布三个核心工具
- ✅ 完善文档体系
- ✅ 优化用户体验

---

## 📄 许可证

MIT License - 供个人和商业使用

---

## 🙏 致谢

感谢以下开源项目：
- [Python-Markdown](https://python-markdown.github.io/)
- [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/)
- [Requests](https://requests.readthedocs.io/)

---

**祝你使用愉快！** 🎉

如有问题或建议，欢迎通过上方二维码联系我！

---
---

<div id="english"></div>

# WeChat Article Skills

## 📖 Project Overview

A powerful WeChat Official Account Skills toolkit, featuring **AI Writing Assistant (Tech/Product)**, **Article Formatting**, and **Draft Publishing**. Streamline your WeChat content creation workflow with four core tools.

## ✨ Core Tools

### 1️⃣ WeChat Product Manager Writer - AI PM Assistant
Write from an AI Product Manager's perspective. Covers product teardowns, scenario solutions, efficiency boosts, methodology, and industry trends.

**Key Features:**
- 🤖 Product-thinking driven writing
- 📊 Mandatory infographics/structure maps
- 🎨 Professional cover image generation
- 🎯 Scenario-oriented practical insights

[📚 Documentation](./wechat-product-manager-writer/SKILL.md)

---

### 2️⃣ WeChat Tech Writer - AI Writing Assistant
AI-powered technical writing assistant for creating high-quality tech content.

**Key Features:**
- 🤖 AI-assisted writing
- 📊 Technical content optimization
- 🎯 SEO keyword optimization
- 📱 Mobile reading optimization

[📚 Documentation](./wechat-tech-writer/SKILL.md)

---

### 3️⃣ WeChat Article Formatter
Convert Markdown articles to beautifully formatted HTML optimized for WeChat Official Accounts.

**Key Features:**
- 📝 Full Markdown syntax support
- 🎨 Three premium themes (Tech, Minimal, Business)
- 💅 Professional styling for WeChat
- 🌈 Multi-language syntax highlighting
- ⚡ Batch conversion support
- 👀 Real-time preview

[📚 Documentation](./wechat-article-formatter/README.md)

---

### 4️⃣ WeChat Draft Publisher
Automatically publish HTML articles to your WeChat Official Account draft box.

**Key Features:**
- ✅ Auto access_token management
- ✅ Cover image upload support
- ✅ Smart error handling & retry
- ✅ CLI + Interactive modes
- ✅ Complete logging

[📚 Documentation](./wechat-draft-publisher/README.md)

---

## 🚀 Quick Start

### Clone to your /.Claude/skills

```bash
# Clone the repository
git clone <repository-url>
cd wechat_article_skills

# Install Python dependencies
pip install -r requirements.txt  # if needed
```

### Typical Workflow

**One-sentence workflow**
```bash
Help me write an article about Claude Code, format it beautifully, and publish it to my WeChat Official Account backend
```

---

## 📂 Project Structure

```
wechat_article_skills/
├── wechat-article-formatter/   # Markdown to HTML converter
│   ├── scripts/                 # Conversion scripts
│   ├── templates/               # CSS theme templates
│   ├── references/              # Documentation
│   └── README.md
│
├── wechat-draft-publisher/      # Draft publishing tool
│   ├── publisher.py             # Core publishing script
│   ├── config.json.example      # Configuration template
│   └── README.md
│
├── wechat-tech-writer/          # AI writing assistant
│   ├── scripts/                 # Writing scripts
│   ├── references/              # Reference materials
├── wechat-product-manager-writer/ # AI PM writing assistant
│   ├── scripts/                 # Image generation scripts
│   ├── references/              # Style & cover guides
│   └── SKILL.md
│
└── README.md                    # This file
```

---

## 💡 Use Cases

### Tech Bloggers
- Use **WeChat Tech Writer** for AI-assisted content creation
- Use **Article Formatter** with tech theme for professional styling
- Use **Draft Publisher** for one-click publishing

### Content Operators
- Use **Article Formatter** for batch converting articles
- Choose themes based on content style
- Automate publishing workflow

### Media Creators
- Focus on writing in Markdown
- One-click conversion to beautiful layouts
- Quick publishing to WeChat

---

## 📋 System Requirements

- **Python**: 3.6+
- **OS**: Windows / macOS / Linux
- **Browser**: Chrome / Edge (for preview)
- **WeChat Account**: Verified Service or Subscription Account (for API publishing)

---

## 🔧 Configuration

### WeChat Draft Publisher Setup

Create config file at `~/.wechat-publisher/config.json`:

```json
{
  "appid": "wx1234567890abcdef",
  "appsecret": "your_appsecret_here"
}
```

**Get AppID and AppSecret:**
1. Login to [WeChat Official Accounts Platform](https://mp.weixin.qq.com)
2. Go to "Settings & Development" → "Basic Configuration"
3. Find Developer ID and Secret

---

## 📚 Documentation

### Tool-Specific Guides
- [WeChat Article Formatter Complete Guide](./wechat-article-formatter/README.md)
- [WeChat Draft Publisher User Guide](./wechat-draft-publisher/README.md)
- [WeChat Tech Writer Skill Documentation](./wechat-tech-writer/SKILL.md)
- [WeChat Product Manager Writer Skill Documentation](./wechat-product-manager-writer/SKILL.md)

### External Resources
- [WeChat Official Accounts Help Center](https://kf.qq.com/product/weixinmp.html)
- [Markdown Guide](https://www.markdownguide.org/)

---

## 📝 Example Articles

Featured articles created and published using this toolkit:

### Technical Article Examples

1. **[Claude Code Beginner's Guide: Can You Develop Without Coding? This Guide Has You Covered, Double Your Efficiency!](https://mp.weixin.qq.com/s/Dx-XYcj74c2LdZOWwNS7GQ)**  

2. **[From 70 Minutes to 9 Minutes: WeChat Official Account Automation Skills! Efficiency Booster!](https://mp.weixin.qq.com/s/iBKgEX_vfYNIe90qPi03Sw)**  

3. **[From Chat to Agent: Why Claude Agent SDK is the Real Productivity Switch for AI](https://mp.weixin.qq.com/s/58nZuLJGNjm6hqfGzJg-ZA)**  

4. **[Claude Skill: Why Will It Replace Dify, n8n, and Coze?](https://mp.weixin.qq.com/s/rXl4nLI6ouJMIMfvL1iSbQ)**

> 💡 **Tip**: All articles above were formatted and published using this toolkit. Feel free to reference them!

---

## 📱 Follow Official Account

Scan the QR code below to follow my WeChat Official Account for more quality content:

![Official Account QR Code](./qrcodes/公众号.png)
> 👆 **Follow Account** - Get the latest articles and tool updates

---

## 🤝 About the Author

### Contact

#### Add Personal WeChat
Scan the QR code below to connect with the author:

![Personal WeChat QR Code](./qrcodes/personal_wechat.png)
> 👆 **Add WeChat** - One-on-one communication

---

#### Join Community Group
Scan to join our WeChat group for discussions:

![Group WeChat QR Code](./qrcodes/group_wechat.png)
> 👆 **Join Group** - Tech discussions, Q&A, and community exchange

---

#### Support This Project
If this project helps you, consider buying me a coffee:

![Appreciation QR Code](./qrcodes/appreciation.png)
> 👆 **Appreciate** - Your support motivates me

---

## ⚠️ Important Notes

1. **API Rate Limits**
   - access_token has daily request limits (2000/day)
   - This tool auto-caches tokens to minimize requests

2. **Image Guidelines**
   - WeChat doesn't support local images
   - Recommended cover size: 900x500 pixels
   - Image size limit: 2MB

3. **Style Compatibility**
   - WeChat editor has limited CSS support
   - Some advanced styles may not render
   - Use provided themes for best results

---

## 🐛 Troubleshooting

### Common Issues

**Q: Styles lost after pasting?**
- Use Chrome or Edge browser
- Try selecting and copying all content

**Q: access_token fetch failed?**
- Verify AppID and AppSecret
- Ensure account is verified
- Check IP whitelist settings

For more issues, check tool-specific documentation or submit an Issue.

---

## 📝 Changelog

### v2.0.0 (2026-01-16)
- 🚀 Added `WeChat Product Manager Writer` (AI PM perspective)
- 🎨 Mandatory infographic and professional cover generation
- 📂 Refactored structure to support four core tools
- 🐛 Fixed rendering issues
- 🐛 Fixed WeChat Official Account compatibility bugs

### v1.0.0 (2025-12-28)
- ✅ Released three core tools
- ✅ Complete documentation
- ✅ Optimized user experience

---

## 📄 License

MIT License - Free for personal and commercial use

---

## 🙏 Acknowledgments

Thanks to these open-source projects:
- [Python-Markdown](https://python-markdown.github.io/)
- [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/)
- [Requests](https://requests.readthedocs.io/)

---

**Happy Writing!** 🎉

Feel free to contact me via QR codes above for questions or suggestions!

