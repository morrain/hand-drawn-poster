# 📕 手绘海报 (Hand-Drawn Poster) Skill

> **专为单项知识主题/文章片段生成单张高颜值 Q 版手绘图文海报设计的 AI Skill**  
> 接收上层业务逻辑分发或用户指定的单项知识主题，深入抽取 3-5 个核心干货，融合小机器人“小智 (Xiao Zhi)” IP 形象，自动生成单张高颜值小红书科普海报脚本与精细生图 Prompt。

---

## 📁 目录结构 (Directory Structure)

```
hand-drawn-poster/
├── SKILL.md                          # Skill 主配置文件 (含干货萃取、Grill-Me工作流、Prompt公式、双语范例与 8 维 Checklist)
├── README.md                         # 本说明文档
├── LICENSE                           # MIT 开源许可证
├── .gitignore                        # Git 忽略配置
├── references/                       # 参考文档库
│   ├── qa_checklist.md               # ✅ 8 维 Quality Assurance 单页海报质量自检与复核清单
│   ├── ip_mascot.md                  # 🤖 科技感小机器人 IP 形象指南 (小智 动作/形态/表情联动矩阵)
│   ├── style_guide.md                # 🖌️ 手绘视觉风格指南 (暖米白纸质感、莫兰迪配色、软墨线条)
│   ├── layout_templates.md           # 📐 5 大单页经典版式与 8 大类手绘视觉组件库
│   └── prompt_recipes.md             # 📖 单张海报场景化 Prompt 实战配方集
└── examples/                         # 实战案例与效果集
    ├── master_article.md             # 📄 标杆测试文章 (大模型 MCP 协议深度科普)
    └── *.jpg                         # 🖼️ 手绘海报真实生成效果图样例
```

---

## 🚀 核心工作流 (Core Workflow)

1. **单页知识干货萃取**：针对给定的单项知识点或段落，提炼 3-5 个具体核心要点、对比数据与总结金句。
2. **单页版式与隐喻提案**：匹配 5 大单页经典版式（Hero 破题版、四宫格干货版、左右分栏对比版、架构流程切片版、金句速查闭环版）。
3. **小智 IP 场景联动**：结合该页干货，匹配小智机器人（方块头、单天线、点点眼）的专属动作与道具。
4. **输出精细 Prompt 脚本**：输出包含全量显式中文文案（单引号包裹）、丰富视觉组件及 100% 无占位符的中文与英文生图 Prompt。

---

## 🤖 AI Agent 接入与使用指南 (Agent Integration Guide)

本 Skill 遵循 AI Agent 标准 Skill 规格（包含 `SKILL.md` YAML Frontmatter 与 `references/` 详细参考手册）：

- **自动加载**：将本仓库目录或软链接放置于 Agent 的 Skill 扫描路径（如 `.agents/skills/hand-drawn-poster` 或 `~/.gemini/config/skills/hand-drawn-poster`）中即可自动注册。
- **触发逻辑**：当用户请求生成手绘科普海报、小红书图文海报、或指定主题知识卡片 Prompt 时，Agent 会自动载入本 Skill 指令及依赖文档。
- **双语 Prompt 机制**：Agent 内部使用**英文 Prompt**确保生图模型渲染质量，输出时同时提供 **🔵 中文确认版 Prompt** 与 **🟢 英文生图版 Prompt** 供用户审核与最终调用。

---

## 📄 许可证 (License)

[MIT License](LICENSE)
