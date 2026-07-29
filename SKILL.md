---
name: hand-drawn-poster
description: 专业的手绘图文科普海报生图 Skill。接收上层业务逻辑分发或用户指定的单项知识主题/文章段落，深入理解并梳理核心干货，引入 Grill-Me 交互确认机制，结合小智 IP 机器人生成包含全量显式中文文案与丰富视觉组件的精细手绘海报 Prompt。
---

# 🎨 手绘图文海报 (Hand-Drawn Educational Infographic Poster) Skill

本 Skill 旨在指导 AI Agent **针对给定的单项知识主题/文章片段/科普要点，将其转化为一张高颜值、高信息密度、极具视觉冲击力的软萌手绘图文科普海报 (Cute Educational Infographic Poster)**。

> 💡 本 Skill 专注且极致地完成**海报从干货萃取、视觉隐喻、版式构图到精细 Prompt 的全流程高品质生成**。

---

## 🎨 视觉风格与深度知识表达原则 (Visual Style & Deep Knowledge Principles)

1. **单页高密度干货与显式文案 (High-Density Knowledge & Explicit Typography)**：
   - **拒绝泛泛装饰画**：单张海报必须精准传递 3-5 个核心干货知识点（如概念定义、对比公式/数据、系统分层、代码步骤、总结金句）。
   - **文案全量显式写入 Prompt**：生图 Prompt **必须用单引号 `'...'` 显式写入海报中需要渲染的所有具体中文文案**（包含主标题、卡片胶囊标题 `1. 2. 3.`、小吊牌标注词、对比框文本、黑板代码步骤、总结金句）。
   - **绝对禁止空洞占位符**：生图 Prompt 中绝对禁止出现 `[要点说明]`、`[隐喻场景描述]` 或 `[具体知识演绎动作]` 等抽象占位符，输出时必须全部填充为抽取的具化文案与插画描述。

2. **纯粹自洽的视觉隐喻 (Self-Consistent Visual Metaphor)**：
   - 画面保持统一、自洽的隐喻叙事（如餐馆点餐、中央总线插头、黑板教学、工厂流水线），避免在单一画面中混杂冲突的概念元素。

3. **层次化视觉组件组合 (Enriched Visual Components Stack)**：
   - 每一张海报必须显式组合 3~5 个具体的视觉组件（如圆角虚线卡片框、彩色胶囊小标题底块、挂在绳子上的手绘小吊牌挂签、圆形放大镜切割图、黑板代码切片框、红绿勾叉对比徽章、黄色手绘气泡总结框）。

4. **IP 形象与知识强联动 (IP Mascot Integration)**：
   - 海报中融入科技感手绘小机器人“小智 (Xiao Zhi)”。小智的姿态与道具必须与其处理的原文具体知识产生强烈联动（如：按压 Allow 授权按钮、用激光笔指着特定代码步骤、挥舞手绘扳手调试总线、高举数据跑腿包）。

---

## 🤝 交互工作流 (Grill-Me Execution Workflow)

Agent 在处理单张海报生成任务时，严格执行以下 4 步流程：

```
[ 步骤 1: 知识点精准萃取 ]     [ 步骤 2: 单页版式与隐喻提案 ]     [ 步骤 3: Grill-Me 交互沟通 ]     [ 步骤 4: 精细脚本与 Prompt 输出 ]
+------------------------+     +--------------------------+     +---------------------------+     +-------------------------------+
| 提取 3-5 个核心知识点、 | --> | 选定单页 5 大经典版式、   | --> | 向用户展示单页蓝图与文案  | --> | 输出包含全量中文文案与        |
| 对比数据、代码与总结   |     | 匹配组件与小智姿态       |     | 收集反馈并优化单页方案    |     | 视觉组件的精细生图 Prompt     |
+------------------------+     +--------------------------+     +---------------------------+     +-------------------------------+
```

1. **步骤 1：知识点精准萃取**：
   - 分析接收到的主题或文章段落，提取 3-5 个具体干货知识点，确保海报内容扎实、数据精准。

