# Awesome OpenClaw Education Skills — 教育 AI 技能库

<div align="center">

[![GitHub Stars](https://img.shields.io/github/stars/xdelin/OpenClaw-Education-Skills?style=for-the-badge&logo=github&color=gold)](https://github.com/xdelin/OpenClaw-Education-Skills)
[![GitHub Forks](https://img.shields.io/github/forks/xdelin/OpenClaw-Education-Skills?style=for-the-badge&logo=github&color=blue)](https://github.com/xdelin/OpenClaw-Education-Skills)
[![GitHub Issues](https://img.shields.io/github/issues/xdelin/OpenClaw-Education-Skills?style=for-the-badge&logo=github)](https://github.com/xdelin/OpenClaw-Education-Skills)
[![技能数量](https://img.shields.io/badge/技能数量-392-brightgreen?style=for-the-badge)](https://github.com/xdelin/OpenClaw-Education-Skills/tree/main/skills)
[![License](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/平台-OpenClaw%20%7C%20NanoClaw-orange?style=for-the-badge)](https://github.com/openclaw)

**最大的开源教育与学术科研 AI 技能库，专为 OpenClaw 框架设计。**
*392 个精选技能 · 智能辅导 · 数学与自然科学 · 人文社科 · 学术科研 · 效率工具*
[English](README.md) | [中文](README_zh.md)

</div>

---

## 项目简介

**Awesome OpenClaw Education Skills** 是一个包含 **392 个 AI Agent 技能**的精选集合，覆盖教育与学术科研的完整领域。涵盖数学、理化生、人文社科及计算机等各个学术分支，这些技能专为 OpenClaw / NanoClaw —— 基于 Claude 的个人 AI 助手框架 —— 设计，能将通用 AI 智能体转变为强大的教学与科研研究伙伴。所有的技能由 AI 实现了双语净化与智能分类，总数量自动同步更新！

每个技能都是一个独立模块（`SKILL.md` 文件），它：
- 为 Agent 注入专业领域知识与教学辅导工作流
- 连接真实的数据源、API 和学术科研工具
- 输出结构化的课题研究或个性化教学结果

### 为什么需要这个技能库？

| 没有技能 | 配备 Awesome OpenClaw Education Skills 后 |
|---|---|
| 对复杂学科的通用 AI 回答 | 真实查询学术论文与高阶数学计算推导 |
| 无结构化学习路径策划 | 能够基于学科提供循序渐进的系统化教学大纲 |
| 无专业写作与文献支持 | LaTeX 排版、文献自动引用、语法深度润色 |
| 无法执行科研代码分析 | 执行 Python 数据分析，绘图与实验统计验证 |
| 缺乏个性化辅导反馈 | 能够模拟教授/导师提供 360 度能力评估与解答 |

本集合实时抓取并深度清洗自开源技能仓库的内容，涵盖学术研究工具、课堂评估工作流、教学辅助框架和前沿的自动化测试生成——让您的 AI 智能体具备媲美专业教研团队的能力。

---

## 安装方法

### 前置要求

- 已安装并运行 OpenClaw 或 NanoClaw
- Git（用于克隆本仓库）

---

### OpenClaw 用户

OpenClaw 从以下两个位置加载技能：

| 优先级别 | 路径 | 作用域 |
|---|---|---|
| 高 | `<workspace>/skills/` | 每个工作区独立（推荐） |
| 低 | `~/.openclaw/skills/` | 全局，所有 Agent 共享 |

#### 方法一 — 克隆并复制（推荐）

```bash
# 克隆本仓库
git clone https://github.com/xdelin/OpenClaw-Education-Skills.git

# 安装到当前工作区的 skills 目录
cp -r Awesome-Education-Skills/skills/* <your-workspace>/skills/

# 或安装到全局（所有 Agent 均可使用）
cp -r Awesome-Education-Skills/skills/* ~/.openclaw/skills/
```

下次会话时技能自动生效，无需重启。

#### 方法二 — 配置额外技能目录

将本仓库的克隆路径永久配置到 `~/.openclaw/openclaw.json` 中：

```json
{
  "skills": {
    "load": {
      "extraDirs": ["/path/to/Awesome-Education-Skills/skills"]
    }
  }
}
```

这样无需复制文件，即可挂载整个技能集合。

---

## 技能总览

| 类别 | 数量 | 代表技能 |
|---|---|---|
| 智能辅导与学习 | 5 | `training-course-designer`, `guided-learning-cn`, `quiz-generator`... |
| 数学与自然科学 | 9 | `book-math-tutor`, `maths-rage-bate`, `mathproofs-claw`... |
| 生物与医学 | 31 | `krumpphysio`, `ocd-erp-therapist`, `bmi-calculator`... |
| 化学与材料 | 6 | `pharmaclaw-catalyst-design`, `pharmaclaw-cheminformatics`, `materials-science-figure-skill`... |
| 人文社科与艺术 | 17 | `teacher-prep`, `language-learning`, `japanese-tutor`... |
| 计算机科学与工程 | 85 | `redux-saga-skill`, `active-learner`, `acg-rust-teacher`... |
| 数据与分析 | 41 | `botlearn-assessment`, `deepread-ocr`, `music-analysis`... |
| 可视化与展示 | 34 | `ppt-compress`, `md-ppt-generator`, `excalidraw-diagram`... |
| 学术研究与写作 | 58 | `reviewer-rebuttal-coach`, `add-educational-comments`, `certificate-generation`... |
| 笔记与知识库 | 51 | `flashcard`, `keep-learning-agent`, `learning-system-skill`... |
| 学习效率与工具 | 55 | `hinihao-chinese-tutor`, `flashcards-podcasts-master`, `recipe-create-classroom-course`... |

---

## 技能列表

### 智能辅导与学习

- **[training-course-designer](skills/training-course-designer)**
  - **描述**: 轻松设计专业的公司培训课程，一键生成包括材料、营销文案和评估在内的完整培训包。
- **[guided-learning-cn](skills/guided-learning-cn)**
  - **描述**: 一款中文引导式学习助手，提供循序渐进的概念讲解、个性化学习计划、备考复习以及费曼技巧。
- **[quiz-generator](skills/quiz-generator)**
  - **描述**: 一个多功能的试题生成器，可以创建选择题、填空题和简答题。支持模拟考试、详细解析、难度分级，并包含题库管理功能。
- **[teacher-toolkit](skills/teacher-toolkit)**
  - **描述**: 教师工具箱为教育工作者提供全面的资源，包括教案设计、评分标准、课堂活动、评估设计、学生反馈和家长沟通工具。
- **[book-tutor](skills/book-tutor)**
  - **描述**: 通过Lokuli MCP预订私人教师服务。当您需要寻找并预订附近的教师时使用。
### 数学与自然科学

- **[book-math-tutor](skills/book-math-tutor)**
  - **描述**: 通过Lokuli MCP预订数学辅导服务，满足个性化辅导需求。当您需要寻找并预订数学家教时使用。
- **[maths-rage-bate](skills/maths-rage-bate)**
  - **描述**: 此AI技能插件使用著名常数（φ、π、e、i）生成讽刺且显然正确的‘数学垃圾’公式。输出为LaTeX格式，适合用来创建数学梗图或回应‘数学垃圾’的请求。
- **[mathproofs-claw](skills/mathproofs-claw)**
  - **描述**: 此技能可与Lean-Claw竞技场互动，使用Lean 4证明数学定理。
- **[calculator-2](skills/calculator-2)**
  - **描述**: 此技能在用户要求计算、运算或提及加、减、乘、除等操作时，提供基本的算术计算功能。
- **[precision-calc](skills/precision-calc)**
  - **描述**: 此技能适用于所有类型的计算，包括算术、金融、科学、单位换算和日常数学，以确保准确性。
- **[lifecycle-carbon-calculator](skills/lifecycle-carbon-calculator)**
  - **描述**: 计算建筑材料和项目的隐含碳及生命周期排放，支持可持续设计决策。
- **[math-formula-calculator](skills/math-formula-calculator)**
  - **描述**: 数学公式计算器，擅长解析、分步计算和边界验证。适用于招投标价格计算及复杂公式的求解。
- **[earthquake-monitor](skills/earthquake-monitor)**
  - **描述**: 实时监测中国大陆、台湾及日本的地震情况，并提供主动警报，数据来源于CENC、CWA和JMA的WebSocket。
- **[survival-analysis-km](skills/survival-analysis-km)**
  - **描述**: 生成Kaplan-Meier生存曲线并计算生存统计量。
### 生物与医学

- **[krumpphysio](skills/krumpphysio)**
  - **描述**: 此AI技能插件训练OpenClaw代理成为受Krump启发的物理治疗教练，提供治疗性动作评分、结合游戏化Krump词汇和拉班记谱法的康复指导以及可选的Canton账本记录。它通过将正宗Krump舞蹈改编为物理治疗来支持健康与福祉计划。
- **[ocd-erp-therapist](skills/ocd-erp-therapist)**
  - **描述**: 一个OpenClaw技能，用于进行强迫症暴露与反应预防（ERP）治疗，具备抑制性学习框架、自动跟进提醒、进度跟踪和安全协议。
- **[bmi-calculator](skills/bmi-calculator)**
  - **描述**: 一个提供理想体重、健康计划和体重追踪的BMI计算器，同时支持儿童BMI计算与解读。
- **[quantinuumclaw](skills/quantinuumclaw)**
  - **描述**: quantinuumclaw插件利用Quantinuum、Guppy、Selene和Fly.io支持量子计算应用的构建与部署。适用于医疗项目，如药物发现和治疗优化，也可用于创建基于量子技术的网络应用并将结果集成到用户界面中。
- **[quantum](skills/quantum)**
  - **描述**: 此插件利用Quantinuum、Guppy、Selene和Fly.io等平台，帮助构建和部署量子计算应用程序。它非常适合用于药物发现、治疗优化等医疗项目，以及构建和部署基于量子技术的网络应用。
- **[afrexai-medical-billing](skills/afrexai-medical-billing)**
  - **描述**: 优化医疗计费流程，减少索赔拒付，并识别收入漏洞，适用于医疗机构、计费公司和收入周期团队。
- **[afrexai-pharmacy-compliance](skills/afrexai-pharmacy-compliance)**
  - **描述**: 帮助药剂师、药店经理和合规官应对DEA、药房管理委员会、USP、DSCSA和PBM的要求。
- **[clinical-data-extractor](skills/clinical-data-extractor)**
  - **描述**: 从药学会议网站或PDF文档中提取并结构化临床试验数据，包括药品名称、制造商、适应症、临床阶段、试验名称、会议以及疗效和安全性数据，并输出到markdown文件。
- **[medical](skills/medical)**
  - **描述**: 严格保护隐私的个人健康记录管理，包括症状跟踪、药物管理和生命体征记录，以及为看医生做准备。请勿用于诊断或治疗建议。
- **[healthie](skills/healthie)**
  - **描述**: Healthie 是一个通过GraphQL API管理患者、预约、目标和文档的工具。
- **[medical-record-structurer](skills/medical-record-structurer)**
  - **描述**: 一款将口头或手写医疗记录转换为标准化电子病历的工具，支持语音和文本输入，自动字段识别并结构化输出。包含通过skillpay.me实现的按次付费功能。
- **[biorxiv-openclaw-skill](skills/biorxiv-openclaw-skill)**
  - **描述**: 访问bioRxiv预印本库，按日期范围或类别检索最新的生物学预印本，并获取论文的元数据，如标题、作者、DOI等。
- **[medical-entity-extractor](skills/medical-entity-extractor)**
  - **描述**: 从患者信息中提取症状、药物、实验室数值和诊断等医学实体。
- **[medical-triage](skills/medical-triage)**
  - **描述**: 根据医疗紧急程度将医疗信息分类为危急、紧急或常规。
- **[lobster-bio-dev](skills/lobster-bio-dev)**
  - **描述**: 为多代理生物信息学引擎Lobster AI贡献代码，包括开发代理、创建服务、理解架构、修复错误或添加功能。适合参与Lobster代码库或开源项目的人。
- **[lobster-bio-use](skills/lobster-bio-use)**
  - **描述**: Lobster AI技能分析生物数据，包括单细胞和批量RNA-seq、文献挖掘和数据集发现，并提供质量控制、聚类、标记识别、差异表达和可视化功能。
- **[lobsterbio-use](skills/lobsterbio-use)**
  - **描述**: “lobsterbio-use”AI技能插件执行全面的生物信息学分析，包括单细胞和批量RNA测序、基因组学、蛋白质组学、代谢组学、机器学习、药物发现、文献和数据集搜索以及可视化。支持多种数据格式及主要生物数据库的访问编号。
- **[pharma-pharmacology-agent](skills/pharma-pharmacology-agent)**
  - **描述**: 此药理学插件从SMILES评估药物候选物，提供ADME/PK分析、类药性评分和PAINS警告。它还能预测诸如血脑屏障通透性、溶解度及CYP3A4抑制等属性。
- **[pharmaclaw-alphafold-agent](skills/pharmaclaw-alphafold-agent)**
  - **描述**: 此AI技能插件从公共PDB/AlphaFold数据库检索蛋白质结构，使用ESMFold预测折叠，检测结合位点，并通过RDKit执行基本的分子对接。它与化学查询集成，支持基于SMILES的对接以及知识产权扩展和催化剂设计。
- **[pharmaclaw-literature-agent](skills/pharmaclaw-literature-agent)**
  - **描述**: pharmaclaw-literature-agent v2.0.0 通过挖掘PubMed、Semantic Scholar和bioRxiv上的文献，专注于二期或三期临床试验，助力新药发现。它提供结构化的结果，包括新颖性评分、标题、作者、摘要、DOI、MeSH术语和引用次数。
- **[pharmaclaw-pharmacology-agent](skills/pharmaclaw-pharmacology-agent)**
  - **描述**: 此药理学工具从SMILES评估药物候选物，提供ADME/PK分析、类药性评分及PAINS警告。
- **[pharmaclaw-tox-agent](skills/pharmaclaw-tox-agent)**
  - **描述**: 此AI技能插件名为'pharmaclaw-tox-agent'，通过计算关键ADMET描述符、检查化学规则违反情况和评估类药性，从SMILES表示法中评价药物的安全性。它输出风险分类和详细的属性报告，并建议更安全的衍生物。
- **[clarity-clinical](skills/clarity-clinical)**
  - **描述**: 通过Clarity协议查询ClinVar和gnomAD的临床变异数据。该技能提供详细的变异注释，包括临床意义、致病性和群体遗传学信息。
- **[bioskills](skills/bioskills)**
  - **描述**: 此插件安装了425种生物信息学技能，涵盖序列分析、RNA-seq、单细胞、变异检测、宏基因组学和结构生物学等多个领域。适用于建立生物信息学能力或处理需要特定技能的任务。
- **[tnbc-research-swarm](skills/tnbc-research-swarm)**
  - **描述**: 加入TNBC研究群，注册为参与者，接收并完成研究或质量控制审核任务，从开放数据库中提交关于人口统计学、药物抗性、亚型、遗传学、生物标志物和诊断等主题的研究发现。
- **[research-automation](skills/research-automation)**
  - **描述**: 自动化的网络研究工具，适用于肽类、生物黑客、长寿科学和健康趋势等主题。适合发现新信息、跟踪趋势、监控科研更新或生成内容创意。支持定期或按需运行。
- **[neuralink-decoder](skills/neuralink-decoder)**
  - **描述**: 模拟并解码神经脉冲活动以控制光标移动（脑机接口）。
- **[intelligent-triage-symptom-analysis](skills/intelligent-triage-symptom-analysis)**
  - **描述**: 此AI技能插件提供智能分诊和症状分析，支持11个身体系统的650多种症状，并采用5级分类。它利用自然语言处理技术提取症状，拥有3000多种疾病的数据库，并通过机器学习增强对危及生命状况的警示机制。
- **[clarity-analyze](skills/clarity-analyze)**
  - **描述**: 通过Clarity协议提交研究问题以进行AI分析，适用于蛋白质变体、突变分析或查询汇总数据。需要CLARITY_WRITE_API_KEY。
- **[clarity-fold-status](skills/clarity-fold-status)**
  - **描述**: 从Clarity Protocol获取概述和状态信息，包括变体数量和数据可用性。适用于查询折叠状态、研究概要或API信息。
- **[clarity-research](skills/clarity-research)**
  - **描述**: 从Clarity Protocol中搜索蛋白质折叠研究数据，包括变体、折叠结果和特定疾病信息。功能包括按疾病或蛋白质名称列出变体及提供API信息。
### 化学与材料

- **[pharmaclaw-catalyst-design](skills/pharmaclaw-catalyst-design)**
  - **描述**: 此AI技能插件为多种药物合成反应推荐有机金属催化剂，并使用RDKit设计新型配体。它支持多种反应类型和催化剂，从精选数据库中提供带有评分的建议。
- **[pharmaclaw-cheminformatics](skills/pharmaclaw-cheminformatics)**
  - **描述**: 一个先进的化学信息学工具，用于三维分子分析、药效团映射、格式转换、RECAP逆合成分解和立体异构体枚举，非常适合三维构象生成和库设计等任务。
- **[materials-science-figure-skill](skills/materials-science-figure-skill)**
  - **描述**: 使用此技能通过Google的Nanobanana/Gemini图像模型生成或编辑出版物风格的图表，如材料科学论文示意图。它非常适合文本到图像、图像编辑和多参考工作流程。
- **[pharmaclaw-chemistry-query](skills/pharmaclaw-chemistry-query)**
  - **描述**: 此AI技能插件pharmaclaw-chemistry-query，支持通过PubChem API查询化合物信息和属性，并利用RDKit进行SMILES处理、分子属性分析及合成路线规划。
- **[chemistry-query](skills/chemistry-query)**
  - **描述**: 此AI技能插件chemistry-query利用PubChem API和RDKit进行化学数据分析，包括化合物信息、结构可视化及合成路线规划。
- **[paramus-chemistry](skills/paramus-chemistry)**
  - **描述**: 一套全面的化学和科学计算工具，包括分子量计算、LogP、TPSA、SMILES验证、热力学分析、聚合物分析、电化学及实验设计。
### 人文社科与艺术

- **[teacher-prep](skills/teacher-prep)**
  - **描述**: 教师备课助手专为小学语文教学设计，支持古诗、现代文、寓言、童话等各类课文。它能自动搜集相关资料，生成markdown格式的备课资料，制作教案PPT，并提供Word格式的课后练习题及答案。
- **[language-learning](skills/language-learning)**
  - **描述**: 这款AI语言导师通过对话、词汇练习、语法课程、闪卡和沉浸式练习帮助您学习任何语言，支持包括西班牙语、法语、德语、日语、中文（普通话/粤语）和韩语在内的所有语言。
- **[japanese-tutor](skills/japanese-tutor)**
  - **描述**: 一款互动日语学习助手，提供词汇、语法、测验、角色扮演和OCR翻译功能，并能解析PDF和DOCX文件以帮助学习和完成作业。
- **[pronunciation-coach](skills/pronunciation-coach)**
  - **描述**: 使用Azure语音服务进行真实语音分析的发音教练，评估音频中的音素准确性、流畅度、韵律和语调。
- **[book-language-tutor](skills/book-language-tutor)**
  - **描述**: 通过Lokuli MCP预订语言家教服务。当您需要寻找并预订语言家教时使用，特别是针对如“预订语言家教”或“查找附近语言家教”的请求。
- **[english-tutor](skills/english-tutor)**
  - **描述**: 这个个性化的美式英语导师帮助用户提升语言技能。
- **[kindergarten-assistant](skills/kindergarten-assistant)**
  - **描述**: 一位专注于英国EYFS框架和瑞吉欧教育法的早期教育专家，针对45天至2岁的儿童设计以孩子为主导的活动，跟踪发展里程碑，并支持创建滋养环境和课堂管理。
- **[voice-note-to-midi](skills/voice-note-to-midi)**
  - **描述**: 使用基于机器学习的音高检测和智能后处理技术，将语音笔记、哼唱和旋律音频录制转换为量化MIDI文件。
- **[aiml-music-generator](skills/aiml-music-generator)**
  - **描述**: 通过AIMLAPI生成高质量的音乐或歌曲，支持Suno、Udio、Minimax和ElevenLabs等多种模型。适用于有特定歌词或风格要求的请求。
- **[on-this-day-art](skills/on-this-day-art)**
  - **描述**: 此AI技能基于维基百科的“历史上的今天”事件，使用本地ComfyUI生成每日图片，适合需要历史或艺术图像的用户。它不使用云API、不生成视频，也不支持SD 3.5（在笔记本电脑上不稳定）。
- **[zeelin-liberal-arts-paper](skills/zeelin-liberal-arts-paper)**
  - **描述**: 文科研究生必备AI工具，提供从论文标题、大纲、引言、文献综述、论证、对策建议到结论的全流程生成支持，强调理论深度与思辨性。支持自定义章节数量。
- **[algorithmic-art-2](skills/algorithmic-art-2)**
  - **描述**: 使用p5.js创建独特的算法艺术，运用种子随机性和交互式参数探索。适用于生成艺术、流场和粒子系统。
- **[afrexai-photography-mastery](skills/afrexai-photography-mastery)**
  - **描述**: 全面的摄影指南，涵盖曝光、构图、光线、特定类型的工作流程、编辑、设备选择、作品集构建和客户管理，适合从初学者到专业人士的所有水平。
- **[torah-scholar](skills/torah-scholar)**
  - **描述**: 通过Sefaria API探索犹太教文献，包括托拉、塔纳赫、塔木德、密释纳和注释。适用于研究资料、查找经文、注释和交叉引用，支持希伯来语和英语。
- **[gaokao-essay](skills/gaokao-essay)**
  - **描述**: 高考作文助手，提供议论文模板、素材库、开头结尾、审题技巧及高分作文分析。
- **[short-drama-writer](skills/short-drama-writer)**
  - **描述**: 短剧作家：用于创作短剧。触发词为“短剧作家”。
- **[reading-knowledge](skills/reading-knowledge)**
  - **描述**: 一个知识丰富的伙伴，助您探索太空、宇宙和历史。它不带偏见地回答问题，清晰解释概念，并推荐教育资源。
### 计算机科学与工程

- **[redux-saga-skill](skills/redux-saga-skill)**
  - **描述**: 此插件为在Redux应用中使用Redux-Saga提供了最佳实践、模式和API指南，涵盖效果创建者、fork模型、通道、测试、并发、取消以及与现代Redux Toolkit的集成。
- **[active-learner](skills/active-learner)**
  - **描述**: 此插件实现了主动学习协议，使代理能够以编程方式将课程整合到`MEMORY.md`中，并生成结构化的反馈请求。
- **[acg-rust-teacher](skills/acg-rust-teacher)**
  - **描述**: 一个以ACG为主题的教育工具，通过动漫（如《Re：从零开始的异世界生活》和《Fate》系列）类比来讲解Rust的所有权系统，降低核心概念的学习难度。
- **[iterative-code-evolution](skills/iterative-code-evolution)**
  - **描述**: 通过结构化的分析、变异和评估循环逐步提升代码质量。适用于优化、调试以及在多个周期内改进设计，以有纪律的反思和原则性的选择取代随意的方法。
- **[coder-workspaces](skills/coder-workspaces)**
  - **描述**: 通过CLI管理Coder工作区和AI编码任务。可以列出、创建、启动、停止和删除工作区，或SSH进入工作区运行命令。使用Claude Code、Aider或其他代理监控AI编码任务。
- **[claude-code-cli](skills/claude-code-cli)**
  - **描述**: 使用Claude Code CLI处理如构建功能、审查PR或重构代码等任务。它支持交互和无头模式，但不适合简单修复或阅读代码。
- **[ctf-writeup-generator](skills/ctf-writeup-generator)**
  - **描述**: 自动生成专业的CTF解题报告，包括标志检测、题目分类和Markdown格式化。
- **[cs-landing-page-generator](skills/cs-landing-page-generator)**
  - **描述**: 此AI技能插件使用Tailwind CSS生成完整的Next.js/React（TSX）组件，创建高转化率的落地页，包含必要的部分并优化SEO以满足核心网页指标。
- **[react-nextjs-generator](skills/react-nextjs-generator)**
  - **描述**: 根据需求文档和UI设计图生成完整的React + Next.js项目，采用Ant Design、Tailwind CSS和Zustand技术栈。
- **[sql-generator](skills/sql-generator)**
  - **描述**: 自然语言转SQL、SQL解释与优化、创建表结构语句、生成测试数据及数据库迁移脚本的工具。
- **[quiverai-quickstart](skills/quiverai-quickstart)**
  - **描述**: QuiverAI SVG生成API的快速入门指南，涵盖从创建API密钥到环境配置、SDK安装及发送请求的全流程。
- **[afrexai-code-reviewer](skills/afrexai-code-reviewer)**
  - **描述**: 一款企业级代码审查工具，能够识别代码中的安全漏洞、性能问题、错误处理缺陷、架构问题和测试覆盖率不足。支持所有语言和代码库，无需任何依赖。
- **[q-kdb-code-review](skills/q-kdb-code-review)**
  - **描述**: 针对Q/kdb+的AI代码审查，用于在金融领域最简洁的语言中发现错误。
- **[matic-mquant-assistant](skills/matic-mquant-assistant)**
  - **描述**: MQuant Python策略开发助手，为MQuant平台生成可运行的Python代码。
- **[perry-workspaces](skills/perry-workspaces)**
  - **描述**: 在您的尾网中创建和管理隔离的Docker工作区，预装了Claude Code和OpenCode，适用于编码代理或远程开发环境。
- **[api-generator](skills/api-generator)**
  - **描述**: API代码生成器，用于创建RESTful端点、GraphQL模式、OpenAPI/Swagger文档、API客户端、模拟服务器、认证、限流和测试套件。非常适合后端开发和API框架搭建。
- **[git-cmt-helper](skills/git-cmt-helper)**
  - **描述**: 此技能按照Conventional Commits格式生成标准化的git提交信息，确保遵循团队关于类型前缀、范围、信息长度及重大变更文档的规定。
- **[gitmap](skills/gitmap)**
  - **描述**: 为ArcGIS网络地图提供版本控制，通过原生OpenClaw工具访问。
- **[afrexai-claude-code-production](skills/afrexai-claude-code-production)**
  - **描述**: Claude代码生产力系统简化了项目设置、提示模式、子代理协调、上下文管理、调试、重构、TDD，并在无需任何脚本的情况下将代码交付速度提高10倍。
- **[afrexai-git-engineering](skills/afrexai-git-engineering)**
  - **描述**: 此AI技能插件名为'afrexai-git-engineering'，帮助团队设计分支策略、实施代码审查流程、管理单一仓库、自动化发布以及维护可扩展的仓库实践。
- **[afrexai-ml-engineering](skills/afrexai-ml-engineering)**
  - **描述**: 从实验到规模化运营，构建、部署和扩展生产级ML/AI系统的一整套方法论。
- **[afrexai-performance-engineering](skills/afrexai-performance-engineering)**
  - **描述**: 一个全面的性能工程解决方案，涵盖性能分析、优化、负载测试、容量规划以及培养性能文化。支持Node.js、Python、Go、Java、数据库、API和前端技术。
- **[developer-agent](skills/developer-agent)**
  - **描述**: 通过与Cursor Agent协作、处理git工作流以及进行构建验证和部署管道来管理软件开发，确保高质量交付。
- **[public-apis-skill-creator](skills/public-apis-skill-creator)**
  - **描述**: 公共API技能创建器自动从public-apis/public-apis检索免费API，按功能推荐并提供最小可用示例（curl/Python/JS），同时还能生成自定义名称的API技能。
- **[code-quality-analyzer](skills/code-quality-analyzer)**
  - **描述**: 专业的代码质量分析工具，提供静态代码分析、代码异味检测、复杂度评估及最佳实践建议，支持JavaScript、TypeScript、Python、Java等主流语言。
- **[doro-docker-essentials](skills/doro-docker-essentials)**
  - **描述**: 此插件涵盖了管理容器、处理镜像和调试所需的基本Docker命令和工作流程。
- **[doro-git-essentials](skills/doro-git-essentials)**
  - **描述**: 版本控制、分支管理和协作所需的基本Git命令和工作流程。
- **[apple-developer-toolkit](skills/apple-developer-toolkit)**
  - **描述**: Apple开发者工具包是一个集成了文档搜索和App Store Connect命令行工具的一体化解决方案，可以搜索Apple框架、符号及WWDC会议内容，并提供超过120个命令来处理构建、TestFlight、提交等任务。
- **[python](skills/python)**
  - **描述**: 此插件强制执行Python编码最佳实践，包括PEP 8风格、语法验证、单元测试和使用现代版本。还提倡惯用模式，并在可能时使用uv进行依赖管理。
- **[devboxes](skills/devboxes)**
  - **描述**: 通过Traefik或Cloudflare隧道管理带有可网页访问的VSCode和VNC的开发环境容器。使用此技能来创建、启动、停止、列出或管理开发环境，或进行首次设置。
- **[azure-devops-mcp-replacement-for-openclaw](skills/azure-devops-mcp-replacement-for-openclaw)**
  - **描述**: 通过直接的REST API调用与Azure DevOps交互，管理和查询项目、团队、仓库、工作项、冲刺、管道、构建、测试计划和Wiki。
- **[a6-github-intel](skills/a6-github-intel)**
  - **描述**: 分析GitHub仓库，将其转换为单一的Markdown文档，生成架构图，并提供结构树、语言分布和最近活动等见解。专为AI设计，使用Python标准库，包含高级搜索技术和API快捷方式，且不执行任何代码。
- **[chrome-devtools-mcp](skills/chrome-devtools-mcp)**
  - **描述**: Chrome DevTools MCP是Google官方的浏览器自动化和测试服务器，通过Puppeteer控制Chrome，支持导航、表单填写、截图和性能分析等功能。
- **[github-intel](skills/github-intel)**
  - **描述**: 分析GitHub仓库，将其转换为AI友好的格式，如单个Markdown文档和架构图。同时提供仓库结构、语言分布及最近活动概要，全程不执行仓库中的任何代码。
- **[mac-mini-server](skills/mac-mini-server)**
  - **描述**: 在Mac Mini上设置OpenClaw作为始终在线的AI服务器，包括硬件推荐、macOS配置、Docker Desktop设置、launchd自动启动、Tailscale远程访问以及与VPS的成本比较。
- **[api-design-reviewer](skills/api-design-reviewer)**
  - **描述**: API设计审查插件评估并提供关于API设计的反馈，确保其高效、安全且易于维护。
- **[code-reviewer-2](skills/code-reviewer-2)**
  - **描述**: 为TypeScript、JavaScript、Python、Go、Swift和Kotlin提供代码审查自动化。分析拉取请求的复杂性、风险和代码质量，识别SOLID原则违反和代码异味，并生成审查报告。
- **[codebase-onboarding](skills/codebase-onboarding)**
  - **描述**: 代码库入职工具帮助新团队成员快速理解并浏览项目代码，加速他们融入开发流程。
- **[cs-code-reviewer](skills/cs-code-reviewer)**
  - **描述**: 自动化TypeScript、JavaScript、Python、Go、Swift和Kotlin的代码审查，分析拉取请求中的复杂度、风险及代码质量，并生成详细的审查报告。
- **[git-worktree-manager](skills/git-worktree-manager)**
  - **描述**: Git Worktree Manager 是一个管理工具，可以将多个工作目录链接到单个仓库，让你能够同时在不同的分支上工作。
- **[mcp-server-builder](skills/mcp-server-builder)**
  - **描述**: MCP服务器构建器是一款用于创建和管理服务器的工具，通过自定义配置简化了设置过程。
- **[senior-devops](skills/senior-devops)**
  - **描述**: 此AI技能插件提供全面的DevOps能力，包括CI/CD、基础设施自动化、容器化和云平台管理。它支持流水线设置、基础设施即代码、部署和监控。
- **[senior-ml-engineer](skills/senior-ml-engineer)**
  - **描述**: 此技能涵盖机器学习模型的部署、MLOps基础设施的搭建、模型性能监控、RAG流水线构建以及集成具有成本控制的大型语言模型。
- **[context7-api](skills/context7-api)**
  - **描述**: 在使用外部库、实现第三方包功能、调试库问题或需要获取训练数据截止日期之后的最新信息时，通过Context7 API获取当前的库文档。
- **[read-github](skills/read-github)**
  - **描述**: ‘read-github’插件技能允许对GitHub仓库进行语义搜索和智能代码导航，提供README、文档和代码的清晰聚合视图，并且尊重速率限制和robots.txt。
- **[senior-django-developer](skills/senior-django-developer)**
  - **描述**: 精通高性能、容器化和异步支持的Django架构，产出安全、静态类型且生产就绪的代码，采用严格的分层设计、全面测试及优先ASGI部署。
- **[github-automation-pro](skills/github-automation-pro)**
  - **描述**: 此插件可自动化GitHub任务，提高生产力并简化工作流程。
- **[task-development-workflow](skills/task-development-workflow)**
  - **描述**: 一种以测试驱动开发为主的流程，包括结构化规划、Trello任务管理和基于PR的代码审查，适用于需要阶段审批和Git分支策略的项目。
- **[github-analyzer](skills/github-analyzer)**
  - **描述**: 输入项目想法或GitHub链接，自动搜索相关开源项目并生成结构化分析报告（包括技术栈、优缺点和评分），同时可下载评分最高的前3名代码包。支持意图搜索和直接链接分析。
- **[github-to-clawhub](skills/github-to-clawhub)**
  - **描述**: 此AI技能插件'github-to-clawhub'能自动将GitHub开源项目转换为OpenClaw技能并发布到Clawhub。它从分析README、在Clawhub查重、撰写SKILL.md文件、创建目录结构，到最后发布技能全程自动化处理。
- **[ipfs-server](skills/ipfs-server)**
  - **描述**: 此插件提供完整的IPFS节点操作，包括安装、配置、内容固定、IPNS发布、对等管理及网关服务。
- **[devops-bridge](skills/devops-bridge)**
  - **描述**: devops-bridge技能将GitHub、CI/CD、Slack、Discord和问题跟踪器集成到自动化工作流程中，提供持续集成失败通知、拉取请求审查提醒以及仓库健康状况监控。它通过连接这些工具来简化开发流程，实现无缝沟通与协作。
- **[docker-essentials](skills/docker-essentials)**
  - **描述**: 用于管理容器、处理镜像和调试的基本Docker命令和工作流程。
- **[git-essentials](skills/git-essentials)**
  - **描述**: 掌握版本控制、分支管理和协作所需的Git基本命令和工作流程。
- **[github-issue-resolver](skills/github-issue-resolver)**
  - **描述**: 此AI技能插件，GitHub问题解决器，可以自动发现、分析并修复GitHub仓库中的开放问题，支持从问题检测到提交PR的全流程，并设有安全措施以防止范围蔓延和未经授权的操作。
- **[xcloud-docker-deploy](skills/xcloud-docker-deploy)**
  - **描述**: xCloud Docker 部署插件自动检测您的项目栈（如WordPress、Laravel、Node.js等），并将其部署到xCloud，生成可用于生产的Docker配置、CI/CD工作流和环境文件。
- **[devvit-publishing-auditor](skills/devvit-publishing-auditor)**
  - **描述**: 一个专为Reddit Devvit开发者设计的工具，用于在上传到Reddit服务器前审核并确保其应用满足所有要求。
- **[gitcode](skills/gitcode)**
  - **描述**: 通过GitCode的REST API获取和查询仓库、分支、议题、拉取请求、提交、标签、用户、组织等数据。兼容Python 3.7+标准库。
- **[claude-code-usage](skills/claude-code-usage)**
  - **描述**: 检查Claude Code OAuth使用限制，包括会话和周配额。还提供会话刷新提醒和重置检测监控。
- **[fullstack-developer](skills/fullstack-developer)**
  - **描述**: 此技能提供全面的全栈开发专业知识，包括前端、后端、数据库管理、API设计、DevOps和架构。非常适合构建、修复、审查或调试任何Web应用程序。
- **[code-quality-guard](skills/code-quality-guard)**
  - **描述**: 在部署前确保代码质量，验证导入、检查标签闭合，并强制执行逻辑最佳实践。
- **[devtools-secrets](skills/devtools-secrets)**
  - **描述**: 此插件提供使用Mise、Fnox和Infisical工具链设置和管理密钥的知识和指南，适用于配置密钥、环境变量，并确保安全的密钥管理实践。
- **[astrai-code-review](skills/astrai-code-review)**
  - **描述**: 基于人工智能的代码审查，通过智能模型路由节省超过40%的成本，相比总是使用最昂贵的模型。
- **[coder-helper](skills/coder-helper)**
  - **描述**: 用自然语言描述需求，工具将自动生成需求文档并打开编辑器。
- **[deepwiki](skills/deepwiki)**
  - **描述**: 查询DeepWiki MCP服务器以获取GitHub仓库文档、维基结构和AI生成的问题。
- **[reporead](skills/reporead)**
  - **描述**: 使用RepoRead AI分析GitHub仓库，适用于生成文档、进行安全审计或创建README等任务。支持MCP服务器集成和REST API。
- **[task-review-workflow](skills/task-review-workflow)**
  - **描述**: 此AI技能插件简化了任务驱动开发中的PR审查与合并流程，帮助决定是否合并或请求更改，并处理合并后的操作如Trello更新和分支清理。
- **[runtime-debug-skill](skills/runtime-debug-skill)**
  - **描述**: 使用运行时执行跟踪诊断并修复Python、Node.js或Java应用程序中的错误。适用于调试错误、分析故障和查找根本原因。
- **[runtime-debugging-skill](skills/runtime-debugging-skill)**
  - **描述**: 使用运行时执行跟踪诊断并修复Python、Node.js或Java应用程序中的错误。适用于调试错误、分析故障和查找根本原因。
- **[sql-query-generator](skills/sql-query-generator)**
  - **描述**: 生成带有内置验证、分页支持、风险分析和面向审计保护的SQL查询。
- **[database-schema-designer](skills/database-schema-designer)**
  - **描述**: 数据库模式设计器是一款用于高效创建、可视化和管理数据库模式的工具。
- **[schema-builder](skills/schema-builder)**
  - **描述**: 数据库模式设计工具，用于创建表结构、生成SQL DDL、迁移脚本、种子数据、ER图、优化报告、NoSQL模式和模式差异。适用于全面的数据库设计与管理。
- **[database-schema-differ](skills/database-schema-differ)**
  - **描述**: 比较不同环境下的数据库模式，生成迁移脚本，并跟踪模式演变。
- **[afrexai-database-engineer](skills/afrexai-database-engineer)**
  - **描述**: 一个涵盖数据库设计、优化、迁移和运维的全面系统，支持PostgreSQL、MySQL、SQLite及通用SQL模式。
- **[tg-mysql-design](skills/tg-mysql-design)**
  - **描述**: 一个MySQL表设计助手，根据业务规则文档和现有SQL脚本生成符合阿里巴巴规范的MySQL 5.7/8.0 DDL语句。支持.md和.sql文件输入，输出遵循RDS标准的表设计。
- **[xcode-build-analyzer](skills/xcode-build-analyzer)**
  - **描述**: 分析Xcode构建日志中的时间、警告、错误、慢编译以及来自DerivedData的构建历史。
- **[database-designer](skills/database-designer)**
  - **描述**: 数据库设计器是一款强大的工具，可高效创建和管理数据库架构。
- **[project-deep-analyzer](skills/project-deep-analyzer)**
  - **描述**: 此技能深入分析项目的系统边界、核心概念、模块架构、关键算法和技术选型，帮助用户理解代码库和排查问题。
- **[tech-data-playbook](skills/tech-data-playbook)**
  - **描述**: 科技与数据手册提供了软件开发、IT基础设施、网络安全、数据分析、云计算、人工智能/机器学习及数字化转型等广泛技术领域的最佳实践和策略。它是讨论任何技术战略、工程或数据平台时的首选。
- **[deepwiki-mcp](skills/deepwiki-mcp)**
  - **描述**: 使用DeepWiki MCP获取关于任何公开GitHub仓库的AI生成见解，包括源代码、架构和配置等细节。触发词包括'如何在<仓库>中实现X'、'deepwiki'或'在代码库中查找'。
- **[cron-scheduling](skills/cron-scheduling)**
  - **描述**: 使用cron和systemd定时器管理并调度重复任务，包括时区感知调度、监控、重试模式及调试。
- **[cs-google-workspace-cli](skills/cs-google-workspace-cli)**
  - **描述**: 通过gws命令行工具管理Google Workspace，包括Gmail、Drive、Sheets、Calendar、Docs、Chat和Tasks。实现任务自动化、运行安全审计，并利用43个内置脚本和10个角色包。
- **[smart-model-switcher-v2](skills/smart-model-switcher-v2)**
  - **描述**: 优化的智能模型切换器（v2）无需重启，零延迟自动选择计划中的最佳模型执行任务，支持新模型自动检测、多模型并行处理和智能任务分类。
- **[smart-model-switcher-v3](skills/smart-model-switcher-v3)**
  - **描述**: 通用智能模型切换器V3从您购买的所有API计划中智能选择最佳模型，支持超过50种模型，实现零延迟切换和高级任务处理。
- **[jules-api](skills/jules-api)**
  - **描述**: 通过Jules REST API管理Google Jules AI编码会话。启动任务、跟踪进度、批准计划、沟通交流以及访问会话详情和成果。
### 数据与分析

- **[botlearn-assessment](skills/botlearn-assessment)**
  - **描述**: BotLearn评估插件可以在五个维度（推理、检索、创造、执行和协调）上评估机器人的能力，支持手动触发或定期自动审查。
- **[deepread-ocr](skills/deepread-ocr)**
  - **描述**: DeepRead是一个AI原生的OCR平台，能在几分钟内将文档转换为高精度数据，准确率超过97%，并通过标记不确定字段将人工审核减少到仅5-10%。
- **[music-analysis](skills/music-analysis)**
  - **描述**: 分析本地音乐/音频文件，提取节奏、律动感、稳定性、结构和情感基调等特征，并结合歌词以获得更细腻的情感解读。
- **[fenge-smart-search](skills/fenge-smart-search)**
  - **描述**: 智能搜索工具，自动选择最佳搜索引擎：中文使用Bing，英文使用DuckDuckGo。无需API密钥，免费无限使用。
- **[afrexai-data-engineering](skills/afrexai-data-engineering)**
  - **描述**: 一个全面的指南，用于设计、构建、运营和扩展数据管道及基础设施，无需外部依赖。
- **[senior-data-engineer](skills/senior-data-engineer)**
  - **描述**: 此AI技能专长于构建可扩展的数据管道和ETL/ELT系统，精通Python、SQL、Spark、Airflow、dbt、Kafka及现代数据栈。涵盖数据建模、管道编排、数据质量和DataOps，适用于设计数据架构和优化工作流。
- **[code-stats](skills/code-stats)**
  - **描述**: 通过统计文件数量、代码行数并按文件扩展名分类，可视化项目复杂度，帮助评估项目的规模或增长。
- **[deepread-agent-setup](skills/deepread-agent-setup)**
  - **描述**: 通过OAuth设备流认证AI代理与DeepRead OCR API，用户在浏览器中批准代码后，代理将接收并以环境变量形式存储DEEPREAD_API_KEY。
- **[jina-reader](skills/jina-reader)**
  - **描述**: Jina AI Reader API 以三种模式提取网页内容：读取（URL转Markdown）、搜索（网络搜索+完整内容）和验证（事实核查）。它提供干净的内容而不暴露服务器IP。
- **[sql-to-bi-builder](skills/sql-to-bi-builder)**
  - **描述**: 将包含SQL查询的Markdown文件转换为BI仪表板规范和UI框架，包括查询解析、度量/维度推断、图表推荐、过滤器设计和布局生成。
- **[afrexai-data-analyst](skills/afrexai-data-analyst)**
  - **描述**: 作为一名资深数据分析师，你的职责是发现数据中的故事，并清晰地呈现出来以指导下一步行动。
- **[afrexai-data-governance](skills/afrexai-data-governance)**
  - **描述**: 评估、评分并改进组织在六个关键领域的数据治理状况。
- **[afrexai-data-privacy](skills/afrexai-data-privacy)**
  - **描述**: afrexai-data-privacy技能确保用户数据按照隐私标准得到保护和管理，防止信息被未经授权的访问。
- **[estat-mcp](skills/estat-mcp)**
  - **描述**: 从日本官方开放数据门户e-Stat检索有关人口、GDP、CPI、贸易和就业的政府统计数据，该平台提供超过3,000个统计表。免费API访问。
- **[senior-data-scientist](skills/senior-data-scientist)**
  - **描述**: 此AI技能插件专注于高级数据科学，包括统计建模、实验设计、因果推断和预测分析，并擅长使用Python、R和SQL进行A/B测试、特征工程、模型评估及MLflow实验跟踪。
- **[dataset-finder](skills/dataset-finder)**
  - **描述**: 使用此技能从Kaggle、UCI ML、Data.gov或Hugging Face等数据仓库中搜索、下载和探索数据集。它还支持预览数据集统计信息和生成数据卡片。
- **[simple-excel](skills/simple-excel)**
  - **描述**: 一个简单的Excel文件处理工具，支持.xlsx和.csv格式。适用于基本的数据操作任务，如读取、编辑和生成表格。
- **[csv-wizard](skills/csv-wizard)**
  - **描述**: 交互式数据清洗命令行工具，支持自动类型推断、缺失值处理和重复检测。
- **[expanso-csv-to-json](skills/expanso-csv-to-json)**
  - **描述**: 将CSV数据转换为JSON对象数组。
- **[expanso-json-to-csv](skills/expanso-json-to-csv)**
  - **描述**: 将JSON对象数组转换为CSV格式。
- **[ai-data-analysis](skills/ai-data-analysis)**
  - **描述**: 此命令对'data.csv'文件进行数据分析，专门关注销售趋势。
- **[csv-analyzer-cn](skills/csv-analyzer-cn)**
  - **描述**: 用于分析包含中文内容的CSV文件。
- **[microsoft-excel](skills/microsoft-excel)**
  - **描述**: 集成Microsoft Excel API，以读写工作簿、管理数据和访问OneDrive中的单元格值。使用此技能进行电子表格修改和数据管理。
- **[analyse-data](skills/analyse-data)**
  - **描述**: '分析数据'技能提供数据分析、解读和可视化功能，包括统计计算、趋势分析和图表生成。
- **[analysis-data](skills/analysis-data)**
  - **描述**: 'analysis-data' 技能提供数据分析、解读和可视化功能，包括统计计算、趋势分析及图表生成。
- **[data-analysis-pro](skills/data-analysis-pro)**
  - **描述**: 数据分析师技能提供数据分析、解释和可视化功能，支持计算统计、分析趋势和生成图表等任务。
- **[data-ground-truth](skills/data-ground-truth)**
  - **描述**: 在报告或建议中呈现数字之前，核实其准确性并对照行业标准进行检查。
- **[nexus-data-profile](skills/nexus-data-profile)**
  - **描述**: 此AI技能插件对数据集进行统计分析和质量评估。
- **[csv-handler](skills/csv-handler)**
  - **描述**: 处理来自建筑软件的CSV文件，自动识别分隔符和编码，并清理混乱的数据。
- **[data-evolution-analysis](skills/data-evolution-analysis)**
  - **描述**: 分析建筑组织的数据演变模式，评估其数字化成熟度和数据战略。
- **[data-lineage-tracker](skills/data-lineage-tracker)**
  - **描述**: 追踪数据的来源、转换和在系统中的流动，以支持审计跟踪、合规性和调试。
- **[pdf-ocr-layout](skills/pdf-ocr-layout)**
  - **描述**: 基于智谱GLM-OCR、GLM-4.7和GLM-4.6V的多模态文档深度分析工具。
- **[recursive-knowledge-miner](skills/recursive-knowledge-miner)**
  - **描述**: 专业的多层次知识提取和递归知识图谱构建。
- **[xml-reader](skills/xml-reader)**
  - **描述**: 此AI技能读取并解析来自各种建筑系统的XML文件，如P6进度表、BSDD导出、IFC-XML和COBie-XML，并将其转换为pandas DataFrame。
- **[geminipdfocr](skills/geminipdfocr)**
  - **描述**: 使用Google Gemini OCR从PDF中提取文本，处理扫描文档或基于图像的PDF。
- **[summary](skills/summary)**
  - **描述**: 使用summarize命令行工具，可以对网页、PDF、图片、音频和YouTube视频等URL或文件内容进行摘要。
- **[summarize-1-0-0](skills/summarize-1-0-0)**
  - **描述**: 使用summarize命令行工具，可以对网页、PDF、图片、音频和YouTube视频等URL或文件的内容进行总结。
- **[smart-summarizer](skills/smart-summarizer)**
  - **描述**: 轻松总结文章、PDF、YouTube视频、网页等内容。提取关键点、行动项和见解，便于快速消化或制作会议笔记。
- **[seek-and-analyze-video](skills/seek-and-analyze-video)**
  - **描述**: 分析并发现来自TikTok、YouTube和Instagram等平台的视频。总结内容，创建可搜索的知识库，用于研究或会议记录。
- **[deepwiki-ask](skills/deepwiki-ask)**
  - **描述**: 通过提供所有者/仓库名和您的问题，使用DeepWiki对仓库进行单次提问。
- **[gws-sheets-read](skills/gws-sheets-read)**
  - **描述**: 从Google Sheets电子表格中读取数据。
### 可视化与展示

- **[ppt-compress](skills/ppt-compress)**
  - **描述**: 通过压缩图片和转换为PDF来减小PPT/PPTX文件的大小，非常适合需要分享或上传大型演示文稿的场景。
- **[md-ppt-generator](skills/md-ppt-generator)**
  - **描述**: 科技产品发布会创意总监，将结构化的Markdown转换为具有视觉冲击力的“大字报”风格HTML幻灯片，专注于电影感暗色渐变、莫兰迪色系文字以及“呼吸感”动效。
- **[excalidraw-diagram](skills/excalidraw-diagram)**
  - **描述**: 根据文本内容生成Excalidraw图表，支持Obsidian（.md）、标准（.excalidraw）和动画（带动画顺序的.excalidraw）三种输出模式。通过关键词如“画图”、“流程图”或“动画图”触发。
- **[slide-maker](skills/slide-maker)**
  - **描述**: 一款用于生成演示文稿大纲、完整幻灯片、演讲笔记和设计建议的工具，输出为Markdown格式。
- **[z-article-card](skills/z-article-card)**
  - **描述**: 将长文转换为多张PNG图片，每张图片代表文章的一页。
- **[long-article-illustration](skills/long-article-illustration)**
  - **描述**: 长文配图助手插件可自动为长文分段、生成AI配图提示词，并调用图像生成工具完成配图。适用于公众号/博客文章、用户上传的文章以及批量生成文章插图。
- **[article-to-video-script](skills/article-to-video-script)**
  - **描述**: 将文章、研究报告和长篇内容转化为结构化的视频脚本，包含钩子、正文和轻量级行动号召部分，适用于短（不超过90秒）或长（约10分钟）的创作者评论。
- **[comman-felo-slides](skills/comman-felo-slides)**
  - **描述**: 此插件使用Claude Code中的Felo PPT任务API生成PPT或幻灯片。它处理API密钥检查、任务创建、轮询，并提供最终的ppt_url。
- **[dragon-ppt-maker](skills/dragon-ppt-maker)**
  - **描述**: 使用python-pptx创建精美的PPT，支持科技风格设计、图文混排及HTML内容嵌入。
- **[image-read](skills/image-read)**
  - **描述**: 使用智谱AI的GLM-4V-Flash免费多模态API理解并描述图片内容，识别图片中的物体。
- **[chart-generator](skills/chart-generator)**
  - **描述**: 一个数据可视化工具，可生成包括柱状图、折线图、饼图等多种SVG图表。适用于从原始数值数据创建视觉表示。
- **[diagrams-generator-pro](skills/diagrams-generator-pro)**
  - **描述**: 生成专业的图表，如云架构图、数据图表和学术插图。可以通过诸如'创建图表'或'可视化数据'的请求触发，或者用户提供的草图或图片进行专业重制时触发。
- **[table-image-generator](skills/table-image-generator)**
  - **描述**: 从数据生成清晰的表格图片，适用于Discord和Telegram等平台。支持暗黑/亮色模式、自定义样式和自动调整大小，无需Puppeteer。
- **[infographic-generation](skills/infographic-generation)**
  - **描述**: 创建专业信息图，优化视觉沟通效果，涵盖统计、流程、对比、时间线、列表、地理、层级、简历、报告及社交媒体等多种类型。
- **[chart-splat](skills/chart-splat)**
  - **描述**: 使用Chart Splat API生成包括折线图、条形图、饼图、环形图、雷达图、极地区域图和蜡烛图/OHLC图在内的美观图表。输出格式为PNG。
- **[chart-image](skills/chart-image)**
  - **描述**: 从数据生成高质量的图表图像，支持折线图、柱状图和饼图等多种类型。适用于数据可视化和报告生成，此插件专为Fly.io/VPS部署设计，无需本地编译或浏览器，使用纯Node.js及预构建二进制文件。
- **[article-to-infographic](skills/article-to-infographic)**
  - **描述**: 将文本内容转换为视觉上吸引人的HTML信息图，支持时间线、统计数据和流程图等多种风格。
- **[prd-visualization-skill](skills/prd-visualization-skill)**
  - **描述**: 此AI技能插件为层级数据（如产品需求文档、组织结构图和文件结构）创建交互式的D3.js可视化图表，支持列表、力导向图和径向聚类等多种视图模式。
- **[obsidian-cloudflare-pages-skill](skills/obsidian-cloudflare-pages-skill)**
  - **描述**: 将选定的Obsidian笔记从你的库发布到静态网站，并部署到Cloudflare Pages。
- **[openclaw-skill-obsidian-cloudflare-pages](skills/openclaw-skill-obsidian-cloudflare-pages)**
  - **描述**: 将选定的Obsidian笔记从你的库发布到静态网站，并部署到Cloudflare Pages。
- **[smart-illustrator](skills/smart-illustrator)**
  - **描述**: 智能配图与信息图生成器，支持文章插图、批量PPT/幻灯片信息图及封面图的生成，默认输出图片，也可仅输出提示。支持Bento Grid风格。
- **[mermaid-architect](skills/mermaid-architect)**
  - **描述**: 使用高级语法特性（如引号标签和ELK布局）创建美观的手绘Mermaid图。此技能适用于与图表、流程图或过程可视化相关的请求。
- **[slide-sniper](skills/slide-sniper)**
  - **描述**: 监控全屏视频或直播，利用视觉模型检测幻灯片翻页，并自动截图提取文字排版到笔记软件中。
- **[mermaid-visualizer](skills/mermaid-visualizer)**
  - **描述**: 将文本转换为专业的Mermaid图表，适用于演示文稿和文档，支持流程图、系统架构、比较图、思维导图等，并内置语法错误预防功能。
- **[ppt-outline](skills/ppt-outline)**
  - **描述**: 此AI技能插件可生成PPT大纲和独立的HTML演示文稿，适用于制作商业路演、商业计划书、工作报告、培训材料等内容。它非常适合于内容结构化，并且可以直接在任何浏览器中打开，无需额外软件支持。
- **[google-slides](skills/google-slides)**
  - **描述**: 通过托管的OAuth集成Google Slides API，创建、修改和格式化演示文稿。对于其他第三方应用，请使用api-gateway技能。
- **[pptx-pdf-font-fix](skills/pptx-pdf-font-fix)**
  - **描述**: 此插件通过为文本应用轻微透明度来修复从PowerPoint导出PDF时的字体嵌入问题，确保自定义字体能够正确嵌入。
- **[skill-mermaid-diagrams](skills/skill-mermaid-diagrams)**
  - **描述**: 为技术内容生成一致且基于模板的Mermaid图表，支持包括架构图、流程图和时间线在内的12种类型，具备自动模板选择、由大语言模型驱动的内容生成及错误处理功能。
- **[xfyun-ppt-gen](skills/xfyun-ppt-gen)**
  - **描述**: 根据优化的主题关键词生成专业的结构化PowerPoint演示文稿。
- **[tiangong-wps-ppt-automation](skills/tiangong-wps-ppt-automation)**
  - **描述**: 在Windows上自动化处理PowerPoint/WPS演示文稿的常见任务，如管理文本/备注/大纲、导出PDF/图片、替换文本、幻灯片操作和样式统一。仅适用于单个演示文稿的操作。
- **[gws-slides](skills/gws-slides)**
  - **描述**: 使用Google幻灯片创建和编辑演示文稿。
- **[md-2-pdf](skills/md-2-pdf)**
  - **描述**: 使用reportlab将Markdown文件转换为整洁、格式化的PDF。
- **[ima-knowledge-ai](skills/ima-knowledge-ai)**
  - **描述**: 此AI内容创作指南提供了工作流设计、模型选择和参数优化等方面的专家建议，确保在图像、视频和音乐生成中达到专业级效果。对于保持一致性和避免常见错误至关重要。
- **[pollinations-sketch-note](skills/pollinations-sketch-note)**
  - **描述**: 一款由AI驱动的工具，能够自动生成手绘风格的知识卡片，并自动搜索和总结主题。
### 学术研究与写作

- **[reviewer-rebuttal-coach](skills/reviewer-rebuttal-coach)**
  - **描述**: 此AI技能插件从剪贴板读取审稿意见、导师批注或评审反馈，并生成逐条回复、修改计划与优先级建议。
- **[add-educational-comments](skills/add-educational-comments)**
  - **描述**: 在指定的文件中添加教育性注释，如果未提供文件，则提示选择文件。
- **[certificate-generation](skills/certificate-generation)**
  - **描述**: 使用each::sense AI生成专业的证书、文凭和奖项。适用于课程结业、成就认证及定制品牌证书。
- **[diataxis-writing](skills/diataxis-writing)**
  - **描述**: Diataxis文档框架实践指南，为教程、操作指南、参考和解释四种类型的文档提供诊断、分类、模板及质量评估。
- **[agentledger-research-assistant](skills/agentledger-research-assistant)**
  - **描述**: 为AI助手设计的结构化网络研究工具，支持多源研究、将研究成果整合成可执行简报，并持续跟踪趋势。适用于市场调研、竞品分析及特定主题的深入研究。
- **[pdf-translate](skills/pdf-translate)**
  - **描述**: 此AI技能将PDF文档翻译成中文，保持专业排版。它逐节提取并翻译文本为结构良好的Markdown格式，然后生成支持CJK的新PDF。
- **[human-writing-azzar](skills/human-writing-azzar)**
  - **描述**: 此技能确保为README、技术文档和正式文件提供专业且类人的写作，避免使用AI特有的语言、流行语和冗余内容。
- **[aibrary-podcast-summary](skills/aibrary-podcast-summary)**
  - **描述**: 生成一段10到15分钟的单人叙述播客脚本，概述一本书的核心思想。
- **[aibrary-reading-list](skills/aibrary-reading-list)**
  - **描述**: 生成一个精心策划的主题阅读列表，书籍按逻辑顺序排列，适合深入探索或在特定领域建立专业知识。
- **[sop-writer](skills/sop-writer)**
  - **描述**: SOP编写工具用于创建标准操作流程，包括流程图、检查清单、审核评估和培训材料，并提供模板库以便快速使用。
- **[article-summarizer](skills/article-summarizer)**
  - **描述**: 文章摘要生成器自动抓取并总结网页文章，提供带有关键点和要点列表的结构化摘要。适合自媒体、运营人员及研究人员使用。
- **[translate-cli](skills/translate-cli)**
  - **描述**: 本指南介绍如何使用`translate`命令行工具处理多种输入的翻译、配置提供商及自定义设置。适用于命令构建、配置更新、提供商设置及故障排除。
- **[banner-youtube-translate-workflow](skills/banner-youtube-translate-workflow)**
  - **描述**: 此AI技能插件自动完成下载YouTube音频、在豆包中播放并捕获翻译的过程，适用于整段视频的翻译。
- **[alicloud-ai-audio-livetranslate](skills/alicloud-ai-audio-livetranslate)**
  - **描述**: 此AI技能插件适用于实时语音翻译，适合双语会议、即时口译以及将语音转换为文本或另一种语言。
- **[alicloud-media-video-translation](skills/alicloud-media-video-translation)**
  - **描述**: 通过OpenAPI管理阿里云IMS视频翻译任务，包括字幕、语音和面部。适用于基于API的翻译、状态更新和任务管理。
- **[clarity-literature](skills/clarity-literature)**
  - **描述**: 从Clarity Protocol检索研究论文、PubMed参考文献或特定主题（如蛋白质）的引用出版详情。
- **[translate-image](skills/translate-image)**
  - **描述**: 使用TranslateImage AI从图片中翻译、提取或移除文本。适用于处理包含外语文字的图片，如漫画。
- **[nexus-translate](skills/nexus-translate)**
  - **描述**: 提供超过50种语言的高质量翻译，具备文化意识。
- **[wechat-article-crayon](skills/wechat-article-crayon)**
  - **描述**: 此AI技能插件“wechat-article-crayon”辅助微信公众号文章的内容创作与改写，包括选题、标题优化、正文写作、重写润色、排版及封面图提示词生成，适用于撰写易读性强、引人入胜且自然流畅的文章。
- **[x-article-reader](skills/x-article-reader)**
  - **描述**: 此AI技能使用macOS的文本转语音功能朗读X（推特）文章。它接受文章链接，自动检测语言并选择合适的声音。可以通过说“朗读”或“读这个X文章”来使用。
- **[wechat-article-writer](skills/wechat-article-writer)**
  - **描述**: 公众号写作助手是一款专为创作微信公众号文章设计的AI工具，涵盖从选题到成稿及自动配图的全过程。
- **[wechat-article-extractor-skill](skills/wechat-article-extractor-skill)**
  - **描述**: 此技能从微信公众号文章中提取元数据和内容，包括标题、作者、内容、发布时间和封面图片，并将其转换为结构化数据。支持多种类型的文章，如图文、视频、图片、语音消息和转载。
- **[article-idea-capture](skills/article-idea-capture)**
  - **描述**: 记录并整理文章灵感、选题和半成型的观点，将其发展成大纲或初稿。当你有想法、想要保存一个念头以备后用，或是需要扩展已保存的概念时使用。
- **[docs-generator](skills/docs-generator)**
  - **描述**: 自动化文档生成器，用于创建API文档、README、CHANGELOG、贡献指南、架构文档、教程、FAQ和参考手册。支持REST、GraphQL和OpenAPI格式。
- **[developer-docs-framework](skills/developer-docs-framework)**
  - **描述**: 此AI技能插件“developer-docs-framework”提供了创建有效技术文档的最佳实践和框架，涵盖内容类型、写作风格、信息架构和开发者体验策略。它支持诸如教程、API参考和迁移指南等多种文档，并可通过如“写文档”或“API文档”等关键词触发。
- **[arxiv-reader](skills/arxiv-reader)**
  - **描述**: 此AI技能插件使用Python通过指定arXiv论文ID或URL，对论文进行分类和深度阅读，并直接打印出阅读笔记。
- **[meyhem-researcher](skills/meyhem-researcher)**
  - **描述**: 一个多查询研究工具，将主题分解为有针对性的查询，并预览顶级结果，无需API密钥。
- **[rubric-gap-analyzer](skills/rubric-gap-analyzer)**
  - **描述**: 分析当前草稿与评分标准或作业要求之间的差距，并给出提分计划。
- **[tavily-research-pro](skills/tavily-research-pro)**
  - **描述**: 一款专业的AI驱动的搜索和研究工具，能够聚合多维度数据，进行语义分析，并自动生成报告以收集结构化信息。
- **[pdf-tools](skills/pdf-tools)**
  - **描述**: 管理PDF文件，支持查看、提取文本、编辑文字、合并、拆分、旋转页面和访问元数据。
- **[ai-researcher](skills/ai-researcher)**
  - **描述**: 对任何主题进行深入研究，提供结构化分析、来源评估和专家级总结。
- **[paper-assistant](skills/paper-assistant)**
  - **描述**: 面向学术论文写作全过程的助手，涵盖选题、提纲到最终润色和投稿准备。
- **[research-logger-pro](skills/research-logger-pro)**
  - **描述**: 此AI技能插件将深度搜索结果自动保存到SQLite和Langfuse中，每个查询都会记录主题标签、时间戳和完整结果，便于检索和回顾。
- **[latex-writer](skills/latex-writer)**
  - **描述**: 从模板生成专业的LaTeX文档，支持学术论文、中文论文、简历以及自定义格式，并自动编译为PDF。
- **[agentarxiv](skills/agentarxiv)**
  - **描述**: 为AI代理提供结果导向的科学出版服务，支持研究、实验和同行评审的分享，并具备里程碑跟踪和复制奖励等功能。
- **[moltarxiv](skills/moltarxiv)**
  - **描述**: 面向结果的AI科研发布平台，支持分享研究成果、实验和同行评审，并提供验证过的数据资源和合作机会。
- **[meta-research](skills/meta-research)**
  - **描述**: 一个全自动的研究生命周期助手，从头脑风暴、文献回顾到实验设计、数据分析及撰写研究成果，注重可重复性和动态阶段转换。
- **[scholar-paper-downloader](skills/scholar-paper-downloader)**
  - **描述**: 一个学术论文PDF批量下载工具，支持从arXiv、PubMed等网站搜索并下载论文。自动提取元数据并生成索引列表，优先使用官方免费渠道下载，并为付费文献提供手动下载指引。
- **[academic-research-hub](skills/academic-research-hub)**
  - **描述**: 使用此技能搜索、下载和引用学术论文，以及收集学术信息。适用于文献综述、参考书目生成和访问arXiv、PubMed、Semantic Scholar或Google Scholar等数据库。
- **[citation-finder](skills/citation-finder)**
  - **描述**: 此AI技能插件citation-finder通过标题在多个数据库中搜索学术论文，并返回GB/T 7714、APA第七版和MLA第九版格式的引用及来源链接。
- **[web-researcher](skills/web-researcher)**
  - **描述**: 使用此技能进行深度研究、事实核查或获取最新的技术新闻。
- **[gemini-deep-research](skills/gemini-deep-research)**
  - **描述**: 使用Gemini深度研究助手进行深入且耗时的研究任务，包括多源综合、竞争分析、市场研究和技术调查。
- **[mckinsey-decision-memo-writer](skills/mckinsey-decision-memo-writer)**
  - **描述**: 将长文档、报告、提案和电子邮件线程精简为简洁的备忘录，突出关键点、风险、待解决的问题和下一步行动。
- **[scihub-paper-downloader](skills/scihub-paper-downloader)**
  - **描述**: 通过DOI从Sci-Hub获取PDF链接。
- **[auto-researcher](skills/auto-researcher)**
  - **描述**: 自主研究助手是一款用于深度调研、交叉验证并生成引用报告的工具。
- **[paper-fetcher](skills/paper-fetcher)**
  - **描述**: 通过DOI从Sci-Hub获取学术论文，自动下载并将PDF保存到research/papers/目录下，文件名简洁明了。适用于涉及DOI或PubMed论文的请求。
- **[core-researcher](skills/core-researcher)**
  - **描述**: 您是一位跨学科的学术研究助手，使用Core API进行文献综述、论文分析和学术写作。
- **[parallel-ai-research](skills/parallel-ai-research)**
  - **描述**: 针对某一主题进行开放式研究，创建动态的Markdown文档，并支持交互式和深度探索。
- **[research-agent](skills/research-agent)**
  - **描述**: 对任何主题进行深入研究，生成动态Markdown文档。支持互动和深度研究模式。
- **[proofreader](skills/proofreader)**
  - **描述**: 此AI技能插件提供校对功能，包括错别字检查、语法纠错、文风统一、可读性评分及全面的校对报告。需要校对时使用。
- **[thesis-helper](skills/thesis-helper)**
  - **描述**: 一款论文写作助手，可根据学术层次自动生成大纲、文献综述和摘要，同时管理引用格式、格式检查及答辩准备。
- **[paper-parse-figures](skills/paper-parse-figures)**
  - **描述**: 此AI技能插件将学术PDF论文转换为markdown格式，并提取其中的图表。
- **[chonkie-deepresearch](skills/chonkie-deepresearch)**
  - **描述**: 使用Chonkie DeepResearch进行深度查询，生成带有引用的详细研究报告，适用于市场分析、竞争情报和技术深入研究等任务。
- **[arxiv-watch](skills/arxiv-watch)**
  - **描述**: 按类别监控arXiv上的新论文。适合查看最新研究、跟踪特定主题或管理阅读列表。
- **[research-to-wechat](skills/research-to-wechat)**
  - **描述**: 此AI技能插件可将主题、笔记、文章、网址或转录转换为结构良好、带有内联视觉和封面图片的Markdown文章，适用于微信及其他平台。它还包括证据记录、HTML转换及多平台分发选项。
- **[knowledge-answer](skills/knowledge-answer)**
  - **描述**: 此AI技能'knowledge-answer'以用户偏好语言提供答案，基于搜索结果时会附上可点击的脚注引用。日期和引用格式均按标准设置。
- **[knowledge-forge](skills/knowledge-forge)**
  - **描述**: 将个人经验、案例研究和商业文档转化为结构化、易于理解、记忆和应用的教学内容。适用于创建课程大纲、演示文稿或可分享的知识文档。
- **[pro-zh-summary](skills/pro-zh-summary)**
  - **描述**: 专业工具，用于总结长篇中文文本，当用户要求摘要或要点时，自动分段并压缩内容。
### 笔记与知识库

- **[flashcard](skills/flashcard)**
  - **描述**: 闪卡生成与间隔复习系统，具备测验模式、导出功能（Markdown/Anki）及学习统计分析。适用于高效学习和复习。
- **[keep-learning-agent](skills/keep-learning-agent)**
  - **描述**: 持续学习Agent是一个知识沉淀与经验固化框架，支持学习记录、快速索引、自我修复及经验转模型等功能。内置完整模板、索引系统和SOP流程，助力AI持续进化。
- **[learning-system-skill](skills/learning-system-skill)**
  - **描述**: “learning-system-skill”插件管理知识图谱、深度学习笔记、实战复盘和关联网络。适用于制定学习计划、更新知识图谱、深入研究AI主题、总结经验或每周学习回顾等场景。在改完代码、读完论文或完成调研后，使用该插件提炼和组织知识。
- **[notebooklm-skill](skills/notebooklm-skill)**
  - **描述**: 此技能允许您从Claude Code查询Google NotebookLM笔记本，提供基于文档的答案，并具备浏览器自动化、库管理和持久认证功能。它通过仅使用文档内容来减少错误信息。
- **[session-memory-workspace](skills/session-memory-workspace)**
  - **描述**: 此AI技能插件将对话会话总结并保存到每日记忆文件中，使OpenClaw能够回忆和引用过去的对话。
- **[tiangong-notebooklm-cli](skills/tiangong-notebooklm-cli)**
  - **描述**: 一个用于NotebookLM的CLI工具，支持身份验证、笔记本管理、聊天、源处理、笔记、分享、研究及生成/下载工件。
- **[wechat-article-reader](skills/wechat-article-reader)**
  - **描述**: 此AI技能插件可将微信公众号文章导出为Markdown格式，当用户提供微信文章链接或要求下载、导出、保存文章时触发，默认保存到工作空间的source目录。
- **[feishu-article-collector](skills/feishu-article-collector)**
  - **描述**: 自动从今日头条和微信公众号收集文章，提取正文并通过AI生成摘要和分类，保存到飞书多维表格中。支持去重。
- **[article-extract](skills/article-extract)**
  - **描述**: 从微信公众号、博客和新闻网站中提取正文内容，绕过反爬机制，以纯文本形式输出。
- **[wechat-article-explainer](skills/wechat-article-explainer)**
  - **描述**: 此AI技能根据用户提供的链接或URL，用通俗的语言总结和解释微信公众号文章的内容。
- **[wechat-article-extractor](skills/wechat-article-extractor)**
  - **描述**: 从微信公众号文章链接中提取全文和图片，并保存为整洁的Markdown文件，自动处理反爬虫机制，寻找镜像站点。
- **[librag-knowledge-recall](skills/librag-knowledge-recall)**
  - **描述**: LibRAG 插件通过本地 `/api/v1/librag/knowbase/recall` 接口从知识库中召回数据，适用于中文场景下的知识检索、资料召回和证据提取等任务。
- **[feishu-document-reader](skills/feishu-document-reader)**
  - **描述**: 通过官方飞书开放API，从所有飞书文档类型中读取和提取内容。
- **[obsidian-openclaw-sync](skills/obsidian-openclaw-sync)**
  - **描述**: 在多个iCloud设备间同步Obsidian OpenClaw配置，管理符号链接以实现无缝集成。
- **[notion-2026-01-15](skills/notion-2026-01-15)**
  - **描述**: 更新至2026年1月15日的Notion API，新增了创建、移动和管理页面、数据源及模块的功能。
- **[agxntsix-research-logger](skills/agxntsix-research-logger)**
  - **描述**: 一个AI研究流程，能够自动将数据记录到SQLite并使用Langfuse进行追踪。
- **[research-logger](skills/research-logger)**
  - **描述**: 轻松管理研究，自动记录结果并保存到SQLite中，并带有元数据和完整的Langfuse追踪。适用于研究、竞争分析和知识库构建。
- **[multimedia-to-obsidian](skills/multimedia-to-obsidian)**
  - **描述**: 将PPT、PDF、DOCX和图片等多种多媒体文档导入Obsidian知识库，自动抽取每一页或每一幅图片的内容，利用多模态模型理解并生成文本描述保存至Obsidian，适用于整理培训材料、迁移笔记及将图像资料转化为结构化知识。
- **[obsidian-canvas-creator](skills/obsidian-canvas-creator)**
  - **描述**: 从文本创建可用于思维导图或自由布局的交互式Obsidian画布文件，非常适合可视化和空间组织信息。
- **[ai-research-to-obsidian](skills/ai-research-to-obsidian)**
  - **描述**: 此AI技能插件使用AI工具搜索信息，并将结果保存为Obsidian文档。当用户要求搜索问题、请求浏览器搜索并保存到Obsidian，或说“帮我查一下”并提到保存到笔记或文档时触发。
- **[pdf-parser-mineru](skills/pdf-parser-mineru)**
  - **描述**: 一个PDF解析工具，可将文档转换为Markdown、JSON等机器可读格式。
- **[pdf-co](skills/pdf-co)**
  - **描述**: PDF.co API与托管OAuth集成，用于PDF转换、合并、拆分、编辑和数据提取。使用此技能执行如将PDF转换为其他格式、添加水印或文本以及解析发票等任务。
- **[pdfagent](skills/pdfagent)**
  - **描述**: 一个自托管的PDF操作和转换解决方案，支持用量计量。
- **[zotero-pdf-upload](skills/zotero-pdf-upload)**
  - **描述**: 在Zotero网络图书馆中上传和管理PDF，支持个人和群组图书馆。适用于添加论文、整理收藏以及通过API管理您的图书馆。
- **[links-to-pdfs](skills/links-to-pdfs)**
  - **描述**: 从Notion、DocSend和PDF等来源下载并转换网页文档为本地PDF文件。支持受保护文档的认证和会话持久化。
- **[pdf-to-markdown](skills/pdf-to-markdown)**
  - **描述**: 将PDF文档转换为Markdown格式。当您需要将PDF转换成更易于编辑的形式时，请使用此工具。
- **[compress-pdf](skills/compress-pdf)**
  - **描述**: 通过将用户提供的PDF上传至Cross-Service-Solutions进行压缩处理，完成后返回压缩文件的下载链接。
- **[convert-to-pdf](skills/convert-to-pdf)**
  - **描述**: 将一个或多个文档上传至Cross-Service-Solutions，转换为PDF格式，并获取转换后文件（如多个文件则为ZIP）的下载链接。
- **[merge-pdf](skills/merge-pdf)**
  - **描述**: 将多个PDF文件上传到Cross-Service-Solutions进行合并，处理完成后会收到合并后的PDF下载链接。
- **[personal-notes](skills/personal-notes)**
  - **描述**: 作为记笔记和写日记的助手，记录想法、反思和日常日志。在提到日记、日志或“记下来”等词语时使用。
- **[book-brain-visual-reader](skills/book-brain-visual-reader)**
  - **描述**: 为LYGO Havens增强的BOOK BRAIN，具备视觉功能，集成三脑文件系统和记忆系统，结合文本和API数据进行浏览器、图像和截图的深度验证与检索。适用于使用视觉工具或浏览器自动化的代理。
- **[obsidian-cli-skills](skills/obsidian-cli-skills)**
  - **描述**: Obsidian CLI 是一个用于管理 Obsidian 笔记库的命令行工具，可以实现搜索、创建、移动和删除笔记等功能。
- **[obsidian-clip](skills/obsidian-clip)**
  - **描述**: 创建和管理Obsidian剪藏笔记，即网页或文章片段。当您希望获取URL的可读摘要并将其保存到Obsidian库中的Clip/YYYY-MM/目录时，使用此技能。
- **[obsidian-cli](skills/obsidian-cli)**
  - **描述**: 此技能适用于官方的Obsidian CLI（v1.12+），可实现库管理自动化，包括文件操作、每日笔记、搜索、任务等，以及开发工具。
- **[note](skills/note)**
  - **描述**: 一个用于捕捉、组织和检索笔记、想法和见解的系统。它会根据主题和项目自动整理内容，并在需要时提供相关信息，连接不同领域的相关概念。
- **[obsidian-cli-official](skills/obsidian-cli-official)**
  - **描述**: 官方Obsidian命令行工具（v1.12+），提供全面的命令行界面，用于管理笔记、任务、搜索、标签、属性、链接等功能。
- **[obsidians](skills/obsidians)**
  - **描述**: 此AI技能插件支持使用纯Markdown笔记和obsidian-cli自动化管理Obsidian库，并提供50多种模型用于图像和视频生成、文本转语音等多种任务。
- **[notebooklm-distiller](skills/notebooklm-distiller)**
  - **描述**: NotebookLM Distiller 可将知识从 Google NotebookLM 提取到 Obsidian，提供问答生成、结构化摘要、术语提取、网络研究和 Markdown 持久化功能。
- **[obsidian-organizer](skills/obsidian-organizer)**
  - **描述**: 整理和标准化Obsidian知识库，以提高可靠性和长期可维护性，包括文件夹结构设计、文件命名规范、迁移以及创建审核和修复工作流程。
- **[neural-note-taker](skills/neural-note-taker)**
  - **描述**: 一款高级的联想记忆工具，帮助在处理密集信息时建立事实与实体之间的联系，并在长时间会话中保持上下文。
- **[obsidian-daily](skills/obsidian-daily)**
  - **描述**: 通过obsidian-cli管理Obsidian每日笔记，包括创建、打开、添加条目和搜索库内容。支持如“昨天”或“3天前”等相对日期。需要通过Homebrew（Mac/Linux）或Scoop（Windows）安装obsidian-cli。
- **[second-brain](skills/second-brain)**
  - **描述**: 由Ensue支持的个人知识库，用于保存、回忆和扩展您的学习内容。可用于管理笔记和工具箱。
- **[save-to-obsidian](skills/save-to-obsidian)**
  - **描述**: 通过SSH将Markdown内容保存到远程Obsidian库。
- **[notesctl-skill-for-openclaw](skills/notesctl-skill-for-openclaw)**
  - **描述**: 通过本地脚本管理Apple Notes，包括创建、追加、列出、搜索、导出和编辑笔记。当您需要通过OpenClaw添加、列出、搜索或管理笔记文件夹时，请使用此技能。
- **[2nd-brain](skills/2nd-brain)**
  - **描述**: 个人知识库，用于存储和检索有关人物、地点、媒体、想法等的信息。当提到特定实体或使用诸如“记住”或“注意”等触发词时使用。
- **[brainrepo](skills/brainrepo)**
  - **描述**: 一个个人知识库，使用PARA和Zettelkasten方法来捕获、组织和检索信息。它通过诸如“保存这个”或“记住”等命令触发，支持每日/每周回顾，并与任何能读取markdown的AI代理集成，将所有内容以.md文件形式存储在Git仓库中，可用于Obsidian、VS Code或任何编辑器。
- **[notion-cli-agent](skills/notion-cli-agent)**
  - **描述**: 使用指定的查询来搜索页面。
- **[microsoft-onenote](skills/microsoft-onenote)**
  - **描述**: 与Microsoft OneNote集成，管理笔记本并操作数据。
- **[notion-integration](skills/notion-integration)**
  - **描述**: 与Notion集成，管理项目、文档和工作流程。使用此技能来操作您的Notion数据。
- **[voicenotes-official](skills/voicenotes-official)**
  - **描述**: 此官方语音笔记技能使OpenClaw能够通过自然对话使用新的API进行语义搜索、获取完整转录、按标签或日期筛选以及创建文本笔记。
- **[timeless](skills/timeless)**
  - **描述**: 管理和查询Timeless会议、房间、转录和AI文档。您还可以捕获播客剧集和YouTube视频进行转录，并与Timeless AI互动讨论会议内容。
### 学习效率与工具

- **[hinihao-chinese-tutor](skills/hinihao-chinese-tutor)**
  - **描述**: 一个主动式的中文导师，按计划提供精选的、来自真实世界的普通话学习内容，适合HSK 1-6级别的学习者。它能够推荐阅读材料、播客、视频和歌曲，并可以通过用户的特定请求或定时课程激活。
- **[flashcards-podcasts-master](skills/flashcards-podcasts-master)**
  - **描述**: 通过EchoDecks外部API管理抽认卡、生成AI内容并提供音频学习会话。
- **[recipe-create-classroom-course](skills/recipe-create-classroom-course)**
  - **描述**: 创建一个Google Classroom课程并邀请学生加入。
- **[training-plan](skills/training-plan)**
  - **描述**: 培训计划设计工具，帮助设计课程体系、效果评估、准备培训材料、安排日程和提供证书模板。适用于创建全面的培训计划和员工发展方案。
- **[optical-quantum-skill](skills/optical-quantum-skill)**
  - **描述**: 使用光纤和线性光学模拟量子内核。
- **[space-autonomy-skill](skills/space-autonomy-skill)**
  - **描述**: 一个使用光学量子核进行地形分类的自主空间导航代理。
- **[quantum-lab](skills/quantum-lab)**
  - **描述**: 使用~/.venvs/qiskit中的现有虚拟环境执行/home/bram/work/quantum_lab目录下的Python脚本和演示。在被要求运行该仓库中的特定子命令或笔记本时使用。
- **[quantumlab](skills/quantumlab)**
  - **描述**: 使用现有的虚拟环境~/.venvs/qiskit执行/home/bram/work/quantum_lab中的Python脚本和演示。这包括运行quant_math_lab.py、qcqi_pure_math_playground.py、quantum_app.py、quantumapp.server或仓库中的任何笔记本文件的子命令。
- **[expanso-language-detect](skills/expanso-language-detect)**
  - **描述**: 使用AI识别给定文本的语言。
- **[natural-language-planner](skills/natural-language-planner)**
  - **描述**: 此AI技能插件通过自然语言管理任务和项目，将任务组织成项目，跟踪进度，并提供本地看板仪表盘。
- **[git-standup](skills/git-standup)**
  - **描述**: 通过分析Git提交自动生成工作日报。
- **[plan-flow](skills/plan-flow)**
  - **描述**: 用于发现、规划、执行、代码审查和测试的AI辅助开发工作流程。
- **[error-analysis](skills/error-analysis)**
  - **描述**: 此AI技能插件提供错题分析，包括错题归类、知识点定位和复习建议。
- **[notion-1-0-0](skills/notion-1-0-0)**
  - **描述**: 此AI技能插件使用Notion API来创建和管理页面、数据库和区块。
- **[notion-template](skills/notion-template)**
  - **描述**: 一个用于生成工作空间、数据库、仪表盘、知识库、项目和个人模板的Notion模板生成器。在需要设计Notion模板时使用。
- **[vibe-notion](skills/vibe-notion)**
  - **描述**: 通过非官方私有API与Notion互动，管理页面、数据库、块、搜索、用户和评论。
- **[vibe-notionbot](skills/vibe-notionbot)**
  - **描述**: 通过官方API与Notion工作区交互，管理页面、数据库、模块、用户和评论。
- **[notion-skill](skills/notion-skill)**
  - **描述**: 通过官方Notion API与Notion页面和数据库进行交互。
- **[notion-clipper-skill](skills/notion-clipper-skill)**
  - **描述**: 将网页剪藏到Notion，通过抓取URL，将HTML转换为Markdown格式再转为Notion块，并保存至用户指定的Notion数据库或页面。当你想要将网页保存或剪藏到Notion时，可以使用此技能。
- **[wechat-to-notion](skills/wechat-to-notion)**
  - **描述**: 将微信公众号文章保存到Notion数据库。用户分享mp.weixin.qq.com链接时，此技能会提取标题、封面图片和正文内容，并将其保存为Notion块。
- **[visual-file-sorter](skills/visual-file-sorter)**
  - **描述**: 自动遍历下载文件夹或桌面，利用视觉模型识别文件内容并重命名，最后归档到指定分类目录。
- **[ux-researcher-designer](skills/ux-researcher-designer)**
  - **描述**: 为资深用户体验设计师和研究员提供的工具包，包括数据驱动的角色创建、旅程图绘制、可用性测试框架以及研究综合，适用于用户研究和设计验证。
- **[deepread-form-fill](skills/deepread-form-fill)**
  - **描述**: 基于AI的PDF表单填写。上传任意PDF和JSON格式的数据，AI将自动识别表单字段、语义映射数据、进行质量检查并填充表单，最终返回已完成的PDF文件。
- **[youtube-summarizer](skills/youtube-summarizer)**
  - **描述**: 自动获取YouTube视频字幕，生成结构化摘要，并将完整字幕发送到消息平台，提供关键见解和元数据。
- **[cognitive-brain](skills/cognitive-brain)**
  - **描述**: 跨会话记忆与认知系统，增强AI在多次互动中的记忆和理解能力。
- **[super-brain](skills/super-brain)**
  - **描述**: 超级大脑AI增强系统能够让AI跨会话记住用户，持续进化，并通过学习用户偏好和服务技巧提供个性化服务。
- **[audio-summary](skills/audio-summary)**
  - **描述**: ‘audio-summary’插件使用`ffmpeg`从视频文件中提取16k单声道压缩音频，基于百炼`qwen3-asr-flash`模型将音频转录并生成内容分段总结，并通过48k压缩支持大文件处理。
- **[notebooklm-bypass](skills/notebooklm-bypass)**
  - **描述**: 此AI技能插件提供对NotebookLM的编程控制，并能自动从认证错误中恢复。
- **[expanso-text-summarize](skills/expanso-text-summarize)**
  - **描述**: 使用AI将文本总结成3到5个要点。
- **[deepreader-skill](skills/deepreader-skill)**
  - **描述**: OpenClaw的默认网页内容阅读器，无需API密钥即可将Twitter、Reddit、YouTube及任何网页转换为干净的Markdown格式。适用于将社交媒体帖子、文章或视频字幕导入到代理记忆中。
- **[read-optimizer](skills/read-optimizer)**
  - **描述**: 通过使用智能策略（如head、tail、grep、diff）优化文件读取，以减少令牌使用和延迟。
- **[obsidian-plugin-tasknotes](skills/obsidian-plugin-tasknotes)**
  - **描述**: 使用TaskNotes插件在Obsidian中管理任务，包括创建、列出、查询、更新和删除任务。
- **[rss-ai-reader](skills/rss-ai-reader)**
  - **描述**: RSS AI阅读器自动抓取订阅内容，使用LLM生成摘要，并推送到飞书、Telegram或电子邮件。支持定时抓取，可通过“帮我订阅”或“监控这个网站”等指令触发。
- **[obsidian-task](skills/obsidian-task)**
  - **描述**: 通过obsidian-cli在终端管理Obsidian任务，包括列出、切换、创建和更新任务。
- **[reddit-readonly](skills/reddit-readonly)**
  - **描述**: 以只读模式浏览和搜索Reddit，允许您探索子版块、按主题查找帖子并查看评论线程。
- **[doc-summarizer](skills/doc-summarizer)**
  - **描述**: 一款多功能AI工具，可生成文档和文本摘要、会议纪要、邮件摘要，并创建思维导图。
- **[notion-mcp](skills/notion-mcp)**
  - **描述**: Notion MCP插件通过托管认证集成，可查询数据库、创建和更新页面以及管理工作区中的块。
- **[yt-summary](skills/yt-summary)**
  - **描述**: 通过分享YouTube视频链接并可选地添加特定指示（如‘关注技术细节’）来生成视频摘要。
- **[shelly-meeting-summarizer](skills/shelly-meeting-summarizer)**
  - **描述**: 将原始会议记录转换为清晰、结构化且可执行的摘要。
- **[tube-summary](skills/tube-summary)**
  - **描述**: 在YouTube上搜索任何主题的视频，并从字幕中获取智能摘要，让您无需观看即可快速了解内容。
- **[rss-reader](skills/rss-reader)**
  - **描述**: 监控RSS和Atom源以进行内容研究、跟踪行业新闻或构建个人新闻聚合器。支持多源分类、过滤和摘要。
- **[youmind-youtube-transcript](skills/youmind-youtube-transcript)**
  - **描述**: 使用YouMind API提取并保存YouTube视频的字幕和文本，支持一次处理最多5个视频。带有时间戳的字幕将以markdown格式保存在您的YouMind面板上，可以从任何IP访问。
- **[slack-reader](skills/slack-reader)**
  - **描述**: 汇总Slack频道的历史消息和讨论线程。适用于Slack链接，查看或总结讨论内容，或检查最近的消息。
- **[plsreadme](skills/plsreadme)**
  - **描述**: 通过plsreadme.com将Markdown文件和文本分享为简洁易读的网页链接，适用于分享文档、README、产品需求文档、提案或笔记。需要使用plsreadme MCP服务器（npx plsreadme-mcp）
- **[youtube-voice-summarizer-elevenlabs](skills/youtube-voice-summarizer-elevenlabs)**
  - **描述**: 使用ElevenLabs TTS将YouTube视频转换成播客风格的语音摘要。
- **[tweet-summarizer-lite](skills/tweet-summarizer-lite)**
  - **描述**: 从Twitter获取并总结单条推文。适用于快速轻量的推文查询。
- **[focus-coach](skills/focus-coach)**
  - **描述**: 专注教练插件使用BJ Fogg的B=MAP模型帮助AI代理诊断注意力问题，并提出一个小而可行的步骤。它适用于提高专注力、克服拖延症并通过微习惯提升生产力。
- **[google-workspace-automation](skills/google-workspace-automation)**
  - **描述**: 使用范围感知计划自动化Gmail、Drive、Sheets和Calendar的日常任务，确保明确的OAuth权限范围及可审计的输出。
- **[task-decomposer](skills/task-decomposer)**
  - **描述**: 此技能将复杂请求分解为简单的子任务，确定所需功能，并根据需要查找现有解决方案或创建新方案。
- **[time-checker](skills/time-checker)**
  - **描述**: 使用time.is获取全球任意地点的准确时间、日期和时区信息。适用于查询“X地现在几点”或验证时区差。
- **[afrexai-email-to-calendar](skills/afrexai-email-to-calendar)**
  - **描述**: 此AI技能从邮件中提取日历事件、截止日期、行动项和跟进事项，兼容任何日历提供商。它使用纯代理智能，无需外部依赖。
- **[afrexai-sprint-planner](skills/afrexai-sprint-planner)**
  - **描述**: 高效规划、界定范围并执行敏捷冲刺，确保成果交付，无冗余流程。
- **[todolist](skills/todolist)**
  - **描述**: 此技能模块提供专用的增强功能，以提高开发与研究效率。
- **[aibrary-growth-plan](skills/aibrary-growth-plan)**
  - **描述**: 创建一个包含书籍推荐、里程碑和可执行的周任务的结构化个人成长计划，适用于学习、技能提升或职业发展。
- **[student-timetable](skills/student-timetable)**
  - **描述**: 一个学生时间表管理工具，适用于自我管理或家长管理的孩子档案，包括初始化流程和在日程/档案下的档案注册。
