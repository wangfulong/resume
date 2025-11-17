# CLAUDE.md - AI Assistant Guide for Resume Repository

## Repository Overview

This is a **professional resume repository** for 王复隆 (Wang Fulong), a Senior Full-Stack Software Engineer. The repository maintains a structured, version-controlled resume in Markdown format.

**Key Information:**
- **Owner:** wangfulong (wfllike@gmail.com)
- **Purpose:** Personal resume/CV documentation
- **Primary File:** `README.md` (contains the complete resume)
- **Language:** Simplified Chinese (简体中文)
- **Format:** Markdown with structured sections

## Repository Structure

```
/home/user/resume/
├── .git/                    # Git repository metadata
├── README.md               # Main resume content (Chinese)
└── CLAUDE.md               # This file - AI assistant guide
```

**File Details:**
- `README.md` - The complete resume (~102 lines, 4.5KB)
- No source code files
- No build configurations
- No package dependencies

## Content Structure

The resume follows a standard professional format with these sections:

### 1. **Header**
```markdown
wfllike@gmail.com | 15210594796

# 王复隆 - Senior Full-Stack Engineer
```

### 2. **Summary (概况)**
- Brief professional overview (8 years experience)
- Core competencies and focus areas
- Key strengths

### 3. **Education (教育背景)**
- University: 首都师范大学 (Capital Normal University)
- Degree: Computer Science (学士)
- Years: 2009 - 2013

### 4. **Skills (技能)**
Organized by category:
- **Languages** - JavaScript, TypeScript, Java, Solidity, CSS/LESS, HTML
- **Frontend** - React, Vue, Next.js, Electron, Redux, etc.
- **Backend** - Node.js, Express, Spring Boot, Meteor
- **Engineering** - Vite, Webpack, Jenkins, OpenAPI Generator
- **Database** - MongoDB, Realm, Redis, MySQL, Oracle
- **Web3 & Other** - Smart Contracts, GraphQL, gRPC, Protocol Buffers

### 5. **Experience (工作经历)**
Listed in reverse chronological order:
1. **RockFlow** (2021/11 - 至今) - Senior Full-Stack Engineer
2. **快手科技 (Kuaishou)** (2018/5 - 2021/11) - Senior Front-End Engineer
3. **一起写 Office** (2016/10 - 2018/5) - Front-End Engineer
4. **北京点聚信息科技** (2014/9 - 2016/10) - Software Engineer

## Development Workflows

### Making Resume Updates

When updating the resume, follow this workflow:

1. **Review Current Content**
   ```bash
   # Read the current README.md first
   cat README.md
   ```

2. **Make Targeted Changes**
   - Use precise edits rather than rewriting entire sections
   - Preserve existing formatting and structure
   - Maintain Chinese language and professional tone
   - Keep quantifiable achievements (metrics, percentages)

3. **Verify Changes**
   - Ensure Markdown formatting is valid
   - Check that contact information hasn't been accidentally modified
   - Verify dates are in correct format (YYYY/MM or YYYY)
   - Confirm URLs are functional (if adding/modifying)

4. **Commit with Descriptive Messages**
   - Use Chinese for commit messages (matching repository style)
   - Be specific about what was changed
   - Examples:
     - "更新工作经历" (Update work experience)
     - "优化技能描述" (Optimize skills description)
     - "添加新项目成果" (Add new project achievements)

### Git Workflow

**Branch Strategy:**
- **Main Branch:** Primary branch for stable resume versions
- **Feature Branches:** Use `claude/` prefix for AI-generated changes
  - Format: `claude/claude-md-{random-id}-{session-id}`
  - Example: `claude/claude-md-mi2s0atsnd1o3qq9-01C3rVmYXnXxkWqs34YDeXJL`

**Commit Guidelines:**
```bash
# Stage changes
git add README.md

# Commit with descriptive message (Chinese preferred)
git commit -m "优化简历结构和内容表述"

# Push to feature branch
git push -u origin claude/claude-md-{branch-name}
```

