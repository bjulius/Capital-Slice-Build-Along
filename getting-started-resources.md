# Getting Started: Building Great Claude Skills

A curated collection of free resources to help you get started with Claude Code, Visual Studio Code, Git/GitHub, and Claude Skills development.

---

## Claude Code

| Resource | Description |
|----------|-------------|
| [Claude Code Overview](https://code.claude.com/docs/en/overview) | Official documentation covering installation, features, and configuration |
| [Net Ninja Claude Code Tutorial](https://youtube.com/playlist?list=PLqyUgadpThTIkF2lgMlu3PlUrl2dODiRk&si=K20nG9Br2na8NAmb) | 10-part video course covering CLAUDE.md, tools, MCP servers, subagents, and GitHub integration |
| [Claude Code GitHub Repository](https://github.com/anthropics/claude-code) | Source repo with installation instructions, issue tracking, and community discussions |
| [Claude Code Best Practices](https://www.anthropic.com/engineering/claude-code-best-practices) | Anthropic's engineering guide on CLAUDE.md files and effective workflows |
| [ClaudeLog](https://claudelog.com/) | Community-maintained docs, guides, tutorials, and best practices |

**Quick Start:** Install with `npm install -g @anthropic-ai/claude-code`, navigate to your project, and run `claude`.

---

## Visual Studio Code

| Resource | Description |
|----------|-------------|
| [VS Code Getting Started Tutorial](https://code.visualstudio.com/docs/getstarted/getting-started) | Official walkthrough of the UI, code editing features, and debugging |
| [VS Code Introductory Videos](https://code.visualstudio.com/docs/getstarted/introvideos) | Short video series (2-7 min each) covering setup, productivity tips, and extensions |
| [VS Code Documentation](https://code.visualstudio.com/docs) | Comprehensive reference for all features including GitHub Copilot integration |
| [Beginner VS Code (Udemy - Free)](https://www.udemy.com/course/beginner-vs-code/) | Free course focused on HTML, CSS, and JavaScript development in VS Code |

**Why VS Code?** It's free, cross-platform, and has excellent Git integration built-in. The Claude Code extension works seamlessly with it.

---

## Git & GitHub

| Resource | Description |
|----------|-------------|
| [Net Ninja Git & GitHub Tutorial](https://www.youtube.com/playlist?list=PL4cUxeGkcC9goXbgTDQ0n_4TBzOO0ocPR) | Free YouTube playlist - beginner-friendly video tutorials by Shaun Pelling |
| [GitHub Skills](https://docs.github.com/en/get-started/start-your-journey/git-and-github-learning-resources) | Free interactive courses built into GitHub with automated feedback |
| [W3Schools Git Tutorial](https://www.w3schools.com/git/) | Track your progress through fundamentals of Git and remote repositories |
| [Git and GitHub for Beginners (HubSpot)](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners) | Step-by-step guide to pull requests, branching, and merging |
| [GeeksforGeeks Git Tutorial](https://www.geeksforgeeks.org/git/git-tutorial/) | Comprehensive reference covering version control concepts and commands |

### Solo Developer: Minimum Git Knowledge

If you're working alone (not collaborating with a team), you only need these **6 commands** to get started:

| Command | What It Does |
|---------|--------------|
| `git init` | Create a new repository in your project folder |
| `git add .` | Stage all changed files for commit |
| `git commit -m "message"` | Save a snapshot of your staged changes |
| `git status` | See what files have changed since last commit |
| `git log --oneline` | View your commit history |
| `git push` | Upload your commits to GitHub (backup + sharing) |

**Solo Developer Workflow:**
1. Create a repo on GitHub, clone it locally (or `git init` + connect to remote)
2. Write code, then `git add .` and `git commit -m "what you did"`
3. `git push` to back up your work to GitHub
4. Repeat steps 2-3 as you work

**What you can skip for now:** Branching, merging, pull requests, rebasing, and stashing are collaboration features. Learn them later when you start working with others.

---

## Claude Skills Development

| Resource | Description |
|----------|-------------|
| [Introducing Agent Skills (Anthropic)](https://www.anthropic.com/news/skills) | Official announcement explaining what skills are and how they work |
| [Agent Skills Documentation](https://docs.claude.com/en/docs/agents-and-tools/agent-skills/overview) | Official docs on skill structure, SKILL.md format, and best practices |
| [Skills GitHub Repository](https://github.com/anthropics/skills) | Open-source skills including document creation (docx, pdf, pptx, xlsx) |
| [Equipping Agents for the Real World](https://www.anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) | Anthropic engineering deep-dive on skill architecture and design philosophy |
| [Claude Skills Explained (Lenny's Newsletter)](https://www.lennysnewsletter.com/p/claude-skills-explained) | Clear explanation of skills with practical workflow examples |
| [Simon Willison on Claude Skills](https://simonwillison.net/2025/Oct/16/claude-skills/) | Independent analysis: "maybe a bigger deal than MCP" |

**Skill Anatomy:** At minimum, a skill is a folder with a `SKILL.md` file containing YAML frontmatter (name, description) and markdown instructions. Optional folders include `scripts/`, `references/`, and `assets/`.

---

*All resources listed are free unless otherwise noted. Last updated: December 2025.*
