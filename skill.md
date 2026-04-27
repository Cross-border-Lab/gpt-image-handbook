# 反推提示词 Skill Prompt

## 任务说明

这是你的图；请你反推提示词；保证你给出的提示词；使用你的模型能达到 **90%以上** 的场景+内容的还原度。

**输出双版本提示词：**
1. **复杂提示词（高还原度）** - 详细的专业提示词，包含所有技术参数和细节描述，适合追求高质量效果的用户
2. **简化版提示词（快速上手）** - 用自然语言对话的方式总结复杂提示词的核心内容。**关键原则：保留主题身份、核心视觉元素、必要文字信息，确保生成结果具有可识别性**

使用 **Markdown层级 + 句子描述 = 最强组合** 的标准化格式输出。

---

## 分析框架

请按照以下维度系统性分析图片，然后生成结构化提示词：

### 1. 风格定位 (Style)
- 艺术风格类型（写实摄影/插画/3D渲染/手绘等）
- 细分风格特征（水彩/油画/扁平/赛博朋克/动漫等）
- 质感描述（笔触/纹理/材质）

### 2. 构图分析 (Composition)
- 画面布局（对称/三分法/中心构图/黄金分割）
- 视角选择（俯视/平视/仰视/特写/全景）
- 景深效果（浅景深/深景深/焦点位置）
- 空间层次（前景/中景/背景）

### 3. 色彩系统 (Color)
- 主色调（暖色/冷色/中性色）
- 配色方案（互补色/类似色/单色系）
- 色彩饱和度（高饱和/低饱和/柔和/鲜艳）
- 色调氛围（明亮/暗沉/复古/清新）

### 4. 光影效果 (Lighting)
- 光源类型（自然光/人工光/环境光）
- 光线方向（顶光/侧光/逆光/正面光）
- 光线质感（柔和/强烈/漫射/聚光）
- 阴影处理（硬阴影/软阴影/戏剧性阴影）

### 5. 主体内容 (Subject)
- 核心主体描述（人物/物品/场景）
- 主体状态（动作/姿态/表情）
- 主体细节（服装/道具/装饰）
- 主体位置（画面中的具体位置）

### 6. 场景环境 (Environment)
- 场景类型（室内/室外/抽象空间）
- 环境细节（背景元素/装饰物/氛围道具）
- 时间设定（白天/夜晚/黄昏/季节）
- 地点特征（城市/自然/虚构空间）

### 7. 技术参数 (Technical)
- 画面比例（1:1/16:9/3:4/9:16）
- 分辨率要求（高清/超清/4K）
- 镜头参数（焦距/光圈/景深）
- 后期效果（滤镜/调色/特效）

### 8. 文字元素 (Text) **【关键维度】**
- 文字内容（具体文字/标题/标签）
- 文字位置（顶部/中央/底部/角落）
- 字体风格（粗体/细体/手写/印刷体）
- 文字效果（颜色/大小/排版/对齐）

---

## 输出格式标准

使用以下 Markdown 层级结构输出提示词：