**Pull Request Process:**
- Create PR from feature branch to main branch
- Use descriptive PR titles in Chinese
- Review changes carefully before merging

### Network Retry Policy

For git operations that may fail due to network issues:

**Push Operations:**
```bash
# Retry up to 4 times with exponential backoff (2s, 4s, 8s, 16s)
git push -u origin <branch-name>
```

**Fetch/Pull Operations:**
```bash
# Prefer specific branch fetches
git fetch origin <branch-name>
git pull origin <branch-name>
```

## Formatting Standards

### Markdown Conventions

**Headers:**
- H1 (`#`) - Name and title only
- H2 (`##`) - Major sections (Summary, Education, Skills, Experience)
- H3 (`###`) - Company names and subsections

**Lists:**
- Use `-` for unordered lists (bullet points)
- Maintain consistent indentation
- Group related items together

**Emphasis:**
- `**Bold**` for company names, roles, key terms
- No italics used in current format

**Links:**
- Include full URLs for project demonstrations
- Format: `https://example.com` or `[text](url)`
- Examples in resume:
  - `https://rockflow.ai` (official website)
  - `https://meta.rockflow.ai` (NFT project)
  - `https://help.rockflow.ai` (help center)

**Dates:**
- Format: `YYYY/MM - YYYY/MM` or `YYYY/MM - 至今` (present)
- Example: `2021/11 - 至今`

**Metrics & Achievements:**
- Include specific numbers and percentages
- Use bold for impressive metrics
- Format: `提升 X 倍`, `从 X% 提升至 Y%`, `节省 X% 工作量`

### Language Style

**Chinese Writing Guidelines:**
- Use Simplified Chinese (简体中文)
- Professional, concise tone
- Action-oriented descriptions (主导、设计、实现、优化)
- Include quantifiable results where possible
- Technical terms: Mix of Chinese and English
  - Use English for: technology names, tools, frameworks
  - Use Chinese for: descriptions, achievements, roles

**Common Patterns:**
```
- 技术栈：[Technology Stack]
- 业务成果：[Business Results]
- 核心成就：[Core Achievements]
- 独立负责 [Independently responsible for]
- 主导设计 [Led the design of]
- 从零参与构建 [Built from scratch]
```

## Key Conventions for AI Assistants

### ✅ DO

1. **Preserve Structure**
   - Maintain the existing section order
   - Keep consistent formatting throughout
   - Preserve contact information exactly as-is

2. **Use Metrics**
   - Include quantifiable achievements
   - Highlight conversion rates, performance improvements
   - Show impact with numbers (10x, 90% reduction, etc.)

3. **Be Specific**
   - Name technologies explicitly
   - Include project URLs when relevant
   - Provide context for achievements

4. **Follow Date Format**
   - Use `YYYY/MM` format consistently
   - Use `至今` for current positions
   - Maintain reverse chronological order

5. **Maintain Professional Tone**
   - Focus on accomplishments and impact
   - Use action verbs (设计, 实现, 主导, 优化)
   - Keep descriptions concise but informative