2. **步骤 2：单页版式与视觉隐喻提案**：
   - 匹配 5 大经典单页版式（Hero 破题版、四宫格干货版、左右分栏对比版、架构流程版、金句速查版），确定纯粹自洽的手绘隐喻场景与小智动作。

3. **步骤 3：Grill-Me 交互沟通**：
   - 向用户展示单张海报的蓝图规划，提出关键设计选项并询问偏好，收集反馈后迭代方案。
   - **必须与用户确认以下 4 大细节**：
     1. **版式与隐喻选型**：确认使用哪种版式（Hero 破题 / 四宫格 / 左右分栏对比 / 架构代码切片 / 金句速查闭环）及自洽场景隐喻。
     2. **精细文案措辞**：主标题、胶囊小标题、小吊牌标注词、对比框文本与总结金句的具体中文措辞。
     3. **视觉组件选型**：四宫格、放大镜切割、手绘弯曲指引线、小吊牌挂签、代码切片框还是气泡总结框。
     4. **小智知识演绎姿态**：小智如何用具象动作与本页干货交互（如按压 Allow 按钮、激光笔指黑板代码、挥舞扳手调试总线等）。

4. **步骤 4：输出精细脚本与双语生图 Prompt**：
   - Agent **内部以英文构建 Prompt**（英文 Prompt 生图质量更优），确认通过后输出**两个版本**：
     - **🟢 英文生图版 (Primary)**：以英文撰写的完整生图 Prompt，用于实际调用生图模型。这是**主要产物**。
     - **🔵 中文确认版 (Review)**：将英文版忠实翻译为中文，供用户审核所有画面内容、文案措辞是否准确。用户确认后，以英文版提交生图。

---

## 💡 Prompt 对比范例：劣质模糊 vs 优质高密度 (English Prompt Examples)

> 💡 Skill 内部所有提示词案例均使用英文编写（以最大化发挥生图模型效果）。仅在实际输出产物给用户时，附上中文确认版供用户审核。

### ❌ Bad Prompt Example (抽象空洞、缺失文案细节):
> `Cute Q-style hand-drawn educational infographic poster, warm off-white cream paper texture background. Top double-line bubble title '[Main Title]'. Center shows a hand-drawn metaphor scene comparing Pre-MCP and With-MCP. Some cards with key points. Xiao Zhi doing knowledge demonstration. Morandi colors, 3:4 ratio, high resolution.` *(反思：没有任何真实具体文案，全是抽象占位符！)*

### ✅ Good Prompt Example (高密度干货、全量显式文案、组件丰富):
> `Cute Q-style hand-drawn educational infographic poster, warm off-white cream paper texture background. At the top center, a double-line bubble-lettered title reads 'Goodbye "Spaghetti" Cable Nightmare: M×N vs M+N', decorated with colorful fill and hand-drawn cloud and lightbulb doodles. The layout uses a left-right split comparison with contrast bubbles: the left bubble has a yellow exclamation warning triangle and red cross badge, a capsule header '[Pre-MCP: M×N Nightmare]', showing a tangled mess of red hand-drawn wire, with 3 hanging tag labels '[Reinventing the Wheel]', '[10 Independent Plugins]', '[One Change Breaks All]'; the right bubble has a green checkmark badge, a capsule header '[With-MCP: M+N Reduction]', showing a blue hand-drawn central bus with star topology, with 3 hanging tags '[Star Bus]', '[Build Once]', '[Run Everywhere]'. A cute minimalist hand-drawn robot mascot Xiao Zhi with rounded square head, single ball-top antenna, dot eyes and dash mouth, tangled in red wires with X eyes on the left, and cheerfully waving a hand-drawn wrench to tune the blue bus on the right. At the bottom, a yellow hand-drawn speech bubble summary box reads '[MCP introduces a standard abstraction layer, reducing the dense mesh topology to a star bus!]'. Pastel Morandi color palette, soft black ink hand-drawn outlines, single-page panoramic composition, centered main subject, bottom whitespace, 3:4 ratio, high resolution, fine detail.`

