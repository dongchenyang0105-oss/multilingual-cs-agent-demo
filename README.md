# multilingual-cs-agent-demo
LLM-powered multilingual customer service demo with prompt iteration log (pre-sales portfolio project)
# 多语言智能客服 Demo｜LLM Pre-sales Portfolio

跨境电商场景的多语言客服解决方案 MVP：意图识别 → FAQ 知识库锚定 → 目标语言直接生成 → 高风险转人工。
重点不在代码量，在**迭代记录**：通过三轮 prompt 迭代实证了轻量模型的小语种能力边界、知识库信息漂移与输出非确定性。

## 内容
- 📄 [multilingual_demo.pdf](https://github.com/user-attachments/files/28806833/multilingual_demo.pdf) — 需求分析、架构、技术决策 trade-off、ROI 测算、风险披露
- 🔬 [可运行 Colab Demo](https://colab.research.google.com/drive/1F9iGY1Pn6qh41YSSuGkfW4dmDT3PUdDK?usp=sharing) — 含 v1→v2 prompt 迭代记录与原始输出对比
- 💻 demo_zhipu.py — 核心代码（智谱 GLM API）

## 关键发现
1. Prompt 可稳定修复结构性问题（问候语域、敬称、风险分级），无法补足模型的形态复杂语言生成上限（德语格变错误三轮随机换位出现）
2. 知识库改写中出现信息漂移（"预付邮资"失真）——幻觉风险的实证案例
3. 知识库锚定约束有效：超范围问题（"Do you ship to Japan?"）正确拒绝编造


目标方向：AI 解决方案 / 技术售前 / 模型评估