6. **Version Control Best Practices**
   - Read file before editing
   - Make targeted edits, not full rewrites
   - Write clear commit messages in Chinese
   - Push to appropriate branch (claude/* for AI)

### ❌ DON'T

1. **Don't Modify Contact Info** unless explicitly requested
2. **Don't Remove Quantifiable Metrics** - they demonstrate impact
3. **Don't Mix Languages** - keep descriptions in Chinese, tech terms in English
4. **Don't Add Unverified Information** - only use provided facts
5. **Don't Change Date Formats** - maintain consistency
6. **Don't Remove URLs** - they provide proof of work
7. **Don't Use Emojis** - keep professional tone
8. **Don't Create New Sections** without good reason
9. **Don't Reorder Experience** - must remain chronological (newest first)
10. **Don't Push to Main** - always use feature branches

### Common Tasks

**Adding New Experience:**
1. Add to top of Experience section (most recent first)
2. Include: Company | Role | Date range
3. List projects with bullet points
4. Highlight quantifiable achievements
5. Include relevant technologies used

**Updating Skills:**
1. Maintain category groupings
2. Add new skills to appropriate category
3. Keep alphabetical or priority order within categories
4. Use commas to separate items

**Optimizing Content:**
1. Make descriptions more concise
2. Add missing metrics if available
3. Improve clarity without changing meaning
4. Ensure technical accuracy

## Technical Context

### Technologies Referenced in Resume

**Frontend Frameworks:**
- React, Vue (Vue3), Next.js (SSR/SSG)
- Electron (Desktop apps)
- State Management: Redux, Redux-Saga, Vuex, Flux

**Backend Technologies:**
- Node.js, Express, Meteor
- Spring Boot, Java
- GraphQL, gRPC, Protocol Buffers

**Web3 & Blockchain:**
- Solidity (Smart Contracts)
- NFT development
- Ethereum (Contract: 0x39b782a817ce07ff9947bb96ba9df001aad731fb)

**Build & DevOps:**
- Vite, Webpack, Jenkins
- OpenAPI Generator
- Sentry (monitoring)
- Docusaurus (documentation)
- Algolia (search)

**Databases:**
- MongoDB, Realm
- Redis (caching)
- MySQL, Oracle

### Notable Projects

1. **RockFlow Official Website** - https://rockflow.ai
   - Next.js SSR, SEO optimized (Lighthouse 100)
   - Google Search #1 for brand keywords

2. **NFT Meta Platform** - https://meta.rockflow.ai
   - Smart contract on Ethereum
   - Hybrid centralized/decentralized approach
   - 100% test coverage

3. **Help Center** - https://help.rockflow.ai
   - Docusaurus SSG
   - Algolia search integration
   - Self-hosted DocSearch Crawler

4. **Kim IM System** (Kuaishou)
   - Electron + React + GraphQL
   - Enterprise communication platform

## Repository History

**Recent Commits:**
```
d959624 - Merge pull request #1
b6e0f7d - 优化简历结构和内容表述
7fdc568 - update
c13e61a - update
f8c5356 - update
```

**First Commit:** 2021-09-14
**Latest Update:** 2025-10-22 (Claude optimization)

## Best Practices Summary

### For Content Updates

1. **Read First** - Always read README.md before making changes
2. **Targeted Edits** - Use Edit tool for specific changes, not full rewrites
3. **Preserve Format** - Maintain existing Markdown structure
4. **Verify Links** - Ensure URLs are valid if adding/modifying
5. **Check Dates** - Verify date formats match existing style
6. **Review Metrics** - Preserve and highlight quantifiable achievements

### For Git Operations

1. **Branch Naming** - Use `claude/` prefix for AI-generated branches
2. **Commit Messages** - Write clear, descriptive messages in Chinese
3. **Push Strategy** - Always push to feature branch, never directly to main
4. **Pull Requests** - Create PR for review before merging
5. **Network Resilience** - Retry failed operations with exponential backoff

### For Communication

1. **Professional Tone** - Match the resume's professional style
2. **Technical Accuracy** - Verify technology names and terminology
3. **Quantifiable Impact** - Emphasize metrics and measurable results
4. **Concise Writing** - Clear, action-oriented descriptions
5. **Bilingual Balance** - Chinese descriptions, English tech terms

---

## Quick Reference

**Primary File:** `README.md`
**Language:** Simplified Chinese
**Format:** Markdown
**Main Branch:** `main`
**AI Branch Prefix:** `claude/`
**Commit Language:** Chinese (preferred)
**Date Format:** `YYYY/MM`
**Current Position:** RockFlow (2021/11 - 至今)

---

**Last Updated:** 2025-11-17
**Version:** 1.0
**Maintained By:** AI Assistant (Claude)
