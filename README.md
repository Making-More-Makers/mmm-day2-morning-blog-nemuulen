# Assignment: Day 2 Morning - Build Your Technical Blog
# 作业：第2天上午 - 搭建你的技术博客

> **📚 This is a GitHub Classroom Assignment**  
> **这是一个 GitHub Classroom 作业**  
>   
> **Students**: Follow this handbook step-by-step to build your own Docusaurus blog and deploy it to GitHub Pages.  
> **学生**：按照本手册逐步操作，搭建你自己的 Docusaurus 博客并部署到 GitHub Pages。

---

## 📋 Assignment Overview | 作业概览

Welcome to Day 2! Today you'll build something that will last long after this course ends: **your own professional technical blog**. 🎉

欢迎来到第2天！今天你将创建一个在课程结束后仍然对你有用的东西：**你自己的专业技术博客**。🎉

**What You'll Build | 你将搭建什么：**
- ✅ A professional technical blog using Docusaurus (使用 Docusaurus 的专业技术博客)
- ✅ Your Maker Profile showcasing who you are (展示你是谁的 Maker 档案)
- ✅ Documentation of your Day 1 projects (你第1天项目的文档)
- ✅ A project tracking wiki for the 6-day course (6天课程的项目追踪 wiki)
- ✅ Deployed live on the internet via GitHub Pages (通过 GitHub Pages 部署到互联网)

**Timeline | 时间线：**
- ⏰ **Part 1 (60 min)** | **第1部分（60分钟）**: Environment Setup & Local Development | 环境配置与本地开发
- ⏰ **Part 2 (30 min)** | **第2部分（30分钟）**: Content Creation | 内容创作
- ⏰ **Part 3 (30 min)** | **第3部分（30分钟）**: GitHub Pages Deployment | GitHub Pages 部署

---

## 🎯 Learning Objectives | 学习目标

By completing this assignment, you will:

完成此作业后，你将：

- ✅ Understand how to build a static site with Docusaurus | 理解如何使用 Docusaurus 搭建静态网站
- ✅ Learn to write content in Markdown format | 学会使用 Markdown 格式写内容
- ✅ Deploy a website to GitHub Pages | 部署网站到 GitHub Pages
- ✅ Create professional project documentation | 创建专业的项目文档
- ✅ Build your online presence as a Maker | 建立作为 Maker 的在线形象
- ✅ Learn modern web development workflows | 学习现代网页开发工作流

---

## 📦 What to Submit | 提交内容

You need to submit **2 things** for this assignment:

你需要为此作业提交 **2 项内容**：

### 1. 🌐 Your GitHub Pages URL
The live URL of your deployed blog (部署后博客的在线 URL)

**Format | 格式**: `https://your-username.github.io/your-blog-name/`

### 2. 📸 Screenshot
A full-page screenshot of your deployed blog showing:
- The URL bar with your GitHub Pages URL visible (URL 栏显示你的 GitHub Pages URL)
- Your blog homepage with content (博客首页及内容)
- Evidence of at least 3 pages: Home, Maker Profile, Project Tracking (至少3个页面的证据)

**See [SUBMISSION.md](./SUBMISSION.md) for detailed submission instructions.**

**详细提交说明见 [SUBMISSION.md](./SUBMISSION.md)。**

---

## ✅ Prerequisites | 前置要求

Before starting, make sure you have:

开始之前，确保你有：

- [ ] A GitHub account (GitHub 账号)
- [ ] Basic understanding of Git (Git 基础理解)
- [ ] A code editor installed (VS Code, Cursor, etc.) (已安装代码编辑器)
- [ ] Terminal/Command Prompt access (终端/命令提示符访问权限)
- [ ] Stable internet connection (稳定的互联网连接)
- [ ] **Node.js 18+ installed** (已安装 Node.js 18+)
- [ ] **Yarn installed** (已安装 Yarn)

**Don't have Node.js or Yarn?** See [Part 1, Step 1](#step-1-install-nodejs) below.

