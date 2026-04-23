# Source Map

调研日期：2026-04-23。

需要有来源依据时读这个文件。来源可信度排序：官方平台/标准文档 > 产品设计系统 > 成熟 UX 研究 > 专业美术/设计教育 > 当前 SEO 或创作者运营文章。

## UI 与通用视觉设计

- Apple Human Interface Guidelines：Layout 强调视觉层级、阅读顺序、对齐、间距、适配、安全区和平台显示限制；Typography 强调可读性、层级、字重和可缩放文本；Color 强调语义一致、足够对比、明暗/高对比环境测试，以及不要只靠颜色传达含义。
  来源：https://developer.apple.com/design/human-interface-guidelines/layout, https://developer.apple.com/design/human-interface-guidelines/typography, https://developer.apple.com/design/human-interface-guidelines/color

- Material Design / Android Material 3：适合借鉴语义色彩角色、字体层级角色、可访问的色调系统和组件主题一致性。旧版 Material layout 仍适合作为基础版式原则：用字体、栅格、空间、尺度、色彩和图像建立层级。
  来源：https://developer.android.com/develop/ui/compose/designsystems/material3, https://m1.material.io/layout/principles.html, https://m1.material.io/style/color.html, https://m1.material.io/style/typography.html

- NN/g 视觉设计原则：scale、visual hierarchy、balance、contrast、Gestalt 能同时提升美观和可用性。NN/g 十大启发式可补充一致性、系统状态可见、识别优于记忆、审美且极简等判断。
  来源：https://www.nngroup.com/articles/principles-visual-design/, https://www.nngroup.com/articles/ten-usability-heuristics/

- WCAG 2.2：普通文本对比度 4.5:1，大号文本 3:1，重要非文本 UI 线索 3:1；颜色不能是唯一信息载体；文本应能放大到 200% 且不丢失内容或功能。
  来源：https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html, https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html, https://www.w3.org/WAI/WCAG22/Understanding/use-of-color.html, https://www.w3.org/WAI/WCAG22/Understanding/resize-text.html

## 小红书设计与图文笔记

- 小红书 RPDC 52 Design Principles 是小红书产品设计中心的官方设计原则集合。对新手尤其有用：对比、对齐、一致性、邻近、图底关系、均质连接、信噪比、成本-效益。
  来源：https://rpdc.xiaohongshu.com/52-design-principles/about, https://rpdc.xiaohongshu.com/52-design-principles/contrast, https://rpdc.xiaohongshu.com/52-design-principles/alignment, https://rpdc.xiaohongshu.com/52-design-principles/consistency, https://rpdc.xiaohongshu.com/52-design-principles/proximity, https://rpdc.xiaohongshu.com/52-design-principles/figure-ground, https://rpdc.xiaohongshu.com/52-design-principles/signal-to-noise-ratio

- 小红书图文经验资料：3:4 竖版封面通常占据信息流面积更大；方图适合商品网格；封面字要短、高对比、缩略图可读；轮播比例保持一致；避免二维码、联系方式、外站水印、重复图、引起不适的首图。具体尺寸、上传上限和审核规则变化快，最终交付前以 App 或创作后台为准。
  来源：https://www.gzjy100.com/uploads/20230923/e9f6dd9a17b0396fe24c4611ab86bce5.pdf, https://www.huasheng.ai/insights/xiaohongshu-image-design/, https://www.10100.com/article/32618408

## 海报与社交图

- 高质量海报/社交图通常只有一个主意图，层级明显，字体数量受控，对比强，有相关图片或图形钩子，并保留足够留白。教育类案例反复说明：可以极简，也可以复杂，但观众必须快速理解主题。
  来源：https://www.canva.com/learn/poster-design/, https://www.nngroup.com/articles/principles-visual-design/

## 游戏 CG 与 Key Art

- 游戏 UI/HUD 必须在移动、复杂背景中保持可读。Xbox Accessibility Guideline 102 明确点名 HUD、文本、小地图、瞄准图标和高对比模式的对比度问题。
  来源：https://learn.microsoft.com/en-us/gaming/accessibility/xbox-accessibility-guidelines/102

- Steam 图形资产有严格内容规则：基础 capsules 仅限游戏美术、游戏名和官方副标题；Library Hero 应只有美术图；capsule 必须尺寸准确且产品 logo/name 可读。导出前必须回到 Steamworks 核对最新尺寸。
  来源：https://partner.steamgames.com/doc/store/assets/rules, https://partner.steamgames.com/doc/store/assets/standard%20?language=english

- 概念设计/key art 教育资料集中强调：焦点、故事清晰度、明度分组、光线、镜头/透视、空间深度、剪影和快速可读性。这些是工艺启发，不是平台政策。
  来源：https://www.cgmasteracademy.com/courses/93-composition-for-concept-art-and-illustration.html, https://www.creativebloq.com/3d/how-compose-and-create-dramatic-key-art-81412639, https://nvalchev.artstation.com/blog/7oYNO/the-power-of-composition-how-to-guide-a-player-s-eye-through-your-environment

## AI 图像指导

- Text-to-image prompt 研究指出，结构化加入 subject 与 style 关键词能减少盲目试错并提高结果稳定性。生产使用时，还应补充构图、镜头、光线、色板、材质、平台裁切和负面约束。
  来源：https://arxiv.org/abs/2109.06977