```markdown
# [图片类型] - [核心主题]

## Style / 风格
- **Art Style:** [艺术风格类型]
- **Sub-style:** [细分风格特征]
- **Texture:** [质感描述]

## Composition / 构图
- **Layout:** [画面布局方式]
- **Perspective:** [视角选择]
- **Depth of Field:** [景深效果]
- **Layers:** [空间层次描述]

## Color / 色彩
- **Color Tone:** [主色调]
- **Color Scheme:** [配色方案]
- **Saturation:** [饱和度]
- **Mood:** [色调氛围]

## Lighting / 光影
- **Light Source:** [光源类型]
- **Light Direction:** [光线方向]
- **Light Quality:** [光线质感]
- **Shadow:** [阴影处理]

## Subject / 主体
- **Main Subject:** [核心主体描述]
- **Subject State:** [主体状态]
- **Details:** [主体细节]
- **Position:** [主体位置]

## Environment / 环境
- **Scene Type:** [场景类型]
- **Environment Details:** [环境细节]
- **Time Setting:** [时间设定]
- **Location:** [地点特征]

## Technical / 技术
- **Aspect Ratio:** [画面比例]
- **Resolution:** [分辨率要求]
- **Camera Settings:** [镜头参数]
- **Post-processing:** [后期效果]

## Text / 文字（如有）
- **Text Content:** "[具体文字内容]"
- **Text Position:** [文字位置]
- **Font Style:** [字体风格]
- **Text Effects:** [文字效果]

---

## Complete Prompt / 完整提示词

### 复杂版（高还原度）

[将以上所有要素整合成一段连贯的提示词，按照从整体到细节的顺序组织。包含所有技术参数、构图细节、色调描述等专业术语，确保90%以上的还原度]

**组织顺序：**
1. 风格定位 + 整体氛围
2. 构图 + 视角 + 景深
3. 色彩系统 + 光影效果
4. 主体描述（详细）
5. 场景环境（详细）
6. 文字元素（如有，必须精确）
7. 技术参数

### 简化版（快速上手）

[用自然语言对话的方式总结复杂提示词的核心内容。就像在和朋友描述这张图一样。]

**必须保留的核心信息：**
- 主题身份（这是什么类型的图）
- 风格特征（什么风格）
- 核心视觉元素（关键的3-5个元素）
- 文字信息（如果图中有文字，必须提及）

**可以省略的信息：**
- 技术参数（镜头、光圈、分辨率等）
- 细节描述（具体的色值、精确的位置等）
- 专业术语（用通俗语言替代）

---

## Hashtags / 标签分类

`#[风格标签]` `#[场景标签]` `#[用途标签]` `#[特征标签]`

---

## Applicable Scenarios / 适用场景

- [场景1]
- [场景2]
- [场景3]
```

---

## 质量检查清单

在输出提示词前，请确认：

✅ **完整性** - 是否覆盖了所有8个分析维度？
✅ **具体性** - 描述是否足够具体，避免模糊词汇？
✅ **可复现性** - 提示词是否能让 AI 生成 90% 以上相似的图片？
✅ **结构化** - 是否使用了 Markdown 层级结构？
✅ **专业性** - 是否使用了专业术语（如 "shallow depth of field" 而不是 "模糊背景"）？
✅ **文字准确** - 如果图片中有文字，是否准确提取并标注位置？
✅ **简化版完整** - 简化版是否保留了核心识别信息（主题+风格+关键元素+文字）？

---

## 自我验证流程

生成提示词后，进行以下自我检查：

1. **核心识别测试** - 如果只看简化版提示词，能否识别出这是什么类型的图？
2. **文字完整性测试** - 如果图中有文字，简化版是否提到了？
3. **风格还原测试** - 复杂版是否包含足够的风格细节？
4. **技术参数测试** - 复杂版是否包含画面比例、分辨率等关键参数？

如果任何一项测试失败，重新优化提示词。

---

## 示例输出

### 示例 1：水彩风格儿童插画

**输入图片：** 一张水彩风格的儿童插画

**输出：**

```markdown
# Children's Book Illustration - Warm Daily Moment

## Style / 风格
- **Art Style:** Watercolor and gouache illustration
- **Sub-style:** Soft poetic children's book style
- **Texture:** Visible brush strokes, paper grain, hand-painted feel

## Composition / 构图
- **Layout:** Minimalist composition with large negative space
- **Perspective:** Eye-level view, intimate distance
- **Depth of Field:** Soft focus on background, clear foreground
- **Layers:** Two children in foreground, wall and plants in background

## Color / 色彩
- **Color Tone:** Warm tones with soft blue accents
- **Color Scheme:** Muted pastel colors
- **Saturation:** Low saturation, gentle and soothing
- **Mood:** Calm, nostalgic, tender

## Lighting / 光影
- **Light Source:** Natural daylight from window
- **Light Direction:** Soft diffused light from upper left
- **Light Quality:** Gentle, even illumination
- **Shadow:** Minimal shadows, soft edges

## Subject / 主体
- **Main Subject:** Two children sitting together on a bench
- **Subject State:** Quiet conversation, relaxed posture
- **Details:** Boy in white shirt, girl in yellow dress
- **Position:** Center-left of frame, sitting side by side

## Environment / 环境
- **Scene Type:** Indoor corner with natural elements
- **Environment Details:** Climbing plants on wall, simple furniture
- **Time Setting:** Afternoon, gentle daylight
- **Location:** Cozy home interior

## Technical / 技术
- **Aspect Ratio:** 4:3 horizontal
- **Resolution:** High detail for print quality
- **Camera Settings:** N/A (illustration)
- **Post-processing:** Watercolor texture overlay

