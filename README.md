# ARRIVE ON TIME - Sports Matchmaking Web App

一个现代化的运动约球网站界面，使用响应式设计，支持多种运动项目匹配。

## 功能特点

- 🎨 现代化UI设计
- 📱 完全响应式布局，支持所有设备
- 🎯 支持多种运动项目选择
- ✨ 流畅的动画效果
- 🌈 清晰的视觉反馈

## 项目结构

```
arrive-on-time-web/
├── css/
│   └── style.css          # 主样式文件
├── images/
│   └── sports/            # 运动图标
│       ├── basketball.svg
│       ├── football.svg
│       ├── running.svg
│       ├── swimming.svg
│       ├── table-tennis.svg
│       └── volleyball.svg
├── select-sport.html      # 运动选择页面
└── README.md             # 项目说明文档
```

## 技术栈

- HTML5
- CSS3
- Tailwind CSS
- Font Awesome
- 现代 JavaScript (ES6+)

## 快速开始

1. 克隆项目到本地：
```bash
git clone [你的仓库URL]
```

2. 打开项目目录：
```bash
cd arrive-on-time-web
```

3. 使用本地服务器运行项目（任选其一）：
   - 使用 Python：
     ```bash
     python -m http.server 8000
     ```
   - 使用 Node.js 的 http-server：
     ```bash
     npx http-server
     ```
   - 使用 Visual Studio Code 的 Live Server 插件

4. 在浏览器中访问：
   - 如果使用 Python：访问 `http://localhost:8000`
   - 如果使用 http-server：访问 `http://localhost:8080`
   - 如果使用 Live Server：会自动打开默认浏览器

## 设计特点

1. 响应式布局
   - 桌面端：每行3-4个运动卡片
   - 平板端：每行2-3个运动卡片
   - 移动端：每行1-2个运动卡片

2. 交互设计
   - 卡片悬停效果
   - 选中状态视觉反馈
   - 平滑过渡动画

3. 可访问性
   - 语义化HTML结构
   - 适当的颜色对比度
   - 清晰的视觉层级

## 自定义修改

### 添加新的运动项目

1. 在 `images/sports/` 目录下添加新的SVG图标
2. 在 `select-sport.html` 中添加新的卡片：

```html
<div class="sport-card">
    <img src="images/sports/your-sport.svg" alt="Sport Name" class="sport-icon">
    <h3 class="sport-title">Sport Name</h3>
    <p class="sport-subtitle">Sport Description</p>
</div>
```

### 修改颜色主题

在 `css/style.css` 中修改以下变量：

```css
.button-primary {
    background: #22c55e; /* 主色调 */
}

.sport-card.selected {
    background-color: #dcfce7; /* 选中状态背景色 */
    border: 2px solid #22c55e; /* 选中状态边框色 */
}
```

## 贡献指南

1. Fork 这个项目
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的改动 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

## 许可证

MIT License - 详见 LICENSE 文件 