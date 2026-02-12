叙事医学与 NEI 网络：临床科普交互平台 🩺

“最好的科普，是让患者重新听懂自己身体的告白。”

这是一个面向临床医生的单页面交互式 Web 应用 (SPA)，旨在通过叙事医学的视角，重构传统的医学科普范式。项目利用 NEI（神经-内分泌-免疫）网络理论，将晦涩的生理机制转化为可交互、直观的数字体验，帮助医生更有效地开展患教工作。

🌟 核心特性

范式重构对比 (Paradigm Shifter)：通过 A/B 测试式的交互，直观展示“传统宣教”与“叙事沟通”在临床语境下的思维差异。

NEI 实时模拟器 (Bio-Dashboard)：用户可模拟点击不同的情绪状态（焦虑 vs 喜悦），实时观察 IL-6、IgA、NK 细胞等生理指标的动态变化。

循证数据可视化 (Evidence Lab)：基于 Chart.js 驱动的动态图表，量化展示应激状态下的感冒风险及 C 型性格的健康代价。

身体症状解码 (Somatic Map)：交互式器官网格，解读肠脑轴、呼吸系统与皮肤系统背后的心理叙事逻辑。

响应式设计：完美适配桌面、平板与移动端，确保医生在诊室或移动端均能流畅演示。

🛠️ 技术栈

Frontend: HTML5, Tailwind CSS (CDN)

Visualization: Chart.js (Canvas-based)

Icons: FontAwesome 6.4.0

Typography: Google Fonts (Noto Serif SC, Noto Sans SC)

Logic: Vanilla JavaScript (ES6+)

📂 项目结构

├── clinical_narrative_dashboard.html  # 核心单页面应用
└── README.md                          # 项目说明文档


🚀 快速开始

该项目为单文件绿色版，无需安装任何依赖或构建流程：

克隆或下载 clinical_narrative_dashboard.html 文件。

在任意现代浏览器（Chrome, Edge, Safari）中直接打开。

点击导航栏或滑动滚轮开始探索科普章节。

🔬 医学背景

本项目基于以下前沿医学理念：

叙事医学 (Narrative Medicine)：由 Rita Charon 教授提出，强调医生运用叙事能力来实践医学。

神经-内分泌-免疫网络 (NEI Network)：现代生理学核心理论，证明了心理应激与生理指标之间的双向调节关系。

进化医学 (Evolutionary Medicine)：探讨现代社会压力源与人类原始应激反应之间的“进化错配”。

🤝 贡献指南

我们欢迎临床医生和前端开发者提出建议：

提交 Issue 反馈在临床宣教中遇到的常见痛点。

Fork 本仓库并提交 PR 以丰富“身体地图”中的症状解读维度。

📄 许可证

本项目采用 MIT License 开源。

免责声明：本平台所展示的数据源自临床统计学研究，旨在辅助科普演示，不应直接替代针对具体患者的专业诊断。建议在医生指导下结合临床实际情况使用。