---

## 📐 结构化 Prompt 公式 (English Prompt Formula)

$$\text{Prompt} = \text{[Cute Q-Style Hand-Drawn Infographic Style]} + \text{[Warm Off-White Cream Paper Texture]} + \text{[Top Center Double-Line Bubble Title 'Title Text']} + \text{[3-4 Rounded Dashed Card Frames + Pastel Pill Headers '1. Header'...]} + \text{[Visual Components: Hanging Tags 'Label' / Magnifier / Code Block / Contrast Badges]} + \text{[Self-Consistent Metaphor Scene & Xiao Zhi Action]} + \text{[Bottom Yellow Speech Bubble Summary 'Key Takeaway']} + \text{[Morandi Palette + Soft Black Ink Outlines]} + \text{[Single-Page Composition, Centered, Bottom Whitespace]} + \text{[3:4 Aspect Ratio, High Res, Fine Detail]}$$

---

## 📜 输出规范：单张海报生成脚本 (Hand-Drawn Poster Script Output Schema)

> ⚠️ **模板说明**：Prompt 生图时统一以 **🟢 英文生图版 Prompt** 为标准产物（英文生图模型理解与渲染质量更佳），并附带 **🔵 中文确认版 Prompt** 供用户审核与比对文案准确性。

```markdown
### 📊 单张海报蓝图规划 (Grill-Me 确认后完整脚本)
- **海报主题**：（填入：如 MCP 协议将集成复杂度从 M×N 降维至 M+N）
- **版式类型**：（从以下选一：Hero 破题版 / 四宫格干货版 / 左右分栏对比版 / 架构流程切片版 / 金句速查闭环版）
- **视觉风格**：Q 版软萌手绘图文科普风格 + 暖米白纸张 + 黑色软墨线 + 莫兰迪配色 + 小智 IP
- **深度知识还原**：（填入：如 ①星型总线拓扑 ②M+N降维 ③一次开发处处运行 ④告别重复造轮子）
- **视觉隐喻设定**：（填入：如 左侧乱线网 vs 右侧蓝色总线星型拓扑的对比画面）
- **小智动作与情境演绎**：（填入：如 左侧被电线缠绕打叉眼，右侧开心挥舞手绘扳手调试总线）
- **精细文案排版方案**：
  - 主标题：（填入：如 告别"意大利面"乱拉线噩梦：M×N vs M+N）
  - 胶囊小标题：（填入：如 1. Pre-MCP 噩梦 / 2. With-MCP 降维 / 3. 标准总线）
  - 悬挂小吊牌：（填入：如 重复造轮子 / 一改全崩溃 / 星型总线 / 处处运行）
  - 底部金句：（填入：如 MCP 引入标准抽象层，将网状拓扑降维为星型总线！）

---

#### 🟢 英文生图版 Prompt (实际提交生图模型的主提示词)
> `Cute Q-style hand-drawn educational infographic poster, warm off-white cream paper texture background. At the top center, a double-line bubble-lettered title reads 'Goodbye "Spaghetti" Cable Nightmare: M×N vs M+N', decorated with colorful fill and hand-drawn cloud and lightbulb doodles. The layout uses a left-right split comparison with contrast bubbles: the left bubble has a yellow exclamation warning triangle and red cross badge, a capsule header '[Pre-MCP: M×N Nightmare]', showing a tangled mess of red hand-drawn wire, with 3 hanging tag labels '[Reinventing the Wheel]', '[10 Independent Plugins]', '[One Change Breaks All]'; the right bubble has a green checkmark badge, a capsule header '[With-MCP: M+N Reduction]', showing a blue hand-drawn central bus with star topology, with 3 hanging tags '[Star Bus]', '[Build Once]', '[Run Everywhere]'. A cute minimalist hand-drawn robot mascot Xiao Zhi with rounded square head, single ball-top antenna, dot eyes and dash mouth, tangled in red wires with X eyes on the left, and cheerfully waving a hand-drawn wrench to tune the blue bus on the right. At the bottom, a yellow hand-drawn speech bubble summary box reads '[MCP introduces a standard abstraction layer, reducing the dense mesh topology to a star bus!]'. Pastel Morandi color palette, soft black ink hand-drawn outlines, single-page panoramic composition, centered main subject, bottom whitespace, 3:4 ratio, high resolution, fine detail.`

#### 🔵 中文确认版 Prompt (仅供用户确认 Prompt 文案与画面设定)
> `Q版软萌手绘图文科普海报风格，暖米白羊膏纸质感背景。顶部居中是双线手绘泡泡字大标题'告别"意大利面"乱拉线噩梦：M×N vs M+N'，带有彩色字填与手绘云朵涂鸦装饰框。画面采用左右分栏对比气泡框：左框带有黄色感叹号警告三角标与红色叉叉徽章，标有胶囊标题'[Pre-MCP: M×N 噩梦]'，画着一团杂乱缠绕的红色手绘电线网，挂着 3 个小吊牌标有'[重复造轮子]'、'[10套独立插件]'、'[一改全崩溃]'；右框带有绿色勾勾徽章，标有胶囊标题'[With-MCP: M+N 降维]'，画着蓝色手绘中央总线与星型拓扑，挂着 3 个小吊牌标有'[星型总线]'、'[一次开发]'、'[处处运行]'。可爱极简手绘小机器人小智（Xiao Zhi），具有圆角方块头、单球顶天线、黑色点点眼、一字短线嘴巴，在左侧被电线缠绕打叉眼，在右侧开心挥舞手绘扳手调试总线。底部带有黄色手绘气泡金句总结框'[MCP 引入标准抽象层，将密密麻麻的网状拓扑降维为星型总线！]'。莫兰迪粉彩配色，黑色软墨水手绘勾线，单页海报全景构图，中央主体居中，底部留白，3:4 比例，高清，精致细节。``
```

---

## ✅ 单张海报 Quality 自检清单 (Hand-Drawn Poster QA Checklist)

在输出最终海报脚本与生图 Prompt 前，Agent 必须强制对照 [海报 8 维 QA 质量自检与复核清单](references/qa_checklist.md) 进行逐项审查：

| 审查维度 | 核心核查要点 |
| :--- | :--- |
| **1. 深度知识与干货** | 承载 3-5 个具体知识点/数据/代码步骤，拒绝抽象废话 |
| **2. 显式中文文案** | 画面渲染文案全量使用单引号 `'...'` 显式写入，字面无差错 |
| **3. 彻底消除占位符** | Prompt 中 100% 消除 `[要点说明]`、`[具体动作]` 等方括号占位符 |
| **4. 丰富视觉组件** | 显式组合 3-5 个具象组件（卡片框、胶囊标题、吊牌、放大镜、代码框、气泡总结） |
| **5. 纯粹自洽隐喻** | 全图设定统一自洽的场景隐喻（如总线/点餐/黑板），无冲突概念 |
| **6. IP 形象干货联动** | 小智特征描写完整（圆角方块头、单天线、点点眼），动作与知识强联动 |
| **7. Prompt 标准参数** | 包含米白纸张、莫兰迪配色、软墨勾线、全景居中留白、3:4 比例高清 |
| **8. 双语 Prompt 一致性** | 同时输出 🔵 中文确认版（供用户审核）与 🟢 英文生图版（用于生图），两者内容完全对应 |

---

## 📚 参考指南索引 (References Index)

1. [海报 8 维 QA 质量自检与复核清单](references/qa_checklist.md)
2. [海报版式与丰富视觉组件库](references/layout_templates.md)
3. [科技感小机器人 IP 形象指南 (小智 Xiao Zhi)](references/ip_mascot.md)
4. [手绘视觉风格指南](references/style_guide.md)
5. [场景化精细 Prompt 实战配方集](references/prompt_recipes.md)