## Text / 文字
- **Text Content:** "温柔的午后" (handwritten style on wall)
- **Text Position:** Upper right corner
- **Font Style:** Delicate handwritten Chinese characters
- **Text Effects:** Soft gray color, integrated into scene

---

## Complete Prompt / 完整提示词

### 复杂版（高还原度）

Soft poetic children's book illustration with watercolor and gouache textures. 
Clear gentle daylight with slightly brighter highlights. 
Muted pastel colors with soft blue and warm tones. 
Visible brush strokes and paper grain. 
Minimalist composition with large negative space.

Scene: Two children sitting together on a bench, talking quietly. 
Boy wearing white shirt, girl in yellow dress. 
Background shows climbing plants on cream-colored wall. 
Handwritten text "温柔的午后" in soft gray on upper right.

Atmosphere: Calm, nostalgic, tender moment of childhood friendship.

### 简化版（快速上手）

水彩儿童插画，两个孩子坐在长椅上聊天，墙上写着"温柔的午后"

---

## Hashtags / 标签分类

`#水彩插画` `#儿童绘本` `#手绘质感` `#温馨日常`

---

## Applicable Scenarios / 适用场景

- 儿童读物配图
- 亲子内容创作
- 教育材料插图
- 温馨故事配图
- 文艺公众号配图
```

### 示例 2：科幻企业封面

**输入图片：** GPT Image 2 科幻风格企业手册封面

**输出：**

```markdown
# Sci-fi Corporate Cover - GPT Image 2 Manual

[完整的8维度分析...]

### 复杂版（高还原度）

Create a vertical 3:4 ultra high-resolution sci-fi corporate presentation cover poster in hyper-realistic 3D CGI style. The scene is set inside a futuristic space station with glossy black metal architecture, chrome mechanical structures, and neon lime light strips. On the right side, a massive circular observation window reveals Earth from orbit, with a bright sunrise on the horizon casting strong cinematic backlight and lens flare into the interior.

In the foreground, a highly detailed chrome robotic arm extends from the right and interacts with a floating transparent holographic interface labeled "GPT Image 2". The interface is glass-like with neon green UI elements. Beneath it, a circular sci-fi platform with glowing neon lime rings anchors the composition.

Typography layout on the left side: "SIGMA" logo, "GPT Image 2" title, "内部推广演示手册" subtitle, slogans "想象，无界 / 创造，无限", version info, and author name. All text must be clearly readable with neon lime green accents.

### 简化版（快速上手）

GPT Image 2 科幻企业手册封面，空间站场景，机械手操作霓虹绿UI界面，地球背景，包含标题和公司信息文字

---

## Hashtags / 标签分类

`#科幻封面` `#企业设计` `#3DCGI` `#AI科技` `#空间站`

---

## Applicable Scenarios / 适用场景

- AI产品宣传封面
- 企业内部手册设计
- 科技公司品牌视觉
- 路演/PPT封面
```

---

## 使用说明

1. **输入图片** - 将需要反推的图片提供给 AI
2. **执行分析** - AI 按照 8 个维度系统性分析图片
3. **生成提示词** - 使用 Markdown 层级结构输出双版本
4. **自我验证** - 对照验证流程检查质量
5. **质量检查** - 对照检查清单确认完整性
6. **测试验证** - 使用生成的提示词测试还原度

---

## 常见问题

**Q: 简化版应该多长？**
A: 不限制字数，自然表达即可。关键是保留核心识别信息，而不是压缩字数。

**Q: 如果图中有大量文字怎么办？**
A: 复杂版必须完整列出所有文字内容和位置。简化版至少要提到"包含XXX文字"或列出关键标题。

**Q: 如何判断还原度是否达到90%？**
A: 核心标准：主题身份、风格特征、关键视觉元素、文字信息四项必须高度还原。细节差异（如光影角度、次要元素位置）可以接受。

**Q: 简化版和复杂版的区别是什么？**
A: 复杂版 = 技术参数 + 专业术语 + 所有细节；简化版 = 自然语言 + 核心要素 + 可识别性。

---

*版本：v2.0*  
*适用模型：GPT Image 2, DALL-E 3, Midjourney, Stable Diffusion*  
*更新日期：2026-04-24*
