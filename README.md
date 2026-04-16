# Zerobyheart - 个人作品集

> 一个面向面试的个人作品集网站，采用 Awwwards 风格设计

## 🌐 在线演示

[zerobyheart.netlify.app](https://zerobyheart.netlify.app)

## ✨ 特性

- **高级设计感**：低饱和度 Glassmorphism 风格，暗黑/明亮双模式
- **3D 动效交互**：Three.js 粒子星云背景 + GSAP 高级滚动动画
- **响应式设计**：移动端自适应，性能优化
- **项目展示**：交互式项目卡片，详情 Modal 弹窗
- **SEO 优化**：完整的 Meta 标签和 Open Graph 支持

## 🛠️ 技术栈

- **前端框架**：原生 HTML/CSS/JavaScript
- **样式**：Tailwind CSS
- **3D 渲染**：Three.js
- **动画**：GSAP + ScrollTrigger
- **字体**：Inter (Google Fonts)
- **部署**：Netlify

## 🚀 本地运行

```bash
# 克隆项目
git clone https://github.com/zerobyheart/portfolio.git
cd portfolio

# 直接用 Live Server 打开 index.html
# 或使用任意静态文件服务器
npx serve .
```

## 📁 项目结构

```
.
├── index.html          # 主页面
├── images/             # 项目截图
│   ├── AI 简历助手.PNG
│   └── 个人网站.PNG
├── .gitignore
└── README.md
```

## 🎨 设计亮点

### 视觉效果
- 低饱和度 Stone 色系，避免高饱和色彩
- Glassmorphism 毛玻璃效果
- Noise 纹理叠加增加质感
- 渐变文字和微妙的边框发光

### 交互体验
- 自定义光标（圆点 + 圆环）
- 磁性按钮涟漪效果
- 滚动进度条
- 返回顶部按钮
- 移动端汉堡菜单

### 性能优化
- Three.js 移动端降级（300 vs 800 粒子）
- Resize 事件节流
-  prefers-reduced-motion 支持

## 📊 Lighthouse 评分

目标：Performance 90+, Accessibility 90+, Best Practices 90+

## 📝 更新日志

- **v1.0.0** - 初始版本
  - 完整的个人作品展示
  - Two.js 3D 背景
  - GSAP 滚动动画
  - Dark/Light 双模式

## 📄 License

MIT

---

**Made with ❤️ by Zerobyheart**