**还没有 Node.js 或 Yarn？** 请看下面的[第1部分，步骤1](#step-1-install-nodejs)。

---

## 🚀 Part 1: Environment Setup (60 minutes)
## 🚀 第1部分：环境配置（60分钟）

### Step 1: Install Node.js
### 步骤1：安装 Node.js

**What is Node.js? | 什么是 Node.js？**

Node.js is a JavaScript runtime that allows you to run JavaScript outside of a web browser. We need it to run Docusaurus.

Node.js 是一个 JavaScript 运行环境，允许你在网页浏览器之外运行 JavaScript。我们需要它来运行 Docusaurus。

**Check if you already have Node.js | 检查是否已安装 Node.js：**

Open your terminal (Terminal on Mac/Linux, Command Prompt or PowerShell on Windows) and run:

打开终端（Mac/Linux 上的 Terminal，Windows 上的 Command Prompt 或 PowerShell）并运行：

```bash
node --version
```

If you see a version number like `v18.0.0` or higher, **you're good to go! Skip to Step 2.**

如果看到 `v18.0.0` 或更高版本号，**你已经准备好了！跳到步骤2。**

If you see `command not found` or a version lower than v18, follow the installation steps below:

如果看到 `command not found` 或版本低于 v18，请按照下面的安装步骤操作：

#### Installation Instructions | 安装说明

**For Windows | Windows 系统：**

1. Go to https://nodejs.org/
2. Download the **LTS version** (recommended) (下载 **LTS 版本**（推荐）)
3. Run the installer and follow the prompts (运行安装程序并按照提示操作)
4. Restart your terminal after installation (安装后重启终端)
5. Verify with `node --version` (用 `node --version` 验证)

**For Mac | Mac 系统：**

Option A - Using the installer (使用安装程序):
1. Go to https://nodejs.org/
2. Download the **LTS version** (下载 **LTS 版本**)
3. Run the .pkg installer (运行 .pkg 安装程序)
4. Verify with `node --version`

Option B - Using Homebrew (推荐，使用 Homebrew):
```bash
brew install node
```

**For Linux | Linux 系统：**

```bash
# Ubuntu/Debian
curl -fsSL https://deb.nodesource.com/setup_lts.x | sudo -E bash -
sudo apt-get install -y nodejs

# Verify installation
node --version
```

⏱️ **Expected time**: 5-10 minutes (预计时间：5-10分钟)

---

### Step 1.5: Install Yarn
### 步骤1.5：安装 Yarn

**What is Yarn? | 什么是 Yarn？**

Yarn is a fast, reliable package manager for JavaScript. It's an alternative to npm and offers faster installation speeds and better dependency management.

Yarn 是一个快速、可靠的 JavaScript 包管理器。它是 npm 的替代品，提供更快的安装速度和更好的依赖管理。

**Check if you already have Yarn | 检查是否已安装 Yarn：**

```bash
yarn --version
```

If you see a version number like `1.22.0` or higher, **you're good to go! Skip to Step 2.**

如果看到 `1.22.0` 或更高版本号，**你已经准备好了！跳到步骤2。**

If you see `command not found`, follow the installation steps below:

如果看到 `command not found`，请按照下面的安装步骤操作：

#### Installation Instructions | 安装说明

**Method 1: Using Corepack (Recommended for Node.js 16.10+) | 方法1：使用 Corepack（推荐 Node.js 16.10+ 使用）**

Corepack comes with Node.js and allows you to enable Yarn easily:

Corepack 随 Node.js 一起提供，让你可以轻松启用 Yarn：

```bash
# Enable Corepack
# 启用 Corepack
corepack enable

# Verify Yarn is installed
# 验证 Yarn 已安装
yarn --version
```

**Method 2: Using npm (Works on all systems) | 方法2：使用 npm（适用于所有系统）**

```bash
# Install Yarn globally using npm
# 使用 npm 全局安装 Yarn
npm install -g yarn

# Verify installation
# 验证安装
yarn --version
```

**For Windows (Alternative - using installer) | Windows 系统（替代方法 - 使用安装程序）：**

1. Download the installer from https://classic.yarnpkg.com/en/docs/install#windows-stable
2. Run the `.msi` installer (运行 `.msi` 安装程序)
3. Restart your terminal (重启终端)
4. Verify with `yarn --version` (用 `yarn --version` 验证)

**For Mac (Alternative - using Homebrew) | Mac 系统（替代方法 - 使用 Homebrew）：**

```bash
brew install yarn
```

**For Linux | Linux 系统：**

```bash
# Ubuntu/Debian
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update && sudo apt install yarn

# Verify installation
yarn --version
```

⏱️ **Expected time**: 2-5 minutes (预计时间：2-5分钟)

---

### Step 2: Create Your Docusaurus Project
### 步骤2：创建你的 Docusaurus 项目

Now that you have Node.js installed, let's create your blog!

现在你已经安装了 Node.js，让我们创建你的博客吧！

**Open your terminal** and navigate to where you want to create your blog project:

**打开终端**并导航到你想创建博客项目的位置：

```bash
# Navigate to your desired directory
# 导航到你想要的目录
cd Documents
# or on Windows: cd C:\Users\YourName\Documents
```

**Create your Docusaurus project | 创建你的 Docusaurus 项目：**

```bash
yarn create docusaurus my-maker-blog classic
```

**What does this command do? | 这个命令做什么？**
- `yarn create`: Creates a new project using Yarn (使用 Yarn 创建新项目)
- `docusaurus`: The Docusaurus package (Docusaurus 包)
- `my-maker-blog`: Your blog's folder name (you can change this!) (你的博客文件夹名称（可以修改！）)
- `classic`: Uses the classic template (使用经典模板)

**What you'll see | 你会看到：**
1. Lots of text scrolling in your terminal (终端中滚动的大量文本)
2. Some warnings about peer dependencies - **this is normal, ignore them** (一些关于 peer dependencies 的警告 - **这是正常的，忽略它们**)
3. A question asking "Which language do you want to use?" (一个问题询问"Which language do you want to use?"）

**⚠️ IMPORTANT: When asked to choose a language | 重要：当被要求选择语言时：**

```
? Which language do you want to use?
>   JavaScript    ← Select this! 选择这个！按 Enter
    TypeScript
```

**Use arrow keys to select JavaScript, then press Enter.**

**使用箭头键选择 JavaScript，然后按 Enter。**

💡 **Why JavaScript?** (为什么选 JavaScript？)
- Easier for beginners (对初学者更容易)
- No extra typing configuration needed (不需要额外的类型配置)
- Works perfectly for this course (对本课程完全够用)

**Success! You should see | 成功！你应该看到：**
```
Success! Created my-maker-blog
```

⏱️ **Expected time**: 2-3 minutes (预计时间：2-3分钟)

---

### Step 3: Navigate to Your Project
### 步骤3：进入你的项目

```bash
cd my-maker-blog
```

`cd` means "change directory" - we're entering the folder we just created.

`cd` 意思是"切换目录" - 我们正在进入刚创建的文件夹。

---

### Step 4: Initialize Git Repository
### 步骤4：初始化 Git 仓库

**Why do this now? | 为什么现在做？**

Before making any changes, let's set up Git version control. This allows you to:
- Track all your changes (跟踪所有更改)
- Undo mistakes easily (轻松撤销错误)
- Prepare for GitHub deployment (为 GitHub 部署做准备)

在进行任何更改之前，让我们设置 Git 版本控制。这允许你：
- 跟踪所有更改
- 轻松撤销错误
- 为 GitHub 部署做准备

**Initialize Git and make your first commit | 初始化 Git 并进行第一次提交：**

```bash
# Initialize git repository
# 初始化 git 仓库
git init

# Check git status (you'll see many untracked files)
# 检查 git 状态（你会看到许多未跟踪的文件）
git status

# Add all files to staging
# 将所有文件添加到暂存区
git add .

# Create your first commit
# 创建第一次提交
git commit -m "Initial commit - Fresh Docusaurus blog"
```

**What just happened? | 刚才发生了什么？**

1. `git init` - Created a `.git` folder to track changes (创建 `.git` 文件夹来跟踪更改)
2. `git add .` - Staged all files for commit (将所有文件暂存以进行提交)
3. `git commit` - Saved a snapshot of your project (保存项目快照)

**Success! You should see | 成功！你应该看到：**
```
[main (root-commit) xxxxxxx] Initial commit - Fresh Docusaurus blog
 XX files changed, XXXX insertions(+)
 create mode 100644 ...
```

💡 **Pro Tip | 专业提示:**
From now on, commit your changes regularly as you work!
从现在开始，在工作时定期提交更改！

⏱️ **Expected time**: 2 minutes (预计时间：2分钟)

---

### Step 5: Install Dependencies
### 步骤5：安装依赖

```bash
yarn install
```

**What does this do? | 这做什么？**

This installs all the packages and libraries that Docusaurus needs to run. You'll see hundreds of packages being downloaded - this is normal for modern web development!

这会安装 Docusaurus 运行所需的所有包和库。你会看到数百个包被下载 - 这对现代 Web 开发来说很正常！

⏱️ **Expected time**: 1-2 minutes (预计时间：1-2分钟)

**⚠️ Common Issues | 常见问题：**

**Issue: `yarn ERR! network timeout`**
```bash
# Solution: Clear cache and try again
# 解决方案：清除缓存并重试
yarn cache clean
yarn install
```

**Issue: Permission denied (Mac/Linux)**
```bash
# Yarn typically doesn't have permission issues like npm
# If you encounter any, try clearing the cache
# Yarn 通常不会像 npm 那样有权限问题
# 如果遇到任何问题，尝试清除缓存
yarn cache clean
```

---

### Step 6: Start the Development Server
### 步骤6：启动开发服务器

This is the exciting moment! Let's see your blog in action.

这是激动人心的时刻！让我们看看你的博客运行起来。

```bash
yarn start
```

**What happens? | 会发生什么？**
- Your terminal will show "Starting the development server..." (终端显示"Starting the development server...")
- A browser window will automatically open (浏览器窗口会自动打开)
- You'll see your blog at `http://localhost:3000` (你会在 `http://localhost:3000` 看到你的博客)

**What you should see | 你应该看到：**
- A website with a dinosaur mascot (恐龙吉祥物) 🦖
- The title "My Site" at the top ("My Site" 标题在顶部)
- Navigation menu with "Docs", "Blog", "GitHub" (导航菜单)
- A hero section with buttons (英雄区域和按钮)

🎉 **Congratulations! Your blog is running locally!** 

🎉 **恭喜！你的博客在本地运行了！**

⏱️ **Expected time**: 30 seconds to 1 minute (预计时间：30秒到1分钟)

---

### Step 7: Understand the Project Structure
### 步骤7：理解项目结构

**Open your code editor** (VS Code, Cursor, etc.) and open the `my-maker-blog` folder.

**打开你的代码编辑器**（VS Code, Cursor 等）并打开 `my-maker-blog` 文件夹。

You'll see this structure (你会看到这个结构):

```
my-maker-blog/
├── blog/                    ← Blog posts go here | 博客文章放这里
│   ├── 2024-11-21-welcome.md
│   └── ...
├── docs/                    ← Documentation pages | 文档页面放这里
│   └── intro.md
├── src/
│   └── pages/              ← Custom pages (About, Projects) | 自定义页面
│       └── index.js
├── static/                 ← Images and static files | 图片和静态文件
│   └── img/
├── docusaurus.config.js    ← Site configuration | 网站配置 ⭐
├── sidebars.js             ← Sidebar configuration | 侧边栏配置
└── package.json            ← Project info | 项目信息
```

**Key folders to remember | 要记住的关键文件夹：**

📝 **`blog/`**: Your blog posts go here (博客文章放这里)
- Each file is a blog post (每个文件是一篇博客文章)
- Files use Markdown format (文件使用 Markdown 格式)

📄 **`docs/`**: Documentation pages (文档页面)
- Perfect for project documentation (适合项目文档)
- We'll put your Maker Profile here (我们会把你的 Maker 档案放这里)

🖼️ **`static/`**: Images and files (图片和文件)
- Put your project photos here (把项目照片放这里)
- Put wiring diagrams here (把接线图放这里)

⚙️ **`docusaurus.config.js`**: Website configuration (网站配置) ⭐ IMPORTANT!
- Site title, URL, theme settings (网站标题、URL、主题设置)
- We'll edit this later for deployment (稍后我们会编辑它以进行部署)

---

### Step 8: Make Your First Edit
### 步骤8：进行第一次编辑

Let's personalize your blog! We'll change the site title.

让我们个性化你的博客！我们将更改网站标题。

**Open `docusaurus.config.js` in your editor.**

**在编辑器中打开 `docusaurus.config.js`。**

Find these lines near the top (在顶部附近找到这些行):

```javascript
const config = {
  title: 'My Site',
  tagline: 'Dinosaurs are cool',
  // ...
```

**Change them to | 更改为:**

```javascript
const config = {
  title: 'My Maker Journey',
  tagline: 'Building, Learning, Creating',
  // ...
```

**Save the file.** Then look at your browser - the changes appear automatically! This is called "hot reloading". 🔥

**保存文件。**然后看你的浏览器 - 更改自动出现！这叫做"热重载"。🔥

⏱️ **Expected time**: 2 minutes (预计时间：2分钟)

---

### Step 9: Commit Your First Changes
### 步骤9：提交你的第一次更改

**Now that you've made changes, let's save them with Git!**

**现在你已经做了更改，让我们用 Git 保存它们！**

```bash
# Check what files have changed
# 检查哪些文件发生了更改
git status

# You should see "docusaurus.config.js" as modified
# 你应该看到 "docusaurus.config.js" 被标记为已修改

# Add the changes
# 添加更改
git add docusaurus.config.js

# Commit with a descriptive message
# 用描述性信息提交
git commit -m "Personalize blog title and tagline"
```

💡 **Git Best Practices | Git 最佳实践:**
- Commit often (经常提交)
- Write clear commit messages (写清楚的提交信息)
- Describe WHAT you changed and WHY (描述你改了什么和为什么)

**Good commit messages | 好的提交信息:**
```bash
✅ "Add Maker Profile page"
✅ "Update Day 1 project documentation"
✅ "Fix navigation menu links"
```

**Bad commit messages | 不好的提交信息:**
```bash
❌ "update"
❌ "fix"
❌ "changes"
```

⏱️ **Expected time**: 2 minutes (预计时间：2分钟)

---

### 🎉 Part 1 Complete! | 第1部分完成！

You now have:
- ✅ Node.js and Yarn installed (安装了 Node.js 和 Yarn)
- ✅ A Docusaurus project created (创建了 Docusaurus 项目)
- ✅ Git initialized and changes tracked (初始化了 Git 并跟踪更改)
- ✅ Development server running locally (本地运行开发服务器)
- ✅ Understanding of project structure (理解项目结构)
- ✅ Made and committed your first edit (进行并提交了第一次编辑)

**Take a 5-minute break! Stretch, get water, then come back for Part 2.** 💧

**休息5分钟！伸展、喝水，然后回来进行第2部分。** 💧

---

## ✍️ Part 2: Content Creation (30 minutes)
## ✍️ 第2部分：内容创作（30分钟）

Now let's add your content! You'll create three pages:

现在让我们添加你的内容！你将创建三个页面：

1. **Maker Profile** - Who you are (你是谁)
2. **Day 1 Projects** - What you built yesterday (昨天你做了什么)
3. **Project Tracking** - Your 6-day course wiki (你的6天课程 wiki)

---

### Step 10: Create Your Maker Profile
### 步骤10：创建你的 Maker 档案

**Create a new file | 创建新文件**: `docs/maker-profile.md`

Copy and paste this template, then fill in your information:

复制并粘贴此模板，然后填写你的信息：

```markdown
---
sidebar_position: 1
---

# My Maker Profile
# 我的 Maker 档案

## About Me | 关于我

**Name | 姓名**: [Your Name]

**Background | 背景**: [Tell us about yourself - where you're from, what you study, what interests you]

**Why I'm Here | 为什么来参加**: [Why did you join this course? What motivated you?]

## My Interests | 我的兴趣

- [Interest 1]
- [Interest 2]
- [Interest 3]

## Skills I Have | 我拥有的技能

- **Programming | 编程**: [e.g., Python, Arduino, none yet!]
- **Hardware | 硬件**: [e.g., circuits, soldering, beginner]
- **Other | 其他**: [e.g., 3D design, art, photography]

## Skills I Want to Learn | 我想学习的技能

1. [Skill 1]
2. [Skill 2]
3. [Skill 3]

## My Maker Identity | 我的 Maker 身份

Which Maker principle resonates with me most?

最能引起我共鸣的 Maker 原则是什么？

> [Share which principle from Day 1 you connect with and why]

## My 6-Day Goals | 我的6天目标

By the end of this course, I want to:

在本课程结束时，我想要：

- [ ] [Goal 1]
- [ ] [Goal 2]
- [ ] [Goal 3]

## Contact | 联系方式

- **GitHub**: [@your-username](https://github.com/your-username)
- **Email**: your.email@example.com
```

⏱️ **Expected time**: 10 minutes (预计时间：10分钟)

**💾 Commit your changes | 提交你的更改:**
```bash
git add docs/maker-profile.md
git commit -m "Add Maker Profile page"
```

---

### Step 11: Document Your Day 1 Projects
### 步骤11：记录你的第1天项目

**Create a new file | 创建新文件**: `docs/day1-projects.md`

```markdown
---
sidebar_position: 2
---

# Day 1 Projects
# 第1天项目

## Morning: Spaghetti Marshmallow Challenge
## 上午：Spaghetti Marshmallow 挑战

### Challenge Results | 挑战结果

- **Team Name | 团队名称**: [Your team name]
- **Final Height | 最终高度**: [X cm]
- **Marshmallow on Top? | 棉花糖在顶部？**: [Yes/No]

### Our Approach | 我们的方法

[Describe your team's strategy]

### What We Learned | 我们学到了什么

1. [Learning 1]
2. [Learning 2]
3. [Learning 3]

### Photos | 照片

[If you have photos, add them here]

---

## Afternoon: Arduino Hardware CTF
## 下午：Arduino 硬件 CTF

### Flags Captured | 捕获的 Flag

- [ ] Flag 1: Sensor Reading
- [ ] Flag 2: Actuator Control
- [ ] Flag 3: Sensor to Actuator
- [ ] Flag 4: Complex Logic
- [ ] Flag 5: Creative Project

### My Favorite Challenge | 我最喜欢的挑战

**Which flag was most interesting? | 哪个 flag 最有趣？**

[Share about your favorite challenge and what you learned]

### Arduino Code Snippet | Arduino 代码片段

Here's a code snippet from one of my challenges:

这是我某个挑战中的代码片段：

```cpp
// Add your Arduino code here
// 在这里添加你的 Arduino 代码
void setup() {
  // Your setup code
}

void loop() {
  // Your loop code
}
```

### Reflections | 反思

[What did you learn about hardware, sensors, and programming?]
```

⏱️ **Expected time**: 10 minutes (预计时间：10分钟)

**💾 Commit your changes | 提交你的更改:**
```bash
git add docs/day1-projects.md
git commit -m "Add Day 1 projects documentation"
```

---

### Step 12: Create Your Project Tracking Wiki
### 步骤12：创建你的项目追踪 Wiki

**Create a new file | 创建新文件**: `docs/project-tracking.md`

```markdown
---
sidebar_position: 3
---

# Project Tracking Wiki
# 项目追踪 Wiki

This page tracks my progress through the 6-day Making More Makers course.

此页面追踪我在6天 Making More Makers 课程中的进度。

---

## 📅 Day 1: Introduction & Arduino Basics
## 📅 第1天：介绍与 Arduino 基础

**Date | 日期**: [Date]

**Status | 状态**: ✅ Complete

### What I Did | 我做了什么

- [x] Spaghetti Marshmallow Challenge
- [x] GitHub Classroom setup
- [x] Arduino Hardware CTF

### Key Learnings | 关键学习

- [Learning 1]
- [Learning 2]

---

## 📅 Day 2: Technical Blog & Advanced Arduino
## 📅 第2天：技术博客与进阶 Arduino

**Date | 日期**: [Today's date]

**Status | 状态**: 🔄 In Progress

### What I'm Doing | 我正在做什么

- [x] Building Docusaurus blog
- [ ] Advanced Arduino challenges
- [ ] [Add other activities]

### Key Learnings | 关键学习

- Building static sites with Docusaurus
- [Add more as you learn]

---

## 📅 Day 3: [Topic]
## 📅 第3天：[主题]

**Date | 日期**: [Date]

**Status | 状态**: ⏳ Not Started

### Planned Activities | 计划活动

- [ ] [Activity 1]
- [ ] [Activity 2]

---

## 📅 Day 4: [Topic]
## 📅 第4天：[主题]

**Status | 状态**: ⏳ Not Started

---

## 📅 Day 5: [Topic]
## 📅 第5天：[主题]

**Status | 状态**: ⏳ Not Started

---

## 📅 Day 6: Final Project Presentations
## 📅 第6天：最终项目展示

**Status | 状态**: ⏳ Not Started

### My Final Project Idea | 我的最终项目想法

[Describe your final project idea here - what will you build?]

---

## 🎯 Course Goals Tracker
## 🎯 课程目标追踪

- [ ] Goal 1: [Your goal]
- [ ] Goal 2: [Your goal]
- [ ] Goal 3: [Your goal]

---

## 📝 Daily Reflections
## 📝 每日反思

### Day 1 Reflection | 第1天反思

[Your thoughts about Day 1]

### Day 2 Reflection | 第2天反思

[Your thoughts about Day 2 - add this at the end of today]
```

⏱️ **Expected time**: 10 minutes (预计时间：10分钟)

**💾 Commit your changes | 提交你的更改:**
```bash
git add docs/project-tracking.md
git commit -m "Add project tracking wiki"
```

---

### Step 13: Add a Welcome Blog Post (Optional)
### 步骤13：添加欢迎博客文章（可选）

**Edit the existing file | 编辑现有文件**: `blog/[date]-welcome.md`

Or create a new blog post about starting your Maker journey!

或创建一篇关于开始你的 Maker 之旅的新博客文章！

⏱️ **Expected time**: 5 minutes (optional) (预计时间：5分钟（可选）)

**💾 Commit if you made changes | 如果做了更改就提交:**
```bash
git add blog/
git commit -m "Update welcome blog post"
```

---

### 🎉 Part 2 Complete! | 第2部分完成！

You now have:
- ✅ A complete Maker Profile (完整的 Maker 档案)
- ✅ Day 1 project documentation (第1天项目文档)
- ✅ A project tracking wiki (项目追踪 wiki)
- ✅ Content written in Markdown (用 Markdown 写的内容)
- ✅ All changes committed to Git (所有更改已提交到 Git)

**Check your browser** - you should see all these pages in your sidebar!

**查看你的浏览器** - 你应该在侧边栏看到所有这些页面！

**Check your Git history | 查看你的 Git 历史:**
```bash
git log --oneline
```

You should see all your commits! (你应该看到所有的提交！)

---

## 🚀 Part 3: Deploy to GitHub Pages (30 minutes)
## 🚀 第3部分：部署到 GitHub Pages（30分钟）

Now let's make your blog live on the internet! We'll deploy it to GitHub Pages so anyone can visit it.

现在让我们让你的博客在互联网上线！我们将它部署到 GitHub Pages，这样任何人都可以访问。

---

### Step 14: Create a GitHub Repository
### 步骤14：创建 GitHub 仓库

1. Go to https://github.com and log in (访问 https://github.com 并登录)

2. Click the **"+"** button in the top right, then **"New repository"** (点击右上角的 **"+"** 按钮，然后点击 **"New repository"**)

3. **Repository settings | 仓库设置:**
   - **Repository name | 仓库名称**: `my-maker-blog` (or any name you like)
   - **Description | 描述**: "My personal Maker blog built with Docusaurus"
   - **Public** ✅ (Make sure it's public so GitHub Pages works) (确保是公开的，这样 GitHub Pages 才能工作)
   - **DO NOT** check "Initialize with README" (不要勾选"Initialize with README")

4. Click **"Create repository"** (点击 **"Create repository"**)

⏱️ **Expected time**: 2 minutes (预计时间：2分钟)

---

### Step 15: Configure Docusaurus for GitHub Pages
### 步骤15：为 GitHub Pages 配置 Docusaurus

**Open `docusaurus.config.js`** and find these lines:

**打开 `docusaurus.config.js`** 并找到这些行：

```javascript
const config = {
  title: 'My Maker Journey',
  tagline: 'Building, Learning, Creating',
  url: 'https://your-username.github.io',
  baseUrl: '/my-maker-blog/',
  // ...
```

**Change them to YOUR information | 更改为你的信息:**

```javascript
const config = {
  title: 'My Maker Journey',  // Your blog title | 你的博客标题
  tagline: 'Building, Learning, Creating',  // Your tagline | 你的标语
  url: 'https://YOUR-GITHUB-USERNAME.github.io',  // ⭐ CHANGE THIS
  baseUrl: '/YOUR-REPOSITORY-NAME/',  // ⭐ CHANGE THIS (must start and end with /)
  
  // GitHub Pages deployment config
  organizationName: 'YOUR-GITHUB-USERNAME',  // ⭐ CHANGE THIS
  projectName: 'YOUR-REPOSITORY-NAME',  // ⭐ CHANGE THIS
  // ...
```

**Example | 例子:**

If your GitHub username is `alice` and your repository is `my-maker-blog`:

如果你的 GitHub 用户名是 `alice`，仓库是 `my-maker-blog`：

```javascript
url: 'https://alice.github.io',
baseUrl: '/my-maker-blog/',
organizationName: 'alice',
projectName: 'my-maker-blog',
```

**Important | 重要：**
- `baseUrl` must start and end with `/` (`baseUrl` 必须以 `/` 开始和结束)
- Use your actual GitHub username (使用你实际的 GitHub 用户名)
- Match the repository name exactly (准确匹配仓库名称)

⏱️ **Expected time**: 3 minutes (预计时间：3分钟)

**💾 Commit your configuration changes | 提交配置更改:**
```bash
git add docusaurus.config.js
git commit -m "Configure for GitHub Pages deployment"
```

---

### Step 16: Push to GitHub
### 步骤16：推送到 GitHub

**Stop your development server** by pressing `Ctrl+C` in the terminal where `yarn start` is running.

**停止开发服务器**，在运行 `yarn start` 的终端按 `Ctrl+C`。

Now run these commands in your terminal:

现在在终端运行这些命令：

```bash
# Add your GitHub repository as remote
# 将 GitHub 仓库添加为远程仓库
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to GitHub
# 推送到 GitHub
git branch -M main
git push -u origin main
```

**Replace `YOUR-USERNAME` and `YOUR-REPO-NAME` with your actual values!**

**将 `YOUR-USERNAME` 和 `YOUR-REPO-NAME` 替换为你的实际值！**

**Example | 例子:**
```bash
git remote add origin https://github.com/alice/my-maker-blog.git
```

💡 **Note | 注意:** 
Since we already initialized Git in Step 4 and have been committing changes throughout, we now just need to connect to GitHub and push!

因为我们已经在步骤4初始化了 Git 并一直在提交更改，现在我们只需要连接到 GitHub 并推送！

⏱️ **Expected time**: 3 minutes (预计时间：3分钟)

---

### Step 17: Deploy to GitHub Pages
### 步骤17：部署到 GitHub Pages

Now for the magic! ✨ Let's deploy your site.

现在是神奇的时刻！✨ 让我们部署你的网站。

#### Option A: Automated Deployment (Recommended)
#### 选项 A：自动部署（推荐）

**Set up GitHub Actions for automatic deployment:**

**设置 GitHub Actions 进行自动部署：**

1. Create a new file: `.github/workflows/deploy.yml`

创建新文件：`.github/workflows/deploy.yml`

```yaml
name: Deploy to GitHub Pages

on:
  push:
    branches:
      - main

permissions:
  contents: write

jobs:
  deploy:
    name: Deploy to GitHub Pages
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-node@v3
        with:
          node-version: 20
          cache: yarn

      - name: Install dependencies
        run: yarn install --frozen-lockfile
      - name: Build website
        run: yarn build

      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./build
          user_name: github-actions[bot]
          user_email: 41898282+github-actions[bot]@users.noreply.github.com
```

2. **Commit and push this file:**

**提交并推送此文件：**

```bash
git add .github/workflows/deploy.yml
git commit -m "Add GitHub Actions deployment workflow"
git push
```

3. **Enable GitHub Pages in your repository:**

**在仓库中启用 GitHub Pages：**

- Go to your repository on GitHub (访问 GitHub 上的仓库)
- Click **Settings** > **Pages** (点击 **Settings** > **Pages**)
- Under "Build and deployment" > "Source", select **"GitHub Actions"** (在"Build and deployment" > "Source"下，选择 **"GitHub Actions"**)

💡 **Important Update | 重要更新:** 
GitHub now recommends using GitHub Actions instead of deploying from a branch. This is already what we're doing! You'll see two options:
- ✅ **GitHub Actions** ← Select this! (选择这个！)
- Deploy from a branch (the old way)

GitHub 现在推荐使用 GitHub Actions 而不是从分支部署。这正是我们正在做的！你会看到两个选项：
- ✅ **GitHub Actions** ← 选择这个！
- Deploy from a branch（旧方式）

4. **Wait for deployment** (等待部署)
   - Go to the **Actions** tab (访问 **Actions** 标签)
   - Watch your deployment workflow run (观看部署工作流运行)
   - When it's green ✅, your site is live! (当它变绿 ✅，你的网站就上线了！)
   - GitHub Pages will automatically detect and deploy from Actions (GitHub Pages 会自动检测并从 Actions 部署)

#### Option B: Manual Deployment
#### 选项 B：手动部署

If you prefer to deploy manually:

如果你更喜欢手动部署：

```bash
# Build the static site
# 构建静态网站
yarn build

# Deploy to GitHub Pages
# 部署到 GitHub Pages
GIT_USER=YOUR-GITHUB-USERNAME yarn deploy
```

**On Windows PowerShell | 在 Windows PowerShell 上:**
```powershell
cmd /C "set GIT_USER=YOUR-GITHUB-USERNAME && yarn deploy"
```

⏱️ **Expected time**: 5-10 minutes (预计时间：5-10分钟)

---

### Step 18: Verify Your Deployment
### 步骤18：验证你的部署

Your blog should now be live! 🎉

你的博客现在应该上线了！🎉

**Your URL will be | 你的 URL 将是:**
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

**Example | 例子:**
```
https://alice.github.io/my-maker-blog/
```

**Open this URL in your browser and check:**

**在浏览器中打开此 URL 并检查：**

- [ ] The site loads successfully (网站成功加载)
- [ ] You can see your Maker Profile page (可以看到 Maker 档案页面)
- [ ] You can see your Day 1 Projects page (可以看到第1天项目页面)
- [ ] You can see your Project Tracking page (可以看到项目追踪页面)
- [ ] All links and navigation work (所有链接和导航都正常工作)

⏱️ **Expected time**: 2 minutes (预计时间：2分钟)

---

### Step 19: Take Your Screenshot
### 步骤19：截图

**For submission, take a full-page screenshot that shows:**

**用于提交，截取显示以下内容的全页截图：**

1. **The URL bar** with your GitHub Pages URL visible (URL 栏显示你的 GitHub Pages URL)
2. **Your blog homepage** (你的博客首页)
3. **Navigation menu** showing your pages (导航菜单显示你的页面)

**How to take a screenshot | 如何截图:**

- **Windows**: Press `Windows + Shift + S`, then select area (按 `Windows + Shift + S`，然后选择区域)
- **Mac**: Press `Command + Shift + 4`, then select area (按 `Command + Shift + 4`，然后选择区域)
- **Linux**: Press `PrtScn` or use Screenshot tool (按 `PrtScn` 或使用截图工具)

**Save your screenshot** as `blog-screenshot.png`

**保存截图**为 `blog-screenshot.png`

⏱️ **Expected time**: 2 minutes (预计时间：2分钟)

---

### 🎉 Part 3 Complete! | 第3部分完成！

You now have:
- ✅ A GitHub repository with your code (包含代码的 GitHub 仓库)
- ✅ Your blog deployed to GitHub Pages (部署到 GitHub Pages 的博客)
- ✅ A live URL anyone can visit (任何人都可以访问的在线 URL)
- ✅ A screenshot for submission (用于提交的截图)

---

## 📤 Submission Instructions | 提交说明

**You're ready to submit! Follow these steps:**

**你准备好提交了！按照以下步骤操作：**

### Option 1: Submit via GitHub Classroom (Recommended) | 选项1：通过 GitHub Classroom 提交（推荐）

1. **Edit `submission.json`** in this repository (在此仓库中编辑 `submission.json`)
   - Add your GitHub Pages URL (添加你的 GitHub Pages URL)
   - Add your screenshot filename (添加截图文件名)

2. **Upload your screenshot** to this repository (上传截图到此仓库)
   - File name: `blog-screenshot.png` or `blog-screenshot.jpg`

3. **Commit and push** both files (提交并推送两个文件)

4. **AI will auto-grade** your submission within 2-3 minutes! (AI 将在 2-3 分钟内自动评分！)
   - Check the **Issues** tab for feedback (查看 **Issues** 标签获取反馈)

**See [HOW-TO-SUBMIT.md](./HOW-TO-SUBMIT.md) for step-by-step instructions.**

**逐步说明见 [HOW-TO-SUBMIT.md](./HOW-TO-SUBMIT.md)。**

### Option 2: Manual Submission (if instructor specifies) | 选项2：手动提交（如果讲师指定）

**See [SUBMISSION.md](./SUBMISSION.md) for alternative submission methods.**

**其他提交方法见 [SUBMISSION.md](./SUBMISSION.md)。**

---

## 🆘 Troubleshooting | 故障排除

### Common Issues | 常见问题

<details>
<summary><strong>Q: My site shows a 404 error on GitHub Pages | 我的网站在 GitHub Pages 上显示 404 错误</strong></summary>

**Solutions | 解决方案:**

1. Check that your `baseUrl` in `docusaurus.config.js` matches your repository name (检查 `docusaurus.config.js` 中的 `baseUrl` 是否与仓库名称匹配)
2. Make sure `baseUrl` starts and ends with `/` (确保 `baseUrl` 以 `/` 开始和结束)
3. Verify you selected the `gh-pages` branch in Settings > Pages (验证你在 Settings > Pages 中选择了 `gh-pages` 分支)
4. Wait 2-3 minutes for deployment to complete (等待 2-3 分钟部署完成)
</details>

<details>
<summary><strong>Q: `yarn install` is taking forever | `yarn install` 花费很长时间</strong></summary>

**Solutions | 解决方案:**

1. Check your internet connection (检查互联网连接)
2. Try using a different network (尝试使用不同的网络)
3. Clear yarn cache: `yarn cache clean` (清除 yarn 缓存)
4. Try using a different registry: `yarn config set registry https://registry.npmmirror.com` (尝试使用不同的镜像源)
</details>

<details>
<summary><strong>Q: Port 3000 is already in use | 端口 3000 已被占用</strong></summary>

**Solution | 解决方案:**

Run on a different port (在不同端口上运行):
```bash
yarn start --port 3001
```
</details>

<details>
<summary><strong>Q: Git push is asking for authentication | Git push 要求身份验证</strong></summary>

**Solution | 解决方案:**

You need to set up authentication. Use one of these methods:

你需要设置身份验证。使用以下方法之一：

1. **Personal Access Token** (recommended) (推荐):
   - Go to GitHub Settings > Developer settings > Personal access tokens (访问 GitHub Settings > Developer settings > Personal access tokens)
   - Generate new token with `repo` scope (生成具有 `repo` 范围的新令牌)
   - Use the token as your password (使用令牌作为密码)

2. **SSH Key** (more secure):
   - See: https://docs.github.com/en/authentication/connecting-to-github-with-ssh
</details>

<details>
<summary><strong>Q: I made changes but they're not showing on my deployed site | 我做了更改但部署的网站上没有显示</strong></summary>

**Solution | 解决方案:**

After making changes, you need to:

更改后，你需要：

```bash
# Commit your changes
git add .
git commit -m "Update content"

# Push to GitHub
git push

# If using Option B (manual), redeploy:
yarn deploy
```

Wait 2-3 minutes for GitHub Pages to update (等待 2-3 分钟 GitHub Pages 更新)
</details>

---

## ✅ Completion Checklist | 完成检查清单

Before submitting, make sure:

提交前，确保：

- [ ] Node.js is installed and working (Node.js 已安装且工作正常)
- [ ] Docusaurus project is created (Docusaurus 项目已创建)
- [ ] Development server runs locally (开发服务器在本地运行)
- [ ] Maker Profile page is complete (Maker 档案页面已完成)
- [ ] Day 1 Projects page is complete (第1天项目页面已完成)
- [ ] Project Tracking page is complete (项目追踪页面已完成)
- [ ] GitHub repository is created (GitHub 仓库已创建)
- [ ] Code is pushed to GitHub (代码已推送到 GitHub)
- [ ] Site is deployed to GitHub Pages (网站已部署到 GitHub Pages)
- [ ] GitHub Pages URL works and shows your content (GitHub Pages URL 正常工作并显示内容)
- [ ] Screenshot is taken showing the deployed site (已截图显示部署的网站)
- [ ] Both URL and screenshot are submitted (URL 和截图都已提交)

---

## 📚 Resources | 资源

### Documentation | 文档
- 📖 [Docusaurus Official Docs](https://docusaurus.io/docs) - Complete documentation (完整文档)
- 📝 [Markdown Guide](https://www.markdownguide.org/) - Learn Markdown syntax (学习 Markdown 语法)
- 🐙 [GitHub Pages Docs](https://docs.github.com/en/pages) - GitHub Pages guide (GitHub Pages 指南)
- 💡 [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics) - Learn Git (学习 Git)

### Help | 帮助
- 💬 Ask your instructor or TAs during class (课堂上询问讲师或助教)
- 🤝 Work with classmates - collaboration is encouraged! (与同学合作 - 鼓励协作！)
- 🔍 Search online - Stack Overflow, GitHub Discussions (在线搜索 - Stack Overflow, GitHub Discussions)

---

## 🌟 Tips for Success | 成功提示

1. **Follow the steps in order** (按顺序执行步骤)
   - Don't skip ahead (不要跳过)
   - Complete each step before moving on (完成每一步后再继续)

2. **Save often** (经常保存)
   - Save files after every edit (每次编辑后保存文件)
   - Commit to Git regularly (定期提交到 Git)

3. **Test frequently** (频繁测试)
   - Check your local site often (经常检查本地网站)
   - Verify links and navigation work (验证链接和导航正常工作)

4. **Read error messages** (阅读错误消息)
   - Error messages usually tell you what's wrong (错误消息通常告诉你出了什么问题)
   - Copy error messages when asking for help (寻求帮助时复制错误消息)

5. **Personalize your blog** (个性化你的博客)
   - Make it yours! (让它成为你的！)
   - Add your own style and content (添加你自己的风格和内容)
   - This is your portfolio - make it shine! (这是你的作品集 - 让它闪耀！)

---

## 🎉 What's Next? | 接下来做什么？

After completing this assignment:

完成此作业后：

- **Keep your blog updated** throughout the course (在整个课程期间保持博客更新)
- **Add new projects** as you build them (添加你构建的新项目)
- **Share your blog URL** with friends and on social media (与朋友和社交媒体分享你的博客 URL)
- **Continue learning** - add more features to your blog! (继续学习 - 为博客添加更多功能！)

**This blog is yours forever. Keep building!** 🚀

**这个博客永远是你的。继续创造！** 🚀

---

## 📄 Grading | 评分

See **[rubric.md](./rubric.md)** for detailed grading criteria.

详细评分标准见 **[rubric.md](./rubric.md)**。

---

**Happy Building! 🎨🔧💡**

**祝你创作愉快！🎨🔧💡**

---

*If you have any questions, don't hesitate to ask. We're here to help you succeed!*

*如果你有任何问题，请随时提问。我们在这里帮助你成功！*


