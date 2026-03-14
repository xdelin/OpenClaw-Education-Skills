# Awesome OpenClaw Education Skills — Education AI Skills Library

<div align="center">

[![GitHub Stars](https://img.shields.io/github/stars/xdelin/OpenClaw-Education-Skills?style=for-the-badge&logo=github&color=gold)](https://github.com/xdelin/OpenClaw-Education-Skills)
[![GitHub Forks](https://img.shields.io/github/forks/xdelin/OpenClaw-Education-Skills?style=for-the-badge&logo=github&color=blue)](https://github.com/xdelin/OpenClaw-Education-Skills)
[![GitHub Issues](https://img.shields.io/github/issues/xdelin/OpenClaw-Education-Skills?style=for-the-badge&logo=github)](https://github.com/xdelin/OpenClaw-Education-Skills)
[![Skills Count](https://img.shields.io/badge/Skills%20Count-392-brightgreen?style=for-the-badge)](https://github.com/xdelin/OpenClaw-Education-Skills/tree/main/skills)
[![License](https://img.shields.io/badge/License-MIT-purple?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-OpenClaw%20%7C%20NanoClaw-orange?style=for-the-badge)](https://github.com/openclaw)

**The largest open-source Education AI skills library, designed specifically for the OpenClaw framework.**
*392 Curated Skills · Intelligent Tutoring · Math & Science · Humanities · Academic Research · Efficiency Tools*
[English](README.md) | [中文](README_zh.md)

</div>

---

## Project Introduction

**Awesome OpenClaw Education Skills** is a curated collection of **392 AI Agent skills**, covering the entire spectrum of education and academic research. These skills are designed specifically for OpenClaw / NanoClaw —— Claude-based personal AI assistant frameworks —— transforming a general-purpose AI agent into a powerful teaching and academic research partner. 
Each skill is an independent module (`SKILL.md` file) that:
- Injects domain-specific professional knowledge and teaching workflows into the Agent.
- Connects to real academic databases, APIs, and computational tools.
- Outputs structured research findings or personalized educational guides.

### Why do you need this skills library?

| Without Skills | Equipped with OpenClaw Education Skills |
|---|---|
| Generic AI answers to complex subjects | Real-time querying of academic papers and advanced mathematical derivations |
| No structured learning paths | Provides step-by-step systemic syllabi based on chosen subjects |
| No academic writing support | LaTeX typesetting, automatic bibliography citation, grammar polishing |
| Cannot execute code analysis | Executes Python data analysis, plotting, and experimental stat validations |
| Lacks personalized tutoring | Simulates professors/tutors to provide 360-degree assessments and QA |

This collection aggregates massive real-time tools from open-source repositories, strictly filtered to exclude irrelevancy, equipping your AI agent with capabilities comparable to an entire professional educational research team.

---

## Installation

### Prerequisites

- Pre-installed and running OpenClaw or NanoClaw.
- Git (to clone this repository).

---

### OpenClaw Users

OpenClaw loads skills from the following two locations:

| Priority | Path | Scope |
|---|---|---|
| High | `<workspace>/skills/` | Independent per workspace (Recommended) |
| Low | `~/.openclaw/skills/` | Global, shared by all Agents |

#### Method 1 — Clone and Copy (Recommended)

```bash
# Clone this repository
git clone https://github.com/xdelin/OpenClaw-Education-Skills.git

# Install to current workspace's skills directory
cp -r Awesome-Education-Skills/skills/* <your-workspace>/skills/

# Or install globally (available to all Agents)
cp -r Awesome-Education-Skills/skills/* ~/.openclaw/skills/
```

Skills will take effect automatically in your next session without a restart.

#### Method 2 — Configure Extra Skills Directory

Permanently map this repository's clone path inside `~/.openclaw/openclaw.json`:

```json
{
  "skills": {
    "load": {
      "extraDirs": ["/path/to/Awesome-Education-Skills/skills"]
    }
  }
}
```

This mounts the entire skill collection without copying files.

---

## Skills Overview

| Category | Skills Count | Representative Skills |
|---|---|---|
| Intelligent Tutoring | 5 | `training-course-designer`, `guided-learning-cn`, `quiz-generator`... |
| Math & Science | 9 | `book-math-tutor`, `maths-rage-bate`, `mathproofs-claw`... |
| Biology & Medicine | 31 | `krumpphysio`, `ocd-erp-therapist`, `bmi-calculator`... |
| Chemistry & Materials | 6 | `pharmaclaw-catalyst-design`, `pharmaclaw-cheminformatics`, `materials-science-figure-skill`... |
| Arts, Humanities & Social Sciences | 17 | `teacher-prep`, `language-learning`, `japanese-tutor`... |
| Computer Science & Engineering | 85 | `redux-saga-skill`, `active-learner`, `acg-rust-teacher`... |
| Data & Analysis | 41 | `botlearn-assessment`, `deepread-ocr`, `music-analysis`... |
| Visual & Presentation | 34 | `ppt-compress`, `md-ppt-generator`, `excalidraw-diagram`... |
| Academic & Writing | 58 | `reviewer-rebuttal-coach`, `add-educational-comments`, `certificate-generation`... |
| Notes & Knowledge Base | 51 | `flashcard`, `keep-learning-agent`, `learning-system-skill`... |
| Productivity & Study Tools | 55 | `hinihao-chinese-tutor`, `flashcards-podcasts-master`, `recipe-create-classroom-course`... |

---

## Skills List

### Intelligent Tutoring

- **[training-course-designer](skills/training-course-designer)**
  - **Description**: Effortlessly design professional training courses for corporate L&D with one-click generation of complete packages, including materials, marketing copy, and assessments.
- **[guided-learning-cn](skills/guided-learning-cn)**
  - **Description**: A guided learning assistant for mastering any topic or skill in Chinese, offering step-by-step concept teaching, personalized study plans, exam preparation, and the Feynman technique.
- **[quiz-generator](skills/quiz-generator)**
  - **Description**: A versatile quiz generator that creates multiple choice, fill-in-blank, and short answer questions. It supports mock exams, detailed explanations, difficulty levels, and includes features for managing a question bank.
- **[teacher-toolkit](skills/teacher-toolkit)**
  - **Description**: The Teacher Toolkit is a comprehensive resource for educators, offering lesson planning, rubrics, classroom activities, assessments, student feedback, and parent communication tools.
- **[book-tutor](skills/book-tutor)**
  - **Description**: Book a tutor through Lokuli MCP for personalized tutoring services. Use this when you need to find and book a tutor near you.
### Math & Science

- **[book-math-tutor](skills/book-math-tutor)**
  - **Description**: Book math-tutor services through Lokuli MCP for personalized tutoring needs. Use this when looking to find and book a math tutor.
- **[maths-rage-bate](skills/maths-rage-bate)**
  - **Description**: This AI skill plugin generates satirical and trivially true equations, known as 'math slop,' using famous constants (φ, π, e, i). The output is in LaTeX format, perfect for creating math memes or responding to requests for 'math slop.'
- **[mathproofs-claw](skills/mathproofs-claw)**
  - **Description**: This skill enables interaction with the Lean-Claw Arena to prove mathematical theorems using Lean 4.
- **[calculator-2](skills/calculator-2)**
  - **Description**: This skill performs basic arithmetic calculations when the user asks to calculate, compute, or mentions operations like add, subtract, multiply, and divide.
- **[precision-calc](skills/precision-calc)**
  - **Description**: Use this skill for all types of calculations, including arithmetic, finance, science, unit conversions, and everyday math to ensure accuracy.
- **[lifecycle-carbon-calculator](skills/lifecycle-carbon-calculator)**
  - **Description**: Calculate the embodied carbon and lifecycle emissions for construction materials and projects to support sustainable design decisions.
- **[math-formula-calculator](skills/math-formula-calculator)**
  - **Description**: Math formula calculator - excels in parsing, step-by-step computation, and boundary validation. Ideal for bid pricing and solving complex formulas.
- **[earthquake-monitor](skills/earthquake-monitor)**
  - **Description**: Real-time earthquake monitoring for China, Taiwan, and Japan with proactive alerts, using CENC, CWA, and JMA WebSocket data.
- **[survival-analysis-km](skills/survival-analysis-km)**
  - **Description**: Generates Kaplan-Meier survival curves and calculates survival statistics.
### Biology & Medicine

- **[krumpphysio](skills/krumpphysio)**
  - **Description**: This AI skill plugin trains OpenClaw agents to serve as Krump-inspired physiotherapy coaches, offering therapeutic movement scoring, rehab coaching with gamified Krump vocabulary and Laban notation, and optional Canton ledger logging. It supports health and wellbeing initiatives by adapting authentic Krump for physiotherapy.
- **[ocd-erp-therapist](skills/ocd-erp-therapist)**
  - **Description**: An OpenClaw skill for conducting OCD Exposure and Response Prevention (ERP) therapy sessions, featuring an inhibitory learning framework, automated check-ins, progress tracking, and safety protocols.
- **[bmi-calculator](skills/bmi-calculator)**
  - **Description**: A BMI calculator that provides ideal weight, health plans, and tracks weight. It also calculates and interprets BMI for children.
- **[quantinuumclaw](skills/quantinuumclaw)**
  - **Description**: The quantinuumclaw plugin facilitates the development and deployment of quantum computing applications using Quantinuum, Guppy, Selene, and Fly.io. It is ideal for healthcare projects, including drug discovery and treatment optimization, as well as for creating quantum-powered web apps and integrating results into user interfaces.
- **[quantum](skills/quantum)**
  - **Description**: This plugin facilitates the creation and deployment of quantum computing applications using platforms like Quantinuum, Guppy, Selene, and Fly.io. It is ideal for healthcare projects, including drug discovery and treatment optimization, as well as for building and deploying quantum-powered web applications.
- **[afrexai-medical-billing](skills/afrexai-medical-billing)**
  - **Description**: Optimizes medical billing workflows, reduces claim denials, and identifies revenue leaks for healthcare practices, billing companies, and revenue cycle teams.
- **[afrexai-pharmacy-compliance](skills/afrexai-pharmacy-compliance)**
  - **Description**: Assist pharmacists, pharmacy managers, and compliance officers in navigating DEA, Board of Pharmacy, USP, DSCSA, and PBM requirements.
- **[clinical-data-extractor](skills/clinical-data-extractor)**
  - **Description**: Extract and structure clinical trial data from pharmaceutical conference websites or PDFs, including drug name, manufacturer, indication, clinical phase, trial name, conference, and efficacy and safety data, outputting to a markdown file.
- **[medical](skills/medical)**
  - **Description**: Manage personal health records with strict privacy, including tracking symptoms, medications, and vital signs, and preparing for doctor visits. Do not use for diagnosis or treatment advice.
- **[healthie](skills/healthie)**
  - **Description**: Healthie is a tool for managing patients, appointments, goals, and documents through a GraphQL API.
- **[medical-record-structurer](skills/medical-record-structurer)**
  - **Description**: A tool that converts oral or handwritten medical records into standardized electronic medical records, supporting voice and text input with automatic field recognition and structured output. It includes pay-per-use monetization via skillpay.me.
- **[biorxiv-openclaw-skill](skills/biorxiv-openclaw-skill)**
  - **Description**: Access the bioRxiv preprint repository to fetch recent biology preprints, search by date range or category, and retrieve paper metadata such as titles, authors, DOIs, and more.
- **[medical-entity-extractor](skills/medical-entity-extractor)**
  - **Description**: Extracts medical entities such as symptoms, medications, lab values, and diagnoses from patient messages.
- **[medical-triage](skills/medical-triage)**
  - **Description**: Classify medical messages as critical, urgent, or routine based on their level of medical urgency.
- **[lobster-bio-dev](skills/lobster-bio-dev)**
  - **Description**: Contribute to Lobster AI, a multi-agent bioinformatics engine, by developing agents, creating services, understanding its architecture, fixing bugs, or adding features. Ideal for those working on the Lobster codebase or participating in the open-source project.
- **[lobster-bio-use](skills/lobster-bio-use)**
  - **Description**: Lobster AI skill analyzes biological data, including single-cell and bulk RNA-seq, literature mining, and dataset discovery, with features for quality control, clustering, marker identification, differential expression, and visualization.
- **[lobsterbio-use](skills/lobsterbio-use)**
  - **Description**: The 'lobsterbio-use' AI skill plugin performs comprehensive bioinformatics analysis, including single-cell and bulk RNA-seq, genomics, proteomics, metabolomics, machine learning, drug discovery, literature and dataset search, and visualization. It supports various data formats and accessions from major biological databases.
- **[pharma-pharmacology-agent](skills/pharma-pharmacology-agent)**
  - **Description**: This pharmacology agent evaluates drug candidates from SMILES, providing ADME/PK profiling, drug-likeness scores, and PAINS alerts. It predicts properties like BBB permeability, solubility, and CYP3A4 inhibition.
- **[pharmaclaw-alphafold-agent](skills/pharmaclaw-alphafold-agent)**
  - **Description**: This AI skill plugin retrieves protein structures from public PDB/AlphaFold databases, predicts folds using ESMFold, detects binding sites, and performs basic molecular docking with RDKit. It integrates with Chemistry Query for SMILES-based docking and supports IP expansion and catalyst design.
- **[pharmaclaw-literature-agent](skills/pharmaclaw-literature-agent)**
  - **Description**: The pharmaclaw-literature-agent v2.0.0 aids in novel drug discovery by mining literature from PubMed, Semantic Scholar, and bioRxiv, with a focus on Clinical Trials Phase II/III. It provides structured results including novelty scores, titles, authors, abstracts, DOIs, MeSH terms, and citation counts.
- **[pharmaclaw-pharmacology-agent](skills/pharmaclaw-pharmacology-agent)**
  - **Description**: This pharmacology agent evaluates drug candidates from SMILES, providing ADME/PK profiling, drug-likeness scores, and PAINS alerts.
- **[pharmaclaw-tox-agent](skills/pharmaclaw-tox-agent)**
  - **Description**: This AI skill plugin, named 'pharmaclaw-tox-agent', evaluates the safety of pharmaceutical drugs from their SMILES notation by calculating key ADMET descriptors, checking for chemical rule violations, and assessing drug-likeness. It outputs a risk classification along with a detailed property report, and suggests safer derivatives.
- **[clarity-clinical](skills/clarity-clinical)**
  - **Description**: Query clinical variant data from ClinVar and gnomAD using the Clarity Protocol. This skill provides detailed variant annotations, including clinical significance, pathogenicity, and population genetics.
- **[bioskills](skills/bioskills)**
  - **Description**: This plugin installs 425 bioinformatics skills across various categories including sequence analysis, RNA-seq, single-cell, variant calling, metagenomics, and structural biology. Ideal for setting up bioinformatics capabilities or handling specialized tasks.
- **[tnbc-research-swarm](skills/tnbc-research-swarm)**
  - **Description**: Contribute to the TNBC Research Swarm by registering as an agent, receiving and completing research or QC review tasks, and submitting findings from open-access databases on topics like demographics, drug resistance, subtypes, genetics, biomarkers, and diagnostics.
- **[research-automation](skills/research-automation)**
  - **Description**: Automated web research tool for peptides, biohacking, longevity science, and trending health topics. Ideal for discovering new information, tracking trends, monitoring scientific updates, or generating content ideas. Can run periodically or on-demand.
- **[neuralink-decoder](skills/neuralink-decoder)**
  - **Description**: Simulates and decodes neural spike activity to control cursor movement (BCI).
- **[intelligent-triage-symptom-analysis](skills/intelligent-triage-symptom-analysis)**
  - **Description**: This AI skill plugin offers intelligent triage and symptom analysis, supporting over 650 symptoms across 11 body systems with a 5-level classification. It features NLP for symptom extraction, a 3000+ disease database, and a red flag warning system for life-threatening conditions, all enhanced by machine learning.
- **[clarity-analyze](skills/clarity-analyze)**
  - **Description**: Use Clarity Protocol to submit research questions for AI analysis, ideal for analyzing protein variants, mutations, or querying aggregated data. Requires CLARITY_WRITE_API_KEY.
- **[clarity-fold-status](skills/clarity-fold-status)**
  - **Description**: Retrieve an overview and status from Clarity Protocol, including variant counts and data availability. Useful for inquiries about fold status, research summary, or API information.
- **[clarity-research](skills/clarity-research)**
  - **Description**: Search Clarity Protocol for protein folding research data, including variants, fold results, and disease-specific information. Capabilities include listing variants by disease or protein name and providing API details.
### Chemistry & Materials

- **[pharmaclaw-catalyst-design](skills/pharmaclaw-catalyst-design)**
  - **Description**: This AI skill plugin recommends organometallic catalysts for various drug synthesis reactions and designs novel ligands using RDKit. It supports a range of reaction types and catalysts, offering suggestions from a curated database with scoring.
- **[pharmaclaw-cheminformatics](skills/pharmaclaw-cheminformatics)**
  - **Description**: An advanced cheminformatics tool for 3D molecular analysis, pharmacophore mapping, format conversion, RECAP fragmentation, and stereoisomer enumeration, ideal for tasks like 3D conformer generation and library design.
- **[materials-science-figure-skill](skills/materials-science-figure-skill)**
  - **Description**: Use this skill to generate or edit publication-style figures, such as materials-science paper schematics, using Google's Nanobanana/Gemini image models. It is ideal for text-to-image, image editing, and multi-reference workflows.
- **[pharmaclaw-chemistry-query](skills/pharmaclaw-chemistry-query)**
  - **Description**: This AI skill plugin, pharmaclaw-chemistry-query, facilitates PubChem API queries for compound information and properties, as well as RDKit cheminformatics for SMILES processing, molecular property analysis, and synthesis route planning.
- **[chemistry-query](skills/chemistry-query)**
  - **Description**: This AI skill plugin, chemistry-query, leverages the PubChem API and RDKit for comprehensive chemical data analysis, including compound information, structure visualization, and synthesis route planning.
- **[paramus-chemistry](skills/paramus-chemistry)**
  - **Description**: A comprehensive suite of chemistry and scientific computing tools, including molecular weight calculation, LogP, TPSA, SMILES validation, thermodynamics, polymer analysis, electrochemistry, and DOE.
### Arts, Humanities & Social Sciences

- **[teacher-prep](skills/teacher-prep)**
  - **Description**: The Teacher-Prep assistant is designed for primary school Chinese language lesson planning, supporting various texts like ancient poems, modern literature, fables, and fairy tales. It automatically gathers relevant materials, creates markdown-based lesson plans, generates PPTs, and produces Word format exercises with answers.
- **[language-learning](skills/language-learning)**
  - **Description**: This AI language tutor helps you learn any language through conversation, vocabulary drills, grammar lessons, flashcards, and immersive practice, supporting all languages including Spanish, French, German, Japanese, Chinese (Mandarin/Cantonese), and Korean.
- **[japanese-tutor](skills/japanese-tutor)**
  - **Description**: An interactive Japanese learning assistant that offers vocabulary, grammar, quizzes, roleplay, and OCR translation. It also parses PDF and DOCX files for study and homework help.
- **[pronunciation-coach](skills/pronunciation-coach)**
  - **Description**: Pronunciation coaching with real voice analysis using Azure Speech Services, evaluating audio for phoneme accuracy, fluency, prosody, and intonation.
- **[book-language-tutor](skills/book-language-tutor)**
  - **Description**: Book language-tutor services via Lokuli MCP. Use this when looking to find and book a language tutor, especially for requests like 'book a language-tutor' or 'find a language-tutor near me'.
- **[english-tutor](skills/english-tutor)**
  - **Description**: This personalized American English tutor helps users improve their language skills.
- **[kindergarten-assistant](skills/kindergarten-assistant)**
  - **Description**: A specialized early childhood educator in the British EYFS framework and Reggio Emilia approach for children aged 45 days to 2 years, designing child-led activities, tracking developmental milestones, and supporting a nurturing environment and classroom management.
- **[voice-note-to-midi](skills/voice-note-to-midi)**
  - **Description**: Convert voice notes, humming, and melodic audio recordings into quantized MIDI files using ML-based pitch detection and intelligent post-processing.
- **[aiml-music-generator](skills/aiml-music-generator)**
  - **Description**: Generate high-quality music or songs using AIMLAPI, supporting various models like Suno, Udio, Minimax, and ElevenLabs. Ideal for requests with specific lyrics or styles.
- **[on-this-day-art](skills/on-this-day-art)**
  - **Description**: This AI skill generates daily images based on Wikipedia's 'On This Day' events using local ComfyUI, ideal for those seeking historical or artistic visuals. It does not use cloud APIs, generate videos, or support SD 3.5 due to laptop instability.
- **[zeelin-liberal-arts-paper](skills/zeelin-liberal-arts-paper)**
  - **Description**: An essential AI tool for liberal arts graduate students, offering comprehensive support in generating a thesis including the title, outline, introduction, literature review, arguments, suggestions, and conclusion, with an emphasis on theoretical depth and critical thinking. Customizable chapter numbers are supported.
- **[algorithmic-art-2](skills/algorithmic-art-2)**
  - **Description**: Create unique algorithmic art with p5.js, using seeded randomness and interactive parameter exploration. Ideal for generative art, flow fields, and particle systems.
- **[afrexai-photography-mastery](skills/afrexai-photography-mastery)**
  - **Description**: A comprehensive photography guide covering exposure, composition, lighting, genre-specific workflows, editing, gear selection, portfolio building, and client management, suitable for all levels from beginner to professional.
- **[torah-scholar](skills/torah-scholar)**
  - **Description**: Explore Jewish texts, including the Torah, Tanach, Talmud, Midrash, and commentaries, using the Sefaria API. Ideal for researching sources, finding verses, commentaries, and cross-references in Hebrew and English.
- **[gaokao-essay](skills/gaokao-essay)**
  - **Description**: A Gaokao essay assistant providing argumentative essay templates, materials, opening and closing lines, topic analysis techniques, and high-scoring essay reviews.
- **[short-drama-writer](skills/short-drama-writer)**
  - **Description**: Short Drama Writer: Use this skill for creating short dramas. It activates with the trigger 'short drama writer'.
- **[reading-knowledge](skills/reading-knowledge)**
  - **Description**: A knowledgeable companion for exploring space, the universe, and history. It answers questions without judgment, explains concepts clearly, and recommends educational resources.
### Computer Science & Engineering

- **[redux-saga-skill](skills/redux-saga-skill)**
  - **Description**: This plugin offers best practices, patterns, and API guidance for using Redux-Saga in Redux applications, including effect creators, fork model, channels, testing, concurrency, cancellation, and integration with modern Redux Toolkit.
- **[active-learner](skills/active-learner)**
  - **Description**: This plugin implements the Active Learning Protocol, enabling the agent to programmatically integrate lessons into `MEMORY.md` and generate structured feedback requests.
- **[acg-rust-teacher](skills/acg-rust-teacher)**
  - **Description**: An ACG-themed educational tool that uses anime analogies (like ReZero and Fate) to explain Rust's ownership system, making it easier to learn core concepts.
- **[iterative-code-evolution](skills/iterative-code-evolution)**
  - **Description**: Iteratively enhance code quality through structured analysis, mutation, and evaluation. Ideal for optimization, debugging, and evolving designs over multiple cycles, replacing ad-hoc methods with disciplined reflection and principled selection.
- **[coder-workspaces](skills/coder-workspaces)**
  - **Description**: Manage Coder workspaces and AI coding tasks via CLI. List, create, start, stop, and delete workspaces, or SSH into them to run commands. Monitor AI coding tasks with Claude Code, Aider, or other agents.
- **[claude-code-cli](skills/claude-code-cli)**
  - **Description**: Use Claude Code CLI for coding tasks like building features, reviewing PRs, or refactoring. It supports interactive and headless modes but isn't meant for simple fixes or reading code.
- **[ctf-writeup-generator](skills/ctf-writeup-generator)**
  - **Description**: Automatically generates professional CTF writeups, including flag detection, challenge categorization, and markdown formatting.
- **[cs-landing-page-generator](skills/cs-landing-page-generator)**
  - **Description**: This AI skill plugin generates high-converting landing pages as complete Next.js/React (TSX) components with Tailwind CSS, including essential sections and SEO optimization for Core Web Vitals.
- **[react-nextjs-generator](skills/react-nextjs-generator)**
  - **Description**: Generates a complete React + Next.js project based on requirement documents and UI design, using Ant Design, Tailwind CSS, and Zustand.
- **[sql-generator](skills/sql-generator)**
  - **Description**: SQL generator for natural language to SQL conversion, SQL explanation, optimization, DDL creation, mock data generation, and database migration scripts.
- **[quiverai-quickstart](skills/quiverai-quickstart)**
  - **Description**: A quick start guide for the QuiverAI SVG generation API, covering the entire process from creating an API key to configuring the environment, installing the SDK, and making requests.
- **[afrexai-code-reviewer](skills/afrexai-code-reviewer)**
  - **Description**: An enterprise-grade code review tool that identifies security vulnerabilities, performance issues, error handling gaps, architectural problems, and test coverage in PRs, diffs, or code files. It supports all languages and repositories without requiring any dependencies.
- **[q-kdb-code-review](skills/q-kdb-code-review)**
  - **Description**: AI-powered code review for Q/kdb+ to catch bugs in the tersest language used in finance.
- **[matic-mquant-assistant](skills/matic-mquant-assistant)**
  - **Description**: MQuant Python strategy development assistant that generates executable Python code for the MQuant platform.
- **[perry-workspaces](skills/perry-workspaces)**
  - **Description**: Create and manage isolated Docker workspaces on your tailnet, pre-installed with Claude Code and OpenCode, for use with coding agents or remote development environments.
- **[api-generator](skills/api-generator)**
  - **Description**: API code generator for creating RESTful endpoints, GraphQL schemas, OpenAPI/Swagger documentation, API clients, mock servers, authentication, rate limiting, and test suites. Ideal for backend development and API scaffolding.
- **[git-cmt-helper](skills/git-cmt-helper)**
  - **Description**: This skill generates standardized git commit messages following the Conventional Commits format, ensuring adherence to team conventions for type prefixes, scope, message length, and breaking change documentation.
- **[gitmap](skills/gitmap)**
  - **Description**: Version control for ArcGIS web maps, accessible through native OpenClaw tools.
- **[afrexai-claude-code-production](skills/afrexai-claude-code-production)**
  - **Description**: The Claude Code productivity system streamlines project setup, prompting patterns, sub-agent orchestration, context management, debugging, refactoring, TDD, and accelerates code delivery by 10X without requiring any scripts.
- **[afrexai-git-engineering](skills/afrexai-git-engineering)**
  - **Description**: This AI skill plugin, named 'afrexai-git-engineering', assists teams in designing branching strategies, implementing code review workflows, managing monorepos, automating releases, and maintaining scalable repository practices.
- **[afrexai-ml-engineering](skills/afrexai-ml-engineering)**
  - **Description**: A comprehensive methodology for building, deploying, and scaling production ML/AI systems from experimentation to full-scale operation.
- **[afrexai-performance-engineering](skills/afrexai-performance-engineering)**
  - **Description**: A comprehensive performance engineering solution for profiling, optimization, load testing, capacity planning, and fostering a performance culture. It supports Node.js, Python, Go, Java, databases, APIs, and frontend technologies.
- **[developer-agent](skills/developer-agent)**
  - **Description**: Manages software development by coordinating with the Cursor Agent, handling git workflows, and ensuring high-quality delivery through build verification and deployment pipelines.
- **[public-apis-skill-creator](skills/public-apis-skill-creator)**
  - **Description**: The Public APIs Skill Creator automatically retrieves free APIs from public-apis/public-apis, recommends them by functionality, and provides minimal working examples (curl/Python/JS). It can also generate custom-named API skills.
- **[code-quality-analyzer](skills/code-quality-analyzer)**
  - **Description**: A professional code quality analyzer offering static code analysis, detection of code smells, complexity assessment, and best practice recommendations for mainstream languages like JavaScript, TypeScript, Python, and Java.
- **[doro-docker-essentials](skills/doro-docker-essentials)**
  - **Description**: This plugin covers essential Docker commands and workflows for managing containers, handling images, and debugging.
- **[doro-git-essentials](skills/doro-git-essentials)**
  - **Description**: Essential Git commands and workflows for version control, branching, and collaboration.
- **[apple-developer-toolkit](skills/apple-developer-toolkit)**
  - **Description**: The Apple Developer Toolkit is an all-in-one solution with tools for searching documentation across Apple frameworks, symbols, and WWDC sessions, as well as a CLI with over 120 commands for App Store Connect, covering builds, TestFlight, submissions, and more.
- **[python](skills/python)**
  - **Description**: This plugin enforces Python coding best practices, including PEP 8 style, syntax validation, unit testing, and modern version usage. It also promotes idiomatic patterns and uses uv for dependency management when available.
- **[devboxes](skills/devboxes)**
  - **Description**: Manage development environment containers with web-accessible VSCode, VNC, and app routing via Traefik or Cloudflare Tunnels. Use this skill to create, start, stop, list, or manage dev environments, or for initial setup.
- **[azure-devops-mcp-replacement-for-openclaw](skills/azure-devops-mcp-replacement-for-openclaw)**
  - **Description**: Interact with Azure DevOps through direct REST API calls to manage and query projects, teams, repos, work items, sprints, pipelines, builds, test plans, and wikis.
- **[a6-github-intel](skills/a6-github-intel)**
  - **Description**: Analyze GitHub repositories by converting them into single markdown documents, generating architecture diagrams, and providing insights like structure trees, language breakdowns, and recent activity. Designed for AI with Python stdlib, it includes advanced search techniques and API shortcuts, all without executing any code.
- **[chrome-devtools-mcp](skills/chrome-devtools-mcp)**
  - **Description**: Chrome DevTools MCP is Google's official server for browser automation and testing, enabling control over Chrome via Puppeteer with features like navigation, form filling, screenshots, and performance analysis.
- **[github-intel](skills/github-intel)**
  - **Description**: Analyze GitHub repositories by converting them into AI-friendly formats, including single markdown documents and architecture diagrams. It also provides repository structure, language breakdowns, and recent activity summaries, all without executing any code from the repositories.
- **[mac-mini-server](skills/mac-mini-server)**
  - **Description**: Set up an always-on AI server with OpenClaw on Mac Mini, including hardware recommendations, macOS configuration, Docker Desktop setup, launchd auto-start, Tailscale for remote access, and a cost comparison with VPS.
- **[api-design-reviewer](skills/api-design-reviewer)**
  - **Description**: The API Design Reviewer skill plugin evaluates and provides feedback on the design of APIs to ensure they are efficient, secure, and maintainable.
- **[code-reviewer-2](skills/code-reviewer-2)**
  - **Description**: Automates code reviews for TypeScript, JavaScript, Python, Go, Swift, and Kotlin. Analyzes pull requests for complexity, risk, and code quality, identifying SOLID violations and code smells, and generates review reports.
- **[codebase-onboarding](skills/codebase-onboarding)**
  - **Description**: The Codebase Onboarding tool helps new team members quickly understand and navigate the project's code, accelerating their integration into the development process.
- **[cs-code-reviewer](skills/cs-code-reviewer)**
  - **Description**: Automates code reviews for TypeScript, JavaScript, Python, Go, Swift, and Kotlin, analyzing pull requests for complexity, risk, and code quality, and generating detailed review reports.
- **[git-worktree-manager](skills/git-worktree-manager)**
  - **Description**: The Git Worktree Manager is a tool for managing multiple working directories linked to a single repository, allowing you to work on different branches simultaneously.
- **[mcp-server-builder](skills/mcp-server-builder)**
  - **Description**: MCP Server Builder is a tool for creating and managing servers, streamlining the setup process with customizable configurations.
- **[senior-devops](skills/senior-devops)**
  - **Description**: This AI skill plugin provides comprehensive DevOps capabilities, including CI/CD, infrastructure automation, containerization, and cloud platform management. It supports pipeline setup, IaC, deployment, and monitoring.
- **[senior-ml-engineer](skills/senior-ml-engineer)**
  - **Description**: This skill covers deploying ML models, setting up MLOps infrastructure, monitoring model performance, building RAG pipelines, and integrating LLMs with cost controls.
- **[context7-api](skills/context7-api)**
  - **Description**: Use the Context7 API to fetch current library documentation when working with external libraries, implementing third-party package features, debugging library issues, or needing up-to-date information beyond the training data cutoff.
- **[read-github](skills/read-github)**
  - **Description**: The 'read-github' skill plugin allows for semantic search and smart code navigation across GitHub repositories, providing a clean, aggregated view of READMEs, documentation, and code, all while respecting rate limits and robots.txt.
- **[senior-django-developer](skills/senior-django-developer)**
  - **Description**: Expert in high-performance, containerized, and async-capable Django architectures, producing secure, statically typed, and production-ready code with a strict layered design, comprehensive testing, and ASGI-first deployment.
- **[github-automation-pro](skills/github-automation-pro)**
  - **Description**: This plugin automates GitHub tasks, enhancing productivity and streamlining workflows.
- **[task-development-workflow](skills/task-development-workflow)**
  - **Description**: A TDD-first development workflow featuring structured planning, Trello task management, and PR-based code reviews, ideal for projects requiring phased approvals and Git branching policies.
- **[github-analyzer](skills/github-analyzer)**
  - **Description**: Input a project idea or GitHub link to automatically search for related open-source projects, generate a structured analysis report (including tech stack, pros and cons, and ratings), and download the top 3 highest-rated code packages. Supports intent-based search and direct link analysis.
- **[github-to-clawhub](skills/github-to-clawhub)**
  - **Description**: This AI skill plugin, 'github-to-clawhub', automates the process of converting a GitHub open-source project into an OpenClaw skill and publishing it to Clawhub. It handles everything from analyzing the README, checking for duplicates on Clawhub, writing the SKILL.md file, creating the directory structure, to finally publishing the skill.
- **[ipfs-server](skills/ipfs-server)**
  - **Description**: This plugin offers full IPFS node operations including installation, configuration, content pinning, IPNS publishing, peer management, and gateway services.
- **[devops-bridge](skills/devops-bridge)**
  - **Description**: The devops-bridge skill integrates GitHub, CI/CD, Slack, Discord, and issue trackers into automated workflows, providing CI failure notifications, PR review reminders, and repository health monitoring. It streamlines development processes by connecting these tools for seamless communication and collaboration.
- **[docker-essentials](skills/docker-essentials)**
  - **Description**: Essential Docker commands and workflows for managing containers, handling images, and debugging.
- **[git-essentials](skills/git-essentials)**
  - **Description**: Master essential Git commands and workflows for version control, branching, and collaboration.
- **[github-issue-resolver](skills/github-issue-resolver)**
  - **Description**: This AI skill plugin, the GitHub Issue Resolver, autonomously discovers, analyzes, and fixes open issues in GitHub repositories, supporting the full workflow from issue detection to PR submission with safety measures to prevent scope creep and unauthorized actions.
- **[xcloud-docker-deploy](skills/xcloud-docker-deploy)**
  - **Description**: The xCloud Docker Deploy plugin automatically detects your project's stack (e.g., WordPress, Laravel, Node.js) and deploys it to xCloud, generating production-ready Docker configurations, CI/CD workflows, and environment files.
- **[devvit-publishing-auditor](skills/devvit-publishing-auditor)**
  - **Description**: A specialized tool for Reddit Devvit developers to audit and ensure their apps meet all requirements before uploading to Reddit servers.
- **[gitcode](skills/gitcode)**
  - **Description**: Fetch and query data from the GitCode platform using its REST API, including repositories, branches, issues, pull requests, commits, tags, users, organizations, and more. Compatible with Python 3.7+ standard library.
- **[claude-code-usage](skills/claude-code-usage)**
  - **Description**: Check Claude Code OAuth usage limits, including session and weekly quotas. It also provides automated reminders for session refresh and monitors reset detection.
- **[fullstack-developer](skills/fullstack-developer)**
  - **Description**: This skill offers comprehensive full-stack development expertise, including frontend, backend, database management, API design, DevOps, and architecture. It's ideal for building, fixing, reviewing, or debugging any web application.
- **[code-quality-guard](skills/code-quality-guard)**
  - **Description**: Ensures code quality before deployment by validating imports, checking for closed tags, and enforcing best practices in logic.
- **[devtools-secrets](skills/devtools-secrets)**
  - **Description**: This plugin provides knowledge and guidelines for setting up and managing secrets using the Mise, Fnox, and Infisical toolchain. It is useful for configuring secrets, environment variables, and ensuring secure secret management practices.
- **[astrai-code-review](skills/astrai-code-review)**
  - **Description**: AI-powered code review with intelligent model routing, saving over 40% compared to always using the most expensive model.
- **[coder-helper](skills/coder-helper)**
  - **Description**: Describe your requirements in natural language, and the tool will automatically generate a requirements document and open it in an editor.
- **[deepwiki](skills/deepwiki)**
  - **Description**: Query the DeepWiki MCP server for GitHub repository documentation, wiki structure, and AI-generated questions.
- **[reporead](skills/reporead)**
  - **Description**: Analyze GitHub repositories with RepoRead AI for tasks like generating documentation, conducting security audits, or creating a README. Supports MCP server integration and REST API.
- **[task-review-workflow](skills/task-review-workflow)**
  - **Description**: This AI skill plugin streamlines the PR review and merge process for task-driven development, facilitating decisions on merging or requesting changes, and handling post-merge actions like Trello updates and branch cleanup.
- **[runtime-debug-skill](skills/runtime-debug-skill)**
  - **Description**: Diagnose and fix bugs in Python, Node.js, or Java applications using runtime execution traces. Ideal for debugging errors, analyzing failures, and identifying root causes.
- **[runtime-debugging-skill](skills/runtime-debugging-skill)**
  - **Description**: Diagnose and fix bugs in Python, Node.js, or Java applications using runtime execution traces. Ideal for debugging errors, analyzing failures, and identifying root causes.
- **[sql-query-generator](skills/sql-query-generator)**
  - **Description**: Generate secure SQL queries with built-in validation, pagination support, risk analysis, and audit-focused safeguards.
- **[database-schema-designer](skills/database-schema-designer)**
  - **Description**: The Database Schema Designer is a tool for creating, visualizing, and managing database schemas efficiently.
- **[schema-builder](skills/schema-builder)**
  - **Description**: A database schema designer for creating table structures, generating SQL DDL, migration scripts, seed data, ER diagrams, optimization reports, NoSQL schemas, and schema diffs. Use it for comprehensive database design and management.
- **[database-schema-differ](skills/database-schema-differ)**
  - **Description**: Compare database schemas across environments, generate migration scripts, and track schema evolution.
- **[afrexai-database-engineer](skills/afrexai-database-engineer)**
  - **Description**: A comprehensive system for database design, optimization, migration, and operations, covering PostgreSQL, MySQL, SQLite, and general SQL patterns.
- **[tg-mysql-design](skills/tg-mysql-design)**
  - **Description**: A MySQL table design assistant that generates Alibaba-compliant DDL statements for MySQL 5.7/8.0 based on business rule documents and existing SQL scripts. It supports .md and .sql file inputs, producing RDS-standard table designs.
- **[xcode-build-analyzer](skills/xcode-build-analyzer)**
  - **Description**: Analyze Xcode build logs for timing, warnings, errors, slow compiles, and build history from DerivedData.
- **[database-designer](skills/database-designer)**
  - **Description**: Database Designer is a powerful tool for creating and managing database schemas efficiently.
- **[project-deep-analyzer](skills/project-deep-analyzer)**
  - **Description**: This skill provides in-depth analysis of a project's system boundaries, core concepts, module architecture, key algorithms, and technology choices, aiding in codebase understanding and troubleshooting.
- **[tech-data-playbook](skills/tech-data-playbook)**
  - **Description**: The Tech & Data Playbook offers best practices and strategies for a wide range of technology areas including software development, IT infrastructure, cybersecurity, data analytics, cloud computing, AI/ML, and digital transformation. It's your go-to for any discussion on technology strategy, engineering, or data platforms.
- **[deepwiki-mcp](skills/deepwiki-mcp)**
  - **Description**: Use DeepWiki MCP to get AI-generated insights about any public GitHub repository, including details on source code, architecture, and configuration. Trigger with phrases like 'how does X work in <repo>', 'deepwiki', or 'look up in codebase'.
- **[cron-scheduling](skills/cron-scheduling)**
  - **Description**: Manage and schedule recurring tasks using cron and systemd timers, including timezone-aware scheduling, monitoring, retry patterns, and debugging.
- **[cs-google-workspace-cli](skills/cs-google-workspace-cli)**
  - **Description**: Manage Google Workspace with the gws CLI, including Gmail, Drive, Sheets, Calendar, Docs, Chat, and Tasks. Automate tasks, run security audits, and utilize 43 built-in recipes and 10 persona bundles.
- **[smart-model-switcher-v2](skills/smart-model-switcher-v2)**
  - **Description**: The Optimized Smart Model Switcher (v2) automatically selects the best model for each task from your plan with zero latency and no restart required, supporting auto-detection of new models, multi-model parallel processing, and intelligent task classification.
- **[smart-model-switcher-v3](skills/smart-model-switcher-v3)**
  - **Description**: Universal Smart Model Switcher V3 intelligently selects the best model from all your purchased API plans, supporting over 50 models with zero-latency switching and advanced task handling.
- **[jules-api](skills/jules-api)**
  - **Description**: Manage Google Jules AI coding sessions using the Jules REST API. Initiate tasks, track progress, approve plans, communicate, and access session details and artifacts.
### Data & Analysis

- **[botlearn-assessment](skills/botlearn-assessment)**
  - **Description**: BotLearn-assessment evaluates a bot's capabilities across five dimensions: reasoning, retrieval, creation, execution, and orchestration. It can be triggered manually or scheduled for periodic reviews.
- **[deepread-ocr](skills/deepread-ocr)**
  - **Description**: DeepRead is an AI-native OCR platform that converts documents into highly accurate data within minutes, achieving over 97% accuracy and reducing manual review to just 5-10% by flagging only uncertain fields for human inspection.
- **[music-analysis](skills/music-analysis)**
  - **Description**: Analyze local music/audio files to extract features like tempo, groove, stability, structure, and emotional tone, integrating lyrics for a more nuanced emotional read.
- **[fenge-smart-search](skills/fenge-smart-search)**
  - **Description**: A smart search tool that automatically selects the best search engine: Bing for Chinese and DuckDuckGo for English. Free to use with no API key required.
- **[afrexai-data-engineering](skills/afrexai-data-engineering)**
  - **Description**: A comprehensive guide for designing, building, operating, and scaling data pipelines and infrastructure with no external dependencies.
- **[senior-data-engineer](skills/senior-data-engineer)**
  - **Description**: This AI skill specializes in building scalable data pipelines and ETL/ELT systems, with expertise in Python, SQL, Spark, Airflow, dbt, Kafka, and the modern data stack. It covers data modeling, pipeline orchestration, data quality, and DataOps, ideal for designing data architectures and optimizing workflows.
- **[code-stats](skills/code-stats)**
  - **Description**: Visualizes project complexity by counting files, lines of code, and grouping them by file extension, aiding in assessing project size or growth.
- **[deepread-agent-setup](skills/deepread-agent-setup)**
  - **Description**: Authenticate AI agents with the DeepRead OCR API via OAuth device flow, where the user approves a code in their browser, and the agent receives a DEEPREAD_API_KEY stored as an environment variable.
- **[jina-reader](skills/jina-reader)**
  - **Description**: The Jina AI Reader API extracts web content in three modes: read (URL to markdown), search (web search + full content), and ground (fact-checking). It delivers clean content without exposing the server IP.
- **[sql-to-bi-builder](skills/sql-to-bi-builder)**
  - **Description**: Convert a markdown file with SQL queries into a BI dashboard specification and UI scaffold, including query parsing, metric/dimension inference, chart recommendation, filter design, and layout generation.
- **[afrexai-data-analyst](skills/afrexai-data-analyst)**
  - **Description**: As a senior data analyst, your role is to uncover the narrative within the data and present it clearly to inform the next steps.
- **[afrexai-data-governance](skills/afrexai-data-governance)**
  - **Description**: Evaluate, score, and improve your organization's data governance across six key areas.
- **[afrexai-data-privacy](skills/afrexai-data-privacy)**
  - **Description**: The afrexai-data-privacy skill ensures user data is protected and managed according to privacy standards, safeguarding information from unauthorized access.
- **[estat-mcp](skills/estat-mcp)**
  - **Description**: Retrieve Japanese government statistics on population, GDP, CPI, trade, and employment from e-Stat, Japan's official open data portal, which offers over 3,000 statistical tables. Free API access.
- **[senior-data-scientist](skills/senior-data-scientist)**
  - **Description**: This AI skill plugin specializes in advanced data science, including statistical modeling, experiment design, causal inference, and predictive analytics, with expertise in A/B testing, feature engineering, model evaluation, and MLflow tracking using Python, R, and SQL.
- **[dataset-finder](skills/dataset-finder)**
  - **Description**: Use this skill to search for, download, and explore datasets from repositories like Kaggle, UCI ML, Data.gov, or Hugging Face. It also supports previewing dataset statistics and generating data cards.
- **[simple-excel](skills/simple-excel)**
  - **Description**: A simple tool for handling Excel files, supporting .xlsx and .csv formats. It is ideal for basic data operations such as reading, editing, and generating tables.
- **[csv-wizard](skills/csv-wizard)**
  - **Description**: An interactive CLI for data cleaning, featuring automatic type inference, handling of missing values, and duplicate detection.
- **[expanso-csv-to-json](skills/expanso-csv-to-json)**
  - **Description**: Converts CSV data into a JSON array of objects.
- **[expanso-json-to-csv](skills/expanso-json-to-csv)**
  - **Description**: Converts a JSON array of objects into CSV format.
- **[ai-data-analysis](skills/ai-data-analysis)**
  - **Description**: This command runs a data analysis on the 'data.csv' file, focusing specifically on sales trends.
- **[csv-analyzer-cn](skills/csv-analyzer-cn)**
  - **Description**: Use this plugin for analyzing CSV files with Chinese content.
- **[microsoft-excel](skills/microsoft-excel)**
  - **Description**: Integrate with Microsoft Excel API to read and write workbooks, manage data, and access cell values in OneDrive. Use this skill for spreadsheet modifications and data management.
- **[analyse-data](skills/analyse-data)**
  - **Description**: The 'analyse-data' skill offers data analysis, interpretation, and visualization, including statistical calculations, trend analysis, and chart generation.
- **[analysis-data](skills/analysis-data)**
  - **Description**: The 'analysis-data' skill offers data analysis, interpretation, and visualization, including statistical calculations, trend analysis, and chart generation.
- **[data-analysis-pro](skills/data-analysis-pro)**
  - **Description**: The Data Analysis Pro skill offers data analysis, interpretation, and visualization. It supports tasks like calculating statistics, analyzing trends, and generating charts.
- **[data-ground-truth](skills/data-ground-truth)**
  - **Description**: Before presenting numbers in reports or recommendations, verify their accuracy and compare them against industry standards.
- **[nexus-data-profile](skills/nexus-data-profile)**
  - **Description**: This AI skill plugin performs statistical profiling and quality assessment of datasets.
- **[csv-handler](skills/csv-handler)**
  - **Description**: Process CSV files from construction software, automatically detecting delimiters and encodings, and cleaning up messy data.
- **[data-evolution-analysis](skills/data-evolution-analysis)**
  - **Description**: Analyze the evolution of data patterns in construction organizations and assess their digital maturity and data strategy.
- **[data-lineage-tracker](skills/data-lineage-tracker)**
  - **Description**: Track the origin, transformations, and flow of data through systems for audit trails, compliance, and debugging.
- **[pdf-ocr-layout](skills/pdf-ocr-layout)**
  - **Description**: A deep analysis tool for multimodal documents, leveraging Zhipu GLM-OCR, GLM-4.7, and GLM-4.6V.
- **[recursive-knowledge-miner](skills/recursive-knowledge-miner)**
  - **Description**: Professional multi-layered knowledge extraction and recursive knowledge graph construction.
- **[xml-reader](skills/xml-reader)**
  - **Description**: This AI skill reads and parses XML files from various construction systems such as P6 schedules, BSDD exports, IFC-XML, and COBie-XML, converting them into pandas DataFrames.
- **[geminipdfocr](skills/geminipdfocr)**
  - **Description**: Extract text from PDFs and perform OCR on scanned or image-based documents using Google Gemini OCR.
- **[summary](skills/summary)**
  - **Description**: Summarize content from URLs or files, including web pages, PDFs, images, audio, and YouTube videos, using the summarize CLI.
- **[summarize-1-0-0](skills/summarize-1-0-0)**
  - **Description**: Summarize content from URLs or files, including web pages, PDFs, images, audio, and YouTube videos, using the summarize CLI.
- **[smart-summarizer](skills/smart-summarizer)**
  - **Description**: Effortlessly summarize articles, PDFs, YouTube videos, web pages, and more. Extract key points, action items, and insights for quick digestion or meeting notes.
- **[seek-and-analyze-video](skills/seek-and-analyze-video)**
  - **Description**: Analyze and discover videos from platforms like TikTok, YouTube, and Instagram. Summarize content, create searchable knowledge bases, and use for research or meeting notes.
- **[deepwiki-ask](skills/deepwiki-ask)**
  - **Description**: Query a repository with a single question via DeepWiki by providing the owner/repo and your question.
- **[gws-sheets-read](skills/gws-sheets-read)**
  - **Description**: Read values from a Google Sheets spreadsheet.
### Visual & Presentation

- **[ppt-compress](skills/ppt-compress)**
  - **Description**: Compress PPT/PPTX files by reducing image sizes and converting to PDF, ideal for sharing or uploading large presentations.
- **[md-ppt-generator](skills/md-ppt-generator)**
  - **Description**: Creative director for tech product launches, transforming structured Markdown into visually striking, minimalist 'big-character' style HTML slides, with a focus on cinematic dark gradients, Morandi color scheme text, and 'breathing' motion effects.
- **[excalidraw-diagram](skills/excalidraw-diagram)**
  - **Description**: Generate Excalidraw diagrams from text, supporting Obsidian (.md), Standard (.excalidraw), and Animated (.excalidraw with animation) formats. Triggered by keywords like 'Excalidraw', 'diagram', or 'animate'.
- **[slide-maker](skills/slide-maker)**
  - **Description**: A tool for generating presentation outlines, full slide decks, speaker notes, and design recommendations, outputting in Markdown format.
- **[z-article-card](skills/z-article-card)**
  - **Description**: A tool that converts long articles into multiple PNG images, each representing a page of the article.
- **[long-article-illustration](skills/long-article-illustration)**
  - **Description**: The long-article-illustration plugin automatically divides long articles into paragraphs, generates AI image prompts, and creates illustrations using an image generation tool. It is ideal for blog posts, user-uploaded articles, and batch illustration creation.
- **[article-to-video-script](skills/article-to-video-script)**
  - **Description**: Transform articles, research reports, and long-form content into structured video scripts with HOOK, BODY, and LIGHT CTA sections, suitable for short (up to 90 seconds) or long (about 10 minutes) creator commentary.
- **[comman-felo-slides](skills/comman-felo-slides)**
  - **Description**: This plugin generates PPTs or slide decks using the Felo PPT Task API in Claude Code. It handles API key checks, task creation, polling, and provides the final ppt_url.
- **[dragon-ppt-maker](skills/dragon-ppt-maker)**
  - **Description**: Create stylish PPTs with python-pptx, supporting tech-themed designs, mixed text and images, and HTML content embedding.
- **[image-read](skills/image-read)**
  - **Description**: Use the free multimodal API of Zhipu AI's GLM-4V-Flash to understand and describe image content, and identify objects within images.
- **[chart-generator](skills/chart-generator)**
  - **Description**: A data visualization tool that generates SVG charts, including bar, line, pie, and more. Ideal for creating visual representations from raw numerical data.
- **[diagrams-generator-pro](skills/diagrams-generator-pro)**
  - **Description**: Generate professional diagrams such as cloud architecture, data charts, and academic figures. It can be triggered by requests like 'create diagram' or 'visualize data', or when users provide a sketch or image for professional recreation.
- **[table-image-generator](skills/table-image-generator)**
  - **Description**: Generate clean table images from data, ideal for platforms like Discord and Telegram. Supports dark/light mode, custom styling, and auto-sizing without needing Puppeteer.
- **[infographic-generation](skills/infographic-generation)**
  - **Description**: Create professional infographics optimized for visual communication, including statistical, process, comparison, timeline, list, geographic, hierarchical, resume, report, and social media types.
- **[chart-splat](skills/chart-splat)**
  - **Description**: Generate visually appealing charts, including line, bar, pie, doughnut, radar, polar area, and candlestick/OHLC types, using the Chart Splat API. The output is in PNG format.
- **[chart-image](skills/chart-image)**
  - **Description**: Generate high-quality chart images from data, supporting various types like line, bar, and pie charts. Ideal for data visualization and report generation, this plugin is designed for Fly.io/VPS deployments with no need for native compilation or a browser, using pure Node.js with prebuilt binaries.
- **[article-to-infographic](skills/article-to-infographic)**
  - **Description**: Transform text content into visually appealing HTML infographics, supporting various styles like timelines, statistics, and process flows.
- **[prd-visualization-skill](skills/prd-visualization-skill)**
  - **Description**: This AI skill plugin creates interactive D3.js visualizations for hierarchical data, including PRDs, org charts, and file structures, with multiple view modes like List, Force-Directed, and Radial Cluster.
- **[obsidian-cloudflare-pages-skill](skills/obsidian-cloudflare-pages-skill)**
  - **Description**: Publish selected Obsidian markdown files from your vault to a static site and deploy them to Cloudflare Pages.
- **[openclaw-skill-obsidian-cloudflare-pages](skills/openclaw-skill-obsidian-cloudflare-pages)**
  - **Description**: Publish selected Obsidian markdown files from your vault to a static site and deploy them to Cloudflare Pages.
- **[smart-illustrator](skills/smart-illustrator)**
  - **Description**: A smart illustrator for generating illustrations, infographics, and cover images. It supports article illustration, bulk PPT/slide infographics, and cover image creation, with an option to output prompts only. Bento Grid style is also supported.
- **[mermaid-architect](skills/mermaid-architect)**
  - **Description**: Create elegant, hand-drawn Mermaid diagrams with advanced syntax features like quoted labels and ELK layout. Use this skill for requests related to diagrams, flowcharts, or visualizing processes.
- **[slide-sniper](skills/slide-sniper)**
  - **Description**: Monitors full-screen videos or live streams, detects slide changes using visual models, and automatically captures, extracts, and formats the text into note-taking software.
- **[mermaid-visualizer](skills/mermaid-visualizer)**
  - **Description**: Transform text into professional Mermaid diagrams for presentations and documentation, supporting process flows, system architectures, comparisons, mind maps, and more with built-in syntax error prevention.
- **[ppt-outline](skills/ppt-outline)**
  - **Description**: This AI skill plugin generates PPT outlines and standalone HTML presentations, suitable for creating pitch decks, business plans, work reports, training materials, and more. It's perfect for structuring your content and can be opened directly in any browser without additional software.
- **[google-slides](skills/google-slides)**
  - **Description**: Integrate with Google Slides API using managed OAuth to create, modify, and format presentations. Use the api-gateway skill for other third-party apps.
- **[pptx-pdf-font-fix](skills/pptx-pdf-font-fix)**
  - **Description**: This plugin fixes font embedding issues in PDF exports from PowerPoint by applying a slight transparency to text, ensuring custom fonts are correctly embedded.
- **[skill-mermaid-diagrams](skills/skill-mermaid-diagrams)**
  - **Description**: Generate consistent, template-based Mermaid diagrams for technical content across 12 types including architecture, flowcharts, and timelines, with automatic template selection, LLM-powered content generation, and error handling.
- **[xfyun-ppt-gen](skills/xfyun-ppt-gen)**
  - **Description**: Create professional, structured PowerPoint presentations from optimized topic keywords.
- **[tiangong-wps-ppt-automation](skills/tiangong-wps-ppt-automation)**
  - **Description**: Automate common PowerPoint/WPS Presentation tasks on Windows, including text/notes/outline management, PDF/image export, text replacement, slide manipulation, and style unification. Suitable for single-presentation actions only.
- **[gws-slides](skills/gws-slides)**
  - **Description**: Create and edit presentations with Google Slides.
- **[md-2-pdf](skills/md-2-pdf)**
  - **Description**: Convert markdown files into clean, formatted PDFs using reportlab.
- **[ima-knowledge-ai](skills/ima-knowledge-ai)**
  - **Description**: This essential AI content creation guide offers expert advice on workflow design, model selection, and parameter optimization, ensuring professional-grade results in image, video, and music generation. It's crucial for maintaining consistency and avoiding common mistakes.
- **[pollinations-sketch-note](skills/pollinations-sketch-note)**
  - **Description**: An AI-powered tool that generates hand-drawn style knowledge cards, automatically searching and summarizing the topic.
### Academic & Writing

- **[reviewer-rebuttal-coach](skills/reviewer-rebuttal-coach)**
  - **Description**: This AI skill plugin reads review comments, mentor annotations, or feedback from the clipboard and generates itemized responses, a revision plan, and priority suggestions.
- **[add-educational-comments](skills/add-educational-comments)**
  - **Description**: Add educational comments to the specified file, or prompt for a file if none is provided.
- **[certificate-generation](skills/certificate-generation)**
  - **Description**: Create professional certificates, diplomas, and awards with each::sense AI. Ideal for course completions, achievements, certifications, and custom branded certificates.
- **[diataxis-writing](skills/diataxis-writing)**
  - **Description**: A guide for the Diataxis documentation framework, offering diagnosis, classification, templates, and quality assessment for four types of documentation: Tutorial, How-to, Reference, and Explanation.
- **[agentledger-research-assistant](skills/agentledger-research-assistant)**
  - **Description**: A structured web research tool for AI agents, enabling multi-source research, synthesis of findings into actionable briefs, and ongoing trend monitoring. Ideal for market research, competitor analysis, and deep-dives into specific topics.
- **[pdf-translate](skills/pdf-translate)**
  - **Description**: This AI skill translates PDF documents into Chinese, preserving professional typography. It extracts and translates text section-by-section into well-structured Markdown, then generates a new PDF with full CJK support.
- **[human-writing-azzar](skills/human-writing-azzar)**
  - **Description**: This skill ensures professional, human-like writing for READMEs, technical documentation, and formal outputs, avoiding AI-specific language, buzzwords, and unnecessary fluff.
- **[aibrary-podcast-summary](skills/aibrary-podcast-summary)**
  - **Description**: Generate a 10-15 minute engaging, single-narrator podcast script that summarizes the key ideas of a book.
- **[aibrary-reading-list](skills/aibrary-reading-list)**
  - **Description**: Generate a curated, themed reading list with books organized in a logical order, ideal for deep exploration or building expertise in a specific area.
- **[sop-writer](skills/sop-writer)**
  - **Description**: SOP Writer is a tool for creating standard operating procedures, including flowcharts, checklists, audits, and training materials. It also provides a template library for easy access.
- **[article-summarizer](skills/article-summarizer)**
  - **Description**: The article summarizer automatically extracts and summarizes web articles, providing structured summaries with key points and bullet lists. Ideal for self-media, operations, and researchers.
- **[translate-cli](skills/translate-cli)**
  - **Description**: A guide for using the `translate` CLI to manage translations across various inputs, configure providers, and customize settings. Use it for command construction, configuration updates, provider setup, and troubleshooting.
- **[banner-youtube-translate-workflow](skills/banner-youtube-translate-workflow)**
  - **Description**: This AI skill plugin automates the process of downloading YouTube audio, playing it in Doubao, and capturing the translation, ideal for full video translations.
- **[alicloud-ai-audio-livetranslate](skills/alicloud-ai-audio-livetranslate)**
  - **Description**: Use this AI skill plugin for live speech translation, ideal for bilingual meetings, real-time interpretation, and converting speech to text or another language.
- **[alicloud-media-video-translation](skills/alicloud-media-video-translation)**
  - **Description**: Manage Alibaba Cloud IMS video translation jobs, including subtitles, voice, and face, through OpenAPI. Use for API-based translation, status updates, and job management.
- **[clarity-literature](skills/clarity-literature)**
  - **Description**: Search and retrieve publication details from Clarity Protocol for research papers, PubMed references, or citations on specific topics like proteins.
- **[translate-image](skills/translate-image)**
  - **Description**: Translate and extract text from images, or remove text using the TranslateImage AI. Ideal for processing images with foreign-language text, including manga.
- **[nexus-translate](skills/nexus-translate)**
  - **Description**: High-quality translations in over 50 languages, with cultural awareness.
- **[wechat-article-crayon](skills/wechat-article-crayon)**
  - **Description**: This AI skill plugin, 'wechat-article-crayon', aids in creating and refining WeChat public account articles, including topic selection, title optimization, content writing, rewriting, formatting, and cover image prompt generation. It is ideal for producing highly readable, engaging, and natural-sounding content.
- **[x-article-reader](skills/x-article-reader)**
  - **Description**: This AI skill reads X (Twitter) articles aloud using macOS text-to-speech. It accepts an article URL, automatically detects the language, and selects the appropriate voice. Use it with commands like 'read aloud' or 'read this X article'.
- **[wechat-article-writer](skills/wechat-article-writer)**
  - **Description**: The WeChat Article Writer is an AI tool designed to assist in creating WeChat public account articles, covering the entire process from topic selection to final draft and automatic image pairing.
- **[wechat-article-extractor-skill](skills/wechat-article-extractor-skill)**
  - **Description**: This skill extracts metadata and content from WeChat Official Account articles, including title, author, content, publish time, and cover image, and converts them into structured data. It supports various article types such as posts, videos, images, voice messages, and reposts.
- **[article-idea-capture](skills/article-idea-capture)**
  - **Description**: Capture and organize article ideas, topics, and half-formed thoughts, developing them into outlines or drafts. Use this when you have an idea, want to save a thought for later, or need to expand on a saved concept.
- **[docs-generator](skills/docs-generator)**
  - **Description**: Automated documentation generator for creating API docs, README, CHANGELOG, contributing guides, architecture documents, tutorials, FAQ, and reference manuals. Supports REST, GraphQL, and OpenAPI formats.
- **[developer-docs-framework](skills/developer-docs-framework)**
  - **Description**: This AI skill plugin, 'developer-docs-framework', offers best practices and frameworks for creating effective technical documentation, covering content types, writing styles, information architecture, and developer experience strategies. It supports various documentations like tutorials, API references, and migration guides, and is triggered by keywords such as 'write docs' or 'API docs'.
- **[arxiv-reader](skills/arxiv-reader)**
  - **Description**: This AI skill plugin uses Python to classify and deeply analyze an arXiv paper by its ID or URL, then prints the reading notes.
- **[meyhem-researcher](skills/meyhem-researcher)**
  - **Description**: A multi-query research tool that breaks down a topic into focused queries and previews the top results, without requiring an API key.
- **[rubric-gap-analyzer](skills/rubric-gap-analyzer)**
  - **Description**: Analyzes the current draft against grading criteria or assignment requirements, identifying gaps and providing a plan to improve the score.
- **[tavily-research-pro](skills/tavily-research-pro)**
  - **Description**: A professional AI-powered search and research tool that aggregates multidimensional data, performs semantic analysis, and generates automated reports for structured information gathering.
- **[pdf-tools](skills/pdf-tools)**
  - **Description**: Manage PDF files by viewing, extracting, editing text, merging, splitting, rotating pages, and accessing metadata.
- **[ai-researcher](skills/ai-researcher)**
  - **Description**: Conduct in-depth research on any topic, providing structured analysis, source evaluation, and expert-level summaries.
- **[paper-assistant](skills/paper-assistant)**
  - **Description**: A comprehensive assistant for all stages of academic paper writing, from topic selection and outlining to final editing and submission preparation.
- **[research-logger-pro](skills/research-logger-pro)**
  - **Description**: This AI skill plugin auto-saves deep search results to SQLite and Langfuse, logging every query with topic tags, timestamps, and full results for easy retrieval and review.
- **[latex-writer](skills/latex-writer)**
  - **Description**: Generate professional LaTeX documents from templates, including academic papers, Chinese theses, CVs, and custom formats, with auto-compilation to PDF.
- **[agentarxiv](skills/agentarxiv)**
  - **Description**: Facilitate outcome-driven scientific publishing for AI agents, enabling the sharing of research, experiments, and peer reviews with features like milestone tracking and replication bounties.
- **[moltarxiv](skills/moltarxiv)**
  - **Description**: Outcome-driven scientific publishing for AI, enabling the sharing of research, experiments, and peer reviews with validated artifacts and collaboration opportunities.
- **[meta-research](skills/meta-research)**
  - **Description**: An autonomous AI assistant for the full research lifecycle, from brainstorming and literature review to experiment design, analysis, and writing up findings, with a focus on reproducibility and dynamic phase transitions.
- **[scholar-paper-downloader](skills/scholar-paper-downloader)**
  - **Description**: A bulk PDF downloader for academic papers, supporting search and download from multiple scholarly websites like arXiv, PubMed, and PMC. It automatically extracts metadata and generates an index list, prioritizing free official sources and providing manual download guidance for paid content.
- **[academic-research-hub](skills/academic-research-hub)**
  - **Description**: Use this skill to search, download, and cite academic papers, and gather scholarly information. It's ideal for literature reviews, bibliography generation, and accessing databases like arXiv, PubMed, Semantic Scholar, or Google Scholar.
- **[citation-finder](skills/citation-finder)**
  - **Description**: This AI skill plugin, citation-finder, searches for academic papers by title across multiple databases and returns formatted citations in GB/T 7714, APA 7th, and MLA 9th styles, along with source links.
- **[web-researcher](skills/web-researcher)**
  - **Description**: Use this skill for in-depth research, fact-checking, or staying updated with the latest technical news.
- **[gemini-deep-research](skills/gemini-deep-research)**
  - **Description**: Use Gemini Deep Research Agent for in-depth, long-running research tasks, including multi-source synthesis, competitive analysis, market research, and comprehensive technical investigations.
- **[mckinsey-decision-memo-writer](skills/mckinsey-decision-memo-writer)**
  - **Description**: Condense long documents, reports, proposals, and email threads into concise memos, highlighting key points, risks, open questions, and next steps.
- **[scihub-paper-downloader](skills/scihub-paper-downloader)**
  - **Description**: Fetch a PDF link from Sci-Hub using a DOI.
- **[auto-researcher](skills/auto-researcher)**
  - **Description**: The Auto-Researcher is a tool for in-depth research, cross-verification, and generating citation reports.
- **[paper-fetcher](skills/paper-fetcher)**
  - **Description**: Fetch academic papers from Sci-Hub using a DOI, automatically downloading and saving the PDFs to research/papers/ with clean filenames. Ideal for requests involving DOIs or PubMed papers.
- **[core-researcher](skills/core-researcher)**
  - **Description**: You are an academic research assistant with interdisciplinary expertise for literature reviews, paper analysis, and scholarly writing, using only the Core API.
- **[parallel-ai-research](skills/parallel-ai-research)**
  - **Description**: Conduct open-ended research on a topic, creating a dynamic markdown document with support for interactive and in-depth exploration.
- **[research-agent](skills/research-agent)**
  - **Description**: Conduct in-depth research on any topic, creating a dynamic markdown document. Supports interactive and deep research modes.
- **[proofreader](skills/proofreader)**
  - **Description**: This AI skill plugin offers proofreading, including typo detection, grammar correction, style consistency, readability scoring, and comprehensive reports. Use it when you need a proofreader.
- **[thesis-helper](skills/thesis-helper)**
  - **Description**: A thesis helper for generating outlines, literature reviews, abstracts, and managing citation formatting, style checks, and defense preparation, adjusting automatically to the academic level.
- **[paper-parse-figures](skills/paper-parse-figures)**
  - **Description**: This AI skill plugin converts academic PDF papers into markdown and extracts the figures.
- **[chonkie-deepresearch](skills/chonkie-deepresearch)**
  - **Description**: Use Chonkie DeepResearch to conduct in-depth queries, generating detailed research reports with citations for tasks like market analysis, competitive intelligence, and technical deep dives.
- **[arxiv-watch](skills/arxiv-watch)**
  - **Description**: Monitor new papers on arXiv by category. Ideal for checking the latest research, tracking specific topics, or managing reading lists.
- **[research-to-wechat](skills/research-to-wechat)**
  - **Description**: This AI skill plugin transforms a topic, notes, article, URL, or transcript into a well-structured, polished Markdown article with inline visuals and a cover image, ready for WeChat and other platforms. It includes an evidence ledger, HTML conversion, and multi-platform distribution options.
- **[knowledge-answer](skills/knowledge-answer)**
  - **Description**: This AI skill, 'knowledge-answer', provides answers in the user's preferred language, including citations as clickable footnotes when based on search results. The date and citation format are standardized.
- **[knowledge-forge](skills/knowledge-forge)**
  - **Description**: Transform personal experiences, case studies, and business documents into structured, teachable content that is easy to understand, remember, and apply. Ideal for creating course outlines, presentations, or shareable knowledge documents.
- **[pro-zh-summary](skills/pro-zh-summary)**
  - **Description**: A professional tool for summarizing long Chinese texts, automatically segmenting and condensing content when users request a summary or key points.
### Notes & Knowledge Base

- **[flashcard](skills/flashcard)**
  - **Description**: A flashcard creator with spaced repetition, quiz mode, and export options (Markdown/Anki), featuring learning statistics. Use for efficient study and review.
- **[keep-learning-agent](skills/keep-learning-agent)**
  - **Description**: The Keep-Learning Agent is a framework for knowledge accumulation and experience solidification, featuring learning records, quick indexing, self-repair, and experience-to-model conversion. It includes complete templates, an indexing system, and SOP processes to ensure continuous AI evolution.
- **[learning-system-skill](skills/learning-system-skill)**
  - **Description**: The 'learning-system-skill' plugin manages a knowledge graph, deep learning notes, practical reviews, and associated networks. It is activated for tasks like planning studies, updating the knowledge graph, researching AI topics, summarizing experiences, or reviewing weekly learnings. Use it after coding, reading papers, or conducting research to distill and organize knowledge.
- **[notebooklm-skill](skills/notebooklm-skill)**
  - **Description**: This skill lets you query your Google NotebookLM notebooks from Claude Code, providing source-backed answers with browser automation, library management, and persistent authentication. It reduces hallucinations by responding only with document content.
- **[session-memory-workspace](skills/session-memory-workspace)**
  - **Description**: This AI skill plugin summarizes sessions and saves them to daily memory files, allowing OpenClaw to recall and reference past conversations.
- **[tiangong-notebooklm-cli](skills/tiangong-notebooklm-cli)**
  - **Description**: A CLI tool for NotebookLM, facilitating authentication, notebook management, chat, source handling, note-taking, sharing, research, and artifact generation/download.
- **[wechat-article-reader](skills/wechat-article-reader)**
  - **Description**: This AI skill plugin exports articles from WeChat public accounts into Markdown format, triggered when a user provides a WeChat article link or requests to download, export, or save the article. It saves the file by default to the source directory in the workspace.
- **[feishu-article-collector](skills/feishu-article-collector)**
  - **Description**: Automatically collects articles from Jinri Toutiao and WeChat public accounts, extracts the main text, generates summaries and categorizations with AI, and saves them in a Feishu multi-dimensional table. Supports deduplication.
- **[article-extract](skills/article-extract)**
  - **Description**: Extracts the main text content from WeChat public accounts, blogs, and news websites, bypassing anti-crawling mechanisms, and outputs it as plain text.
- **[wechat-article-explainer](skills/wechat-article-explainer)**
  - **Description**: This AI skill summarizes and explains the content of WeChat public account articles in simple language, based on the provided link or URL.
- **[wechat-article-extractor](skills/wechat-article-extractor)**
  - **Description**: Extracts the full text and images from a WeChat public account article URL and saves it as a clean Markdown file, automatically handling bot-detection by finding mirror sites.
- **[librag-knowledge-recall](skills/librag-knowledge-recall)**
  - **Description**: The LibRAG plugin uses the local `/api/v1/librag/knowbase/recall` interface to retrieve data from a knowledge base, suitable for tasks like knowledge retrieval, document recall, and evidence extraction in Chinese contexts.
- **[feishu-document-reader](skills/feishu-document-reader)**
  - **Description**: Extract content from all Feishu (Lark) document types using the official Feishu Open API.
- **[obsidian-openclaw-sync](skills/obsidian-openclaw-sync)**
  - **Description**: Sync Obsidian OpenClaw config across multiple iCloud devices, managing symlinks for seamless integration.
- **[notion-2026-01-15](skills/notion-2026-01-15)**
  - **Description**: Updated Notion API as of January 15, 2026, with new features for creating, moving, and managing pages, data sources, and blocks.
- **[agxntsix-research-logger](skills/agxntsix-research-logger)**
  - **Description**: An AI research pipeline that automatically logs data to SQLite and traces with Langfuse.
- **[research-logger](skills/research-logger)**
  - **Description**: Effortlessly manage your research with automatic logging, saving results to SQLite with metadata, and full Langfuse tracing. Ideal for research, competitive analysis, and knowledge base building.
- **[multimedia-to-obsidian](skills/multimedia-to-obsidian)**
  - **Description**: Import various multimedia documents into your Obsidian knowledge base, supporting formats like PPT, PDF, DOCX, and images. It automatically extracts each page or image, uses multimodal models to understand the content, and saves it as text descriptions in Obsidian, ideal for organizing training materials, migrating notes, and converting image data into structured knowledge.
- **[obsidian-canvas-creator](skills/obsidian-canvas-creator)**
  - **Description**: Create interactive Obsidian Canvas files from text for mind maps or freeform layouts, ideal for visualizing and organizing information spatially.
- **[ai-research-to-obsidian](skills/ai-research-to-obsidian)**
  - **Description**: This AI skill plugin searches for information using AI tools and saves the results as Obsidian documents. It can be triggered when the user asks to search a question, requests a browser search with Obsidian save, or says 'help me check' and mentions saving to notes or documents.
- **[pdf-parser-mineru](skills/pdf-parser-mineru)**
  - **Description**: A PDF parsing tool that converts documents into machine-readable formats like Markdown and JSON.
- **[pdf-co](skills/pdf-co)**
  - **Description**: PDF.co API integration with managed OAuth for PDF conversion, merging, splitting, editing, and data extraction. Use this skill for tasks like converting PDFs to other formats, adding watermarks or text, and parsing invoices.
- **[pdfagent](skills/pdfagent)**
  - **Description**: A self-hosted solution for PDF operations and conversions, with metered usage tracking.
- **[zotero-pdf-upload](skills/zotero-pdf-upload)**
  - **Description**: Upload and manage PDFs in your Zotero Web Library, supporting both personal and group libraries. Ideal for adding papers, organizing collections, and managing your library through the API.
- **[links-to-pdfs](skills/links-to-pdfs)**
  - **Description**: Download and convert web documents from sources like Notion, DocSend, and PDFs into local PDF files. Supports authentication for protected documents and session persistence.
- **[pdf-to-markdown](skills/pdf-to-markdown)**
  - **Description**: Converts PDF documents to Markdown format. Use this when you need to transform PDFs into a more editable form.
- **[compress-pdf](skills/compress-pdf)**
  - **Description**: Compress a user-provided PDF by uploading it to Cross-Service-Solutions, then return a download URL for the compressed file once processing is complete.
- **[convert-to-pdf](skills/convert-to-pdf)**
  - **Description**: Upload one or multiple documents to Cross-Service-Solutions, convert them to PDF, and receive download URLs for the converted files (or a ZIP if multiple).
- **[merge-pdf](skills/merge-pdf)**
  - **Description**: Upload multiple PDF files to Cross-Service-Solutions, merge them, and receive a download URL for the combined PDF once processing is complete.
- **[personal-notes](skills/personal-notes)**
  - **Description**: Serves as a note-taking and journaling assistant, capturing thoughts, reflections, and daily logs. Use it for personal notes or when mentioning terms like diary, log, or 'write down'.
- **[book-brain-visual-reader](skills/book-brain-visual-reader)**
  - **Description**: Enhanced BOOK BRAIN for LYGO Havens with visual capabilities, integrating a 3-brain filesystem and memory system that checks visuals (browser, images, screenshots) alongside text and API data for deeper verification and retrieval. Ideal for agents using visual tools or browser automation.
- **[obsidian-cli-skills](skills/obsidian-cli-skills)**
  - **Description**: Obsidian CLI is a command-line tool for managing Obsidian vaults, enabling you to search, create, move, and delete notes.
- **[obsidian-clip](skills/obsidian-clip)**
  - **Description**: Create and manage Obsidian Clip notes, which are web or article snippets. Use this skill when you want a readable summary of a URL and to save it in your Obsidian vault under the Clip/YYYY-MM/ directory.
- **[obsidian-cli](skills/obsidian-cli)**
  - **Description**: This skill for the official Obsidian CLI (v1.12+) automates vault management, including file operations, daily notes, search, tasks, and more, as well as developer tools.
- **[note](skills/note)**
  - **Description**: A system for capturing, organizing, and retrieving notes, ideas, and insights. It automatically organizes content by topic and project, and surfaces relevant information when needed, connecting related concepts across different areas.
- **[obsidian-cli-official](skills/obsidian-cli-official)**
  - **Description**: Official Obsidian CLI (v1.12+), providing a full command-line interface for managing notes, tasks, search, tags, properties, links, and more.
- **[obsidians](skills/obsidians)**
  - **Description**: This AI skill plugin enables automation of Obsidian vaults using plain Markdown notes and obsidian-cli, and supports over 50 models for various tasks like image and video generation, text-to-speech, and more.
- **[notebooklm-distiller](skills/notebooklm-distiller)**
  - **Description**: NotebookLM Distiller extracts knowledge from Google NotebookLM into Obsidian, offering Q&A generation, structured summaries, glossary extraction, web research, and markdown persistence.
- **[obsidian-organizer](skills/obsidian-organizer)**
  - **Description**: Organize and standardize Obsidian vaults for better reliability and long-term maintainability, including folder structure design, file naming conventions, migration, and the creation of audit-and-fix workflows.
- **[neural-note-taker](skills/neural-note-taker)**
  - **Description**: An advanced associative memory tool that helps build connections between facts and entities, preserving context during long information processing sessions.
- **[obsidian-daily](skills/obsidian-daily)**
  - **Description**: Manage Obsidian Daily Notes with obsidian-cli, including creating, opening, appending entries, and searching vault content. Supports relative dates like 'yesterday' or '3 days ago'. Requires obsidian-cli installed via Homebrew (Mac/Linux) or Scoop (Windows).
- **[second-brain](skills/second-brain)**
  - **Description**: A personal knowledge base powered by Ensue for saving, recalling, and building upon your learnings. Use it to manage your notes and toolbox.
- **[save-to-obsidian](skills/save-to-obsidian)**
  - **Description**: Saves markdown content to a remote Obsidian vault via SSH.
- **[notesctl-skill-for-openclaw](skills/notesctl-skill-for-openclaw)**
  - **Description**: Manage Apple Notes with local scripts for creating, appending, listing, searching, exporting, and editing notes. Use this skill when you need to add, list, search, or manage note folders via OpenClaw.
- **[2nd-brain](skills/2nd-brain)**
  - **Description**: A personal knowledge base for storing and retrieving information on people, places, media, ideas, and more. Use it when mentioning specific entities or using trigger phrases like 'remember' or 'note that'.
- **[brainrepo](skills/brainrepo)**
  - **Description**: A personal knowledge repository that captures, organizes, and retrieves information using PARA and Zettelkasten. It triggers with commands like 'save this' or 'remember', supports daily/weekly reviews, and integrates with any AI agent that reads markdown, storing everything as .md files in a Git repo for use in Obsidian, VS Code, or any editor.
- **[notion-cli-agent](skills/notion-cli-agent)**
  - **Description**: Search for pages using the specified query.
- **[microsoft-onenote](skills/microsoft-onenote)**
  - **Description**: Integrate with Microsoft OneNote to manage your notebooks and interact with your data.
- **[notion-integration](skills/notion-integration)**
  - **Description**: Integrate with Notion to manage projects, documents, and workflows. Use this skill to interact with your Notion data.
- **[voicenotes-official](skills/voicenotes-official)**
  - **Description**: This official Voicenotes skill enables OpenClaw to use new APIs for semantic search, transcript retrieval, filtering by tags or dates, and creating text notes through natural conversation.
- **[timeless](skills/timeless)**
  - **Description**: Manage and query Timeless meetings, rooms, transcripts, and AI documents. You can also capture podcast episodes and YouTube videos for transcription, and interact with the Timeless AI to discuss meeting content.
### Productivity & Study Tools

- **[hinihao-chinese-tutor](skills/hinihao-chinese-tutor)**
  - **Description**: A proactive Chinese language tutor that provides curated, real-world Mandarin learning content on a schedule, suitable for HSK 1-6 learners. It offers recommendations for reading materials, podcasts, videos, and songs, and can be activated by specific user requests or scheduled lessons.
- **[flashcards-podcasts-master](skills/flashcards-podcasts-master)**
  - **Description**: Manages flashcards, generates AI content, and facilitates audio study sessions through the EchoDecks External API.
- **[recipe-create-classroom-course](skills/recipe-create-classroom-course)**
  - **Description**: Create a Google Classroom course and invite students to join.
- **[training-plan](skills/training-plan)**
  - **Description**: A training plan designer that helps with curriculum, evaluation, materials, scheduling, and certificates. Ideal for creating comprehensive training programs and employee development plans.
- **[optical-quantum-skill](skills/optical-quantum-skill)**
  - **Description**: Simulates a quantum kernel using optical fiber and linear optics.
- **[space-autonomy-skill](skills/space-autonomy-skill)**
  - **Description**: An autonomous space navigation agent that uses optical quantum kernels for terrain classification.
- **[quantum-lab](skills/quantum-lab)**
  - **Description**: Execute Python scripts and demos in the /home/bram/work/quantum_lab directory using the existing venv at ~/.venvs/qiskit. Use this when requested to run specific subcommands or notebooks from the repo.
- **[quantumlab](skills/quantumlab)**
  - **Description**: Execute Python scripts and demos in /home/bram/work/quantum_lab using the existing venv ~/.venvs/qiskit. This includes running subcommands for quant_math_lab.py, qcqi_pure_math_playground.py, quantum_app.py, quantumapp.server, or any notebooks in the repository.
- **[expanso-language-detect](skills/expanso-language-detect)**
  - **Description**: Identify the language of given text using AI.
- **[natural-language-planner](skills/natural-language-planner)**
  - **Description**: This AI skill plugin manages tasks and projects through natural language, organizing tasks into projects, tracking progress, and providing a local Kanban dashboard.
- **[git-standup](skills/git-standup)**
  - **Description**: Automatically generates daily work reports by analyzing Git commits.
- **[plan-flow](skills/plan-flow)**
  - **Description**: AI-assisted development workflows for discovery, planning, execution, code reviews, and testing.
- **[error-analysis](skills/error-analysis)**
  - **Description**: This AI skill plugin provides error analysis for studying, including categorizing mistakes, identifying knowledge gaps, and offering review suggestions.
- **[notion-1-0-0](skills/notion-1-0-0)**
  - **Description**: This AI skill plugin uses the Notion API to create and manage pages, databases, and blocks.
- **[notion-template](skills/notion-template)**
  - **Description**: A Notion template generator for creating workspaces, databases, dashboards, wikis, projects, and personal templates. Use it when you need to design Notion templates.
- **[vibe-notion](skills/vibe-notion)**
  - **Description**: Interact with Notion using the unofficial private API to manage pages, databases, blocks, search, users, and comments.
- **[vibe-notionbot](skills/vibe-notionbot)**
  - **Description**: Interact with Notion workspaces to manage pages, databases, blocks, users, and comments using the official API.
- **[notion-skill](skills/notion-skill)**
  - **Description**: Interact with Notion pages and databases using the official Notion API.
- **[notion-clipper-skill](skills/notion-clipper-skill)**
  - **Description**: Clip web pages to Notion by fetching URLs, converting HTML to Markdown and then to Notion blocks, and saving to a user-specified Notion database or page. Use this skill when you want to save or clip a webpage to Notion.
- **[wechat-to-notion](skills/wechat-to-notion)**
  - **Description**: Save WeChat public account articles to a Notion database. When a user shares a mp.weixin.qq.com link, this skill extracts the title, cover image, and body content, then saves it as Notion blocks.
- **[visual-file-sorter](skills/visual-file-sorter)**
  - **Description**: Automatically traverses the download folder or desktop, uses a visual model to 'see' and rename file contents, and archives them into specified categories.
- **[ux-researcher-designer](skills/ux-researcher-designer)**
  - **Description**: A toolkit for senior UX designers and researchers, offering data-driven persona creation, journey mapping, usability testing frameworks, and research synthesis for user research and design validation.
- **[deepread-form-fill](skills/deepread-form-fill)**
  - **Description**: AI-powered PDF form filling. Upload any PDF and your data as JSON; the AI visually detects fields, semantically maps your data, fills the form with quality checks, and returns a completed PDF.
- **[youtube-summarizer](skills/youtube-summarizer)**
  - **Description**: Automatically fetches YouTube video transcripts, generates structured summaries, and sends full transcripts to messaging platforms, providing key insights and metadata.
- **[cognitive-brain](skills/cognitive-brain)**
  - **Description**: A cross-session memory and cognition system that enhances AI's ability to remember and understand across multiple interactions.
- **[super-brain](skills/super-brain)**
  - **Description**: The Super-Brain AI enhancement system enables the AI to remember users across sessions, continuously evolve, and provide personalized services by learning user preferences and service skills.
- **[audio-summary](skills/audio-summary)**
  - **Description**: The 'audio-summary' skill plugin extracts 16k mono compressed audio from video files using `ffmpeg`, transcribes and summarizes the audio content with the `qwen3-asr-flash` model, and supports large files through 48k compression.
- **[notebooklm-bypass](skills/notebooklm-bypass)**
  - **Description**: This AI skill plugin offers programmatic control of NotebookLM with automatic recovery from authentication errors.
- **[expanso-text-summarize](skills/expanso-text-summarize)**
  - **Description**: Summarize text into 3-5 key points using AI.
- **[deepreader-skill](skills/deepreader-skill)**
  - **Description**: The default web content reader for OpenClaw, converting Twitter, Reddit, YouTube, and any webpage into clean Markdown without requiring API keys. Ideal for ingesting social media posts, articles, or video transcripts into agent memory.
- **[read-optimizer](skills/read-optimizer)**
  - **Description**: Optimizes file reading by employing smart strategies (like head, tail, grep, diff) to minimize token usage and latency.
- **[obsidian-plugin-tasknotes](skills/obsidian-plugin-tasknotes)**
  - **Description**: Manage tasks in Obsidian using the TaskNotes plugin, including creating, listing, querying, updating, and deleting tasks.
- **[rss-ai-reader](skills/rss-ai-reader)**
  - **Description**: The RSS AI Reader automatically fetches subscriptions, generates summaries using LLMs, and pushes to Feishu, Telegram, or Email. It supports scheduled fetching and can be triggered by commands like 'subscribe for me' or 'monitor this site'.
- **[obsidian-task](skills/obsidian-task)**
  - **Description**: Manage Obsidian tasks through the terminal with obsidian-cli. Perform actions like listing, toggling, creating, and updating tasks.
- **[reddit-readonly](skills/reddit-readonly)**
  - **Description**: Browse and search Reddit in read-only mode, allowing you to explore subreddits, find posts by topic, and examine comment threads.
- **[doc-summarizer](skills/doc-summarizer)**
  - **Description**: A versatile AI tool for generating summaries, including document and text summarization, meeting notes, email digests, and creating mind maps.
- **[notion-mcp](skills/notion-mcp)**
  - **Description**: The Notion MCP plugin integrates with managed authentication to query databases, create and update pages, and manage blocks within Notion workspaces.
- **[yt-summary](skills/yt-summary)**
  - **Description**: Summarize any YouTube video by sharing its link and optionally add custom instructions for focus, like 'focus on the technical details'.
- **[shelly-meeting-summarizer](skills/shelly-meeting-summarizer)**
  - **Description**: Convert raw meeting transcripts into clear, structured, and actionable summaries.
- **[tube-summary](skills/tube-summary)**
  - **Description**: Search YouTube for videos on any topic and get intelligent summaries from their subtitles, allowing you to quickly understand the content without watching.
- **[rss-reader](skills/rss-reader)**
  - **Description**: Monitor RSS and Atom feeds for content research, tracking industry news, or building a personal news aggregator. Supports multiple feeds with categories, filters, and summaries.
- **[youmind-youtube-transcript](skills/youmind-youtube-transcript)**
  - **Description**: Extract and save YouTube video transcripts and subtitles using the YouMind API, supporting batch processing of up to 5 videos. Transcripts are saved with timestamps in markdown format on your YouMind board, accessible from any IP.
- **[slack-reader](skills/slack-reader)**
  - **Description**: Summarize Slack channel history and thread conversations. Use for Slack links, to view or summarize discussions, or check recent messages.
- **[plsreadme](skills/plsreadme)**
  - **Description**: Share markdown files and text as clean, readable web links via plsreadme.com. Ideal for sharing documents, READMEs, PRDs, proposals, or notes. Requires the plsreadme MCP server (npx plsreadme-mcp).
- **[youtube-voice-summarizer-elevenlabs](skills/youtube-voice-summarizer-elevenlabs)**
  - **Description**: Convert YouTube videos into podcast-style voice summaries using ElevenLabs TTS.
- **[tweet-summarizer-lite](skills/tweet-summarizer-lite)**
  - **Description**: Fetch and summarize single tweets from Twitter. Ideal for quick, lightweight tweet lookups.
- **[focus-coach](skills/focus-coach)**
  - **Description**: The Focus Coach plugin helps AI agents diagnose focus issues using the BJ Fogg B=MAP model and suggests a small, actionable step. It's ideal for improving concentration, overcoming procrastination, and enhancing productivity through tiny habits.
- **[google-workspace-automation](skills/google-workspace-automation)**
  - **Description**: Automate Gmail, Drive, Sheets, and Calendar tasks with scope-aware plans for daily use, ensuring explicit OAuth scopes and audit-ready outputs.
- **[task-decomposer](skills/task-decomposer)**
  - **Description**: This skill breaks down complex requests into simpler subtasks, identifies necessary capabilities, and either finds existing solutions or creates new ones as needed.
- **[time-checker](skills/time-checker)**
  - **Description**: Get accurate current time, date, and timezone information for any location worldwide using time.is. Ideal for queries like 'what time is it in X' or verifying timezone offsets.
- **[afrexai-email-to-calendar](skills/afrexai-email-to-calendar)**
  - **Description**: This AI skill extracts calendar events, deadlines, action items, and follow-ups from emails, compatible with any calendar provider. It uses pure agent intelligence without external dependencies.
- **[afrexai-sprint-planner](skills/afrexai-sprint-planner)**
  - **Description**: Efficiently plan, scope, and execute agile sprints that deliver results without unnecessary formalities.
- **[todolist](skills/todolist)**
  - **Description**: This skill module offers enhanced features to boost development and research efficiency.
- **[aibrary-growth-plan](skills/aibrary-growth-plan)**
  - **Description**: Create a structured personal growth plan with book recommendations, milestones, and actionable weekly tasks for learning, skill development, or professional advancement.
- **[student-timetable](skills/student-timetable)**
  - **Description**: A student timetable manager for self or parent-managed child profiles, including an initialization flow and profile registry under schedules/profiles.
