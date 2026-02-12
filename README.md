# 叙事医学与NEI网络：临床科普交互平台

<div align="center">

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?logo=chartdotjs&logoColor=white)

**从"治疗疾病"到"关怀全人"的临床沟通范式重构**

[在线演示](#) | [功能特性](#功能特性) | [快速开始](#快速开始) | [技术架构](#技术架构)

</div>

---

## 📖 项目简介

这是一个面向医疗从业者的**交互式科普教育平台**,旨在帮助医生理解并应用**叙事医学**理念,通过可视化的方式展示**神经-内分泌-免疫(NEI)网络**如何连接情绪与生理健康。

### 核心理念

- **打破知识赤字误区**: 从单向宣教转向双向共情沟通
- **可视化NEI机制**: 将抽象的生物学概念转化为直观的交互体验
- **循证医学支撑**: 基于真实临床数据展示情绪对健康的量化影响
- **实践行动指南**: 提供可落地的医患沟通改进路径

---

## ✨ 功能特性

### 🔄 临床沟通范式对比器

**交互式标签切换**,直观对比传统宣教模式与叙事沟通模式的差异:

- **传统模式**: 单向知识传递、高位指令式、依从性差
- **叙事模式**: 意义共建、探讨心理背景、激活自愈力

### 🧠 NEI网络实时模拟器

**核心交互功能** - 点击情绪按钮,实时观察生理指标变化:

- **积极情绪**: IL-6降低、IgA增加、NK细胞活性增强
- **负面情绪**: 炎症因子升高、免疫屏障受损、疼痛敏感度增加
- **动态视觉反馈**: 卡片颜色、图标、数值同步变化

### 📊 循证数据可视化

基于**Chart.js**的专业图表展示:

- **感冒风险柱状图**: 不同情绪状态下的发病率对比
- **C型性格风险环形图**: 长期情绪抑制与肿瘤风险的关联

### 🗺️ 身体情绪地图

**可展开的器官系统卡片**,解读症状背后的心理叙事:

- **消化系统**: 肠脑轴反馈机制
- **呼吸系统**: 压抑情绪的生理隐喻
- **皮肤系统**: 边界冲突的免疫表达

### 🛤️ 医生品牌打造路线图

**垂直时间轴设计**,展示从理论到实践的四步行动路径。

---

## 🚀 快速开始

### 前置要求

- 现代浏览器(Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- 无需本地服务器或构建工具

### 安装与运行

```bash
# 1. 克隆仓库
git clone https://github.com/your-username/narrative-medicine-platform.git

# 2. 进入项目目录
cd narrative-medicine-platform

# 3. 直接在浏览器中打开 index.html
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

**或者使用本地服务器(推荐)**:

```bash
# 使用 Python 3
python -m http.server 8000

# 使用 Node.js (需要安装 http-server)
npx http-server -p 8000
```

然后访问 `http://localhost:8000`

---

## 🏗️ 技术架构

### 技术栈

| 技术 | 版本 | 用途 |
|------|------|------|
| **HTML5** | - | 语义化结构 |
| **Tailwind CSS** | 3.x (CDN) | 响应式样式系统 |
| **Chart.js** | 4.x (CDN) | 数据可视化 |
| **Font Awesome** | 6.4.0 | 图标库 |
| **Google Fonts** | - | Noto Sans/Serif SC |

### 设计原则

- **零依赖构建**: 纯前端实现,无需编译步骤
- **CDN加速**: 所有外部资源通过CDN加载,确保快速访问
- **渐进增强**: 核心内容在禁用JavaScript时仍可访问
- **移动优先**: 完全响应式设计,适配各种屏幕尺寸

### 文件结构

```
narrative-medicine-platform/
│
├── index.html          # 主应用文件(单文件架构)
├── README.md           # 项目文档
└── LICENSE             # 开源协议
```

---

## 🎨 设计系统

### 色彩方案

```css
/* 主色调 - 医疗专业感 */
--primary-blue: #004a7c;      /* 深蓝 - 信任与专业 */
--healing-green: #20c997;     /* 疗愈绿 - 积极与康复 */
--alert-red: #dc3545;         /* 警示红 - 风险与警觉 */
--ivory-white: #fbfaf3;       /* 象牙白 - 温暖背景 */
```

### 交互模式

- **标签切换**: 范式对比器使用状态管理
- **按钮触发**: NEI模拟器通过点击事件更新DOM
- **悬停展开**: 症状地图卡片支持点击切换显示
- **平滑滚动**: 导航栏锚点跳转带动画效果

---

## 📱 响应式设计

| 断点 | 屏幕宽度 | 布局调整 |
|------|----------|----------|
| **Mobile** | < 768px | 单列布局,汉堡菜单 |
| **Tablet** | 768px - 1024px | 双列网格,折叠导航 |
| **Desktop** | > 1024px | 三列网格,完整导航 |

---

## 🔧 自定义配置

### 修改配色

在 `<style>` 标签中更新CSS变量:

```css
body {
    background-color: #your-color; /* 修改背景色 */
}
```

### 调整图表数据

在 `<script>` 标签中找到Chart.js配置:

```javascript
data: {
    labels: ['标签1', '标签2'],
    datasets: [{
        data: [25, 45], // 修改数据点
        backgroundColor: ['#color1', '#color2']
    }]
}
```

### 添加新的症状卡片

在"身体情绪地图"部分复制现有卡片结构:

```html
<div class="group p-8 hover:bg-gray-50 transition cursor-pointer" 
     onclick="toggleSymptom('new-system')">
    <!-- 卡片内容 -->
</div>
```

---

## 🤝 贡献指南

我们欢迎各种形式的贡献!

### 贡献方式

1. **Fork** 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 **Pull Request**

### 代码规范

- 使用语义化的HTML标签
- 遵循Tailwind CSS的实用类命名约定
- JavaScript使用ES6+语法
- 添加必要的注释说明复杂逻辑

---

## 📄 许可证

本项目采用 **MIT License** 开源协议 - 详见 [LICENSE](LICENSE) 文件

---

## 🙏 致谢

- **叙事医学理论**: 感谢Rita Charon教授的开创性工作
- **NEI网络研究**: 基于神经免疫学领域的前沿研究成果
- **开源社区**: Tailwind CSS、Chart.js、Font Awesome团队

---

## 📞 联系方式

- **问题反馈**: [GitHub Issues](https://github.com/your-username/narrative-medicine-platform/issues)
- **功能建议**: [GitHub Discussions](https://github.com/your-username/narrative-medicine-platform/discussions)

---

<div align="center">

**"最好的科普,是让患者重新听懂自己身体的告白。"**

Made with ❤️ for Healthcare Professionals

</div>
