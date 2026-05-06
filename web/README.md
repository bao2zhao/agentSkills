# 研发场景web十大热门 Skill 推荐

本文面向实际研发场景，整理并推荐了一组可直接应用于日常开发流程的 Agent Skill。这些 Skill 覆盖前端设计、前后端开发、代码审查、自动化测试、CI/CD、问题修复以及文档维护等常见环节。

---

## 目录

1. [前端设计 (frontend-design)](#前端设计-frontend-design)
2. [前端开发 (cache-components)](#前端开发-cache-components)
3. [全栈开发 (fullstack-developer)](#全栈开发-fullstack-developer)
4. [代码审查（前端）(frontend-code-review)](#代码审查前端-frontend-code-review)
5. [代码审查（通用）(code-reviewer)](#代码审查通用-code-reviewer)
6. [网页应用测试 (webapp-testing)](#网页应用测试-webapp-testing)
7. [CI/CD：PR 创建 (pr-creator)](#cicdpr-创建-pr-creator)
8. [Linting 和格式错误修复 (fix)](#linting-和格式错误修复-fix)
9. [技术文档更新 (update-docs)](#技术文档更新-update-docs)
10. [查找 Skill (find-skills)](#查找-skill-find-skills)

---

## 前端设计 (frontend-design)

| 属性 | 内容 |
|------|------|
| **作者** | Anthropic |
| **地址** | https://github.com/anthropics/skills/tree/main/skills/frontend-design |

### 简介

该 Skill 旨在创建具有独特性和高品质的前端界面，能够达到生产级别的标准。它的核心目标是避免生成千篇一律、缺乏独特风格的 "AI 风格" 界面，而是通过在设计上有意地选择大胆、明确的美学方向（例如：极简、复古、未来感、野兽派等），并注重排版、色彩、动效、空间布局等细节，来打造出令人印象深刻、具有艺术感的前端页面。

### 资源文件

- SKILL.md

### 应用场景

- **构建网页组件或页面**：从零开始创建 React 组件、HTML/CSS 布局或独立静态页面。
- **开发完整的 Web 应用或网站**：构建 Landing Page、数据仪表盘或小型网站，确立统一设计风格。
- **美化或重塑现有界面**：提升现有网页的视觉品质，引入独特字体、创意色彩方案和精致动效。

---

## 前端开发 (cache-components)

| 属性 | 内容 |
|------|------|
| **作者** | vercel |
| **地址** | https://github.com/vercel/next.js/tree/canary/.claude-plugin/plugins/cache-components/skills/cache-components |

### 简介

该 Skill 旨在将 Next.js 的 Partial Prerendering (PPR) 和缓存组件（Cache Components）的最佳实践，通过 AI 助手无缝集成到开发工作流中。当项目环境启用 `cacheComponents: true` 配置时，该 Skill 将被激活，为你提供自动化的代码生成与优化能力。

### 资源文件

- SKILL.md
- PATTERNS.md：详细说明文档，包含代码示例和场景解释
- REFERENCE.md：官方 API 参考手册
- TROUBLESHOOTING.md：故障排查指南

### 应用场景

- **自动生成缓存优化的数据组件**：使用 `use cache` 语法缓存可共享数据，为用户专属内容添加 `<Suspense>` 边界。
- **自动实现数据变更后的缓存失效**：生成 Server Action 时自动注入缓存失效逻辑。
- **智能化页面构建与代码现代化**：遵循 PPR 架构规范，提供现代化改造建议。

---

## 全栈开发 (fullstack-developer)

| 属性 | 内容 |
|------|------|
| **作者** | Shubhamsaboo |
| **地址** | https://github.com/Shubhamsaboo/awesome-llm-apps/tree/main/awesome_agent_skills/fullstack-developer |

### 简介

该 Skill 的主要作用是扮演一个精通现代 Web 开发技术的全栈专家角色。它专注于使用 JavaScript/TypeScript 技术栈，特别是 React (Next.js)、Node.js 和主流数据库，来帮助你完成各类 Web 开发任务。

### 资源文件

- SKILL.md

### 应用场景

- 构建完整的 Web 应用：从前端到后端，提供完整的解决方案
- 开发 API：创建 RESTful 或 GraphQL 风格的后端接口
- 创建前端界面：使用 React 或 Next.js 构建现代化的用户界面
- 数据库和数据建模：设计和设置 PostgreSQL 或 MongoDB 等数据库
- 实现用户认证与授权：集成 JWT、OAuth 等认证机制
- 部署与扩展应用：提供在 Vercel、Netlify 等平台上的部署指导
- 集成第三方服务：在应用中接入外部服务

---

## 代码审查（前端）(frontend-code-review)

| 属性 | 内容 |
|------|------|
| **作者** | langgenius |
| **地址** | https://github.com/langgenius/dify/tree/main/.agents/skills/frontend-code-review |

### 简介

该 Skill 的核心功能是自动化审查前端代码（尤其针对 .tsx、.ts、.js 等文件）。它会依据预定义的规则清单，从代码质量、性能表现、业务逻辑等维度对代码开展全面分析。审查完成后，系统将生成结构清晰的报告。

### 资源文件

- SKILL.md
- references/business-logic.md：定义业务场景相关规则
- references/code-quality.md：通用编码规范
- references/performance.md：前端性能最佳实践

### 应用场景

- **审查待提交的变更**：在 git commit 前审查已修改或暂存的文件
- **审查指定的文件**：对特定文件或模块进行针对性深度分析
- **获取结构化的修复报告**：按紧急程度排序问题，标注文件路径、行号及修复方案

---

## 代码审查（通用）(code-reviewer)

| 属性 | 内容 |
|------|------|
| **作者** | google-gemini |
| **地址** | https://github.com/google-gemini/gemini-cli/tree/main/.gemini/skills/code-reviewer |

### 简介

该 Skill 旨在引导 AI 开展专业且全面的代码审查工作。它既支持审查本地代码改动（包括已暂存和未暂存的变更），也可审查远程代码合并请求（Pull Request）。

### 资源文件

- SKILL.md

### 应用场景

- **审查远程 PR**：提供 PR 编号或 URL，AI 自动检出代码并运行检查脚本
- **审查本地代码变更**：通过 git status、git diff 检查工作区改动
- **提供深度分析与结构化反馈**：从正确性、可维护性、可读性、安全性等维度分析

---

## 网页应用测试 (webapp-testing)

| 属性 | 内容 |
|------|------|
| **作者** | Anthropic |
| **地址** | https://github.com/anthropics/skills/tree/main/skills/webapp-testing |

### 简介

该 Skill 是一个基于 Playwright 构建的本地 Web 应用测试工具集，支持前端功能验证、UI 行为调试、页面截图及浏览器控制台日志采集。

### 资源文件

- SKILL.md
- examples/console_logging.py：捕获网页控制台日志
- examples/element_discovery.py：自动发现页面可交互元素
- examples/static_html_automation.py：静态 HTML 文件自动化测试
- scripts/with_server.py：多服务场景下的服务器生命周期管理

### 应用场景

- **自动验证前端功能**：使用自然语言描述测试需求，AI 自动编写 Playwright 脚本
- **调试与分析 UI 行为**：截取截图或获取 HTML 内容，快速定位问题
- **处理需要后台服务的复杂交互**：同时启动前后端服务进行测试
- **测试静态 HTML 文件**：通过 file:// 协议验证纯静态页面

---

## CI/CD：PR 创建 (pr-creator)

| 属性 | 内容 |
|------|------|
| **作者** | google-gemini |
| **地址** | https://github.com/google-gemini/gemini-cli/tree/main/.gemini/skills/pr-creator |

### 简介

该 Skill 的核心作用是引导并自动化创建高质量、符合规范的拉取请求（Pull Request）。它通过标准化工作流程，确保每一次代码提交均遵循项目预设的模板与质量检查标准。

### 资源文件

- SKILL.md

### 应用场景

- **一键创建符合规范的 PR**：自动执行分支检查、应用 PR 模板、运行预检脚本
- **引导贡献者完成首次代码提交**：智能向导形式，降低代码贡献门槛
- **自动执行创建 PR 前的质量检查**：运行 preflight 脚本，中止失败检查

---

## Linting 和格式错误修复 (fix)

| 属性 | 内容 |
|------|------|
| **作者** | facebook |
| **地址** | https://github.com/facebook/react/tree/main/.claude/skills/fix |

### 简介

这个 skill 的核心作用是自动化地修复代码格式并检查代码规范（linting）错误。它通过执行 `yarn prettier` 和 `yarn linc` 两个关键命令来保证代码质量。

### 资源文件

- SKILL.md

### 应用场景

- **提交代码前的预防性检查**：自动清理代码格式，提示 linting 错误
- **修复已发现的 linting 或格式问题**：快速解决工作区内的代码质量问题
- **解决持续集成（CI）失败问题**：自动修复格式问题，列出需要手动更正的 linting 错误

---

## 技术文档更新 (update-docs)

| 属性 | 内容 |
|------|------|
| **作者** | vercel |
| **地址** | https://github.com/vercel/next.js/tree/canary/.agents/skills/update-docs |

### 简介

该 Skill 是一套用于更新 Next.js 项目文档的引导式工作流，核心作用是帮助你根据源代码的变更，来分析、更新和创建相关的文档，确保代码和文档保持同步。

### 资源文件

- SKILL.md
- references/CODE-TO-DOCS-MAPPING.md：源代码和文档映射关系
- references/DOC-CONVENTIONS.md：文档格式、结构和写作风格指南

### 应用场景

- **分析代码变更对文档的影响**：通过 git diff 检查差异，找出需更新的文档
- **更新现有的文档**：添加或修改 props 表格、更新代码示例、添加废弃通知
- **为新功能创建脚手架文档**：提供标准模板，确保新文档符合项目要求

---

## 查找 Skill (find-skills)

| 属性 | 内容 |
|------|------|
| **作者** | vercel |
| **地址** | https://github.com/vercel-labs/skills/tree/main/skills/find-skills |

### 简介

该 Skill 主要作用帮助你发现并安装 Agent Skill。它依托名为 skills 的命令行工具（CLI），让你可以从开放的 Agent Skill 生态中搜索、安装与管理各类模块化技能包。

### 资源文件

- SKILL.md

### 应用场景

- **探索未知的 Skill**：询问 Agent 是否具备某项能力时，自动搜索相关技能
- **查找特定的 Skill**：使用关键词精确查找匹配的技能
- **提供可执行的 Skill 安装建议**：提供技能名称、功能简介、一键安装指令和官方链接

---

*本文整理自 [TRAE CN 文档](https://docs.trae.cn/ide/top-10-recommended-skills-for-development-scenarios)*