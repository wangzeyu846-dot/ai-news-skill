# 智能资讯助手落地页

React + TypeScript + Vite，本地展示项目，无后端、无实时采集。

## 运行

```sh
pnpm install
pnpm dev
pnpm build
```

默认预览地址由 Vite 启动输出提供。

## 内容

历史试跑示例来自 2026-10-12 已核验简报，仅公开内容节选，无私人飞书链接。产品来源：https://github.com/wangzeyu846-dot/ai-news-skill 。

GSAP：首屏编排、滚动流程与内容入场，useGSAP 和 matchMedia 负责清理与响应式降级。原生 CSS 设计系统；本页面采用黑色商务主题，以冷灰面板与蓝色重点建立内容层级。React Bits CountUp 为独立数字组件，来自实时官方 registry；组件原始许可证见 https://github.com/DavidHDev/react-bits 。

设计参数：DESIGN_VARIANCE 7 / MOTION_INTENSITY 8 / VISUAL_DENSITY 4。层级：普通内容 0，纸面叠层 1，导航 20，跳转主内容链接 30。

页面文案以产品价值、简报成果、资讯范围和质量标准为主，不出现执行平台品牌；公共新闻来源中的名称保留原意。
