# How to Submit Your Blog Assignment
# 如何提交你的博客作业

## Quick Start | 快速开始

Follow these 3 simple steps to submit:

按照这3个简单步骤提交：

### Step 1: Edit `submission.json`
### 步骤1：编辑 `submission.json`

Open the `submission.json` file in this repository and update it with your information:

在此仓库中打开 `submission.json` 文件并更新你的信息：

```json
{
  "github_pages_url": "https://your-username.github.io/your-repo-name/",
  "screenshot_filename": "blog-screenshot.png",
  "notes": "Optional: Add any notes about your submission"
}
```

**Replace | 替换:**
- `your-username` with your actual GitHub username (用你的实际 GitHub 用户名)
- `your-repo-name` with your blog repository name (用你的博客仓库名称)

**Example | 示例:**
```json
{
  "github_pages_url": "https://alice.github.io/my-maker-blog/",
  "screenshot_filename": "blog-screenshot.png",
  "notes": "My first Docusaurus blog! Excited to share my Maker journey."
}
```

---

### Step 2: Add Your Screenshot
### 步骤2：添加你的截图

1. Take a screenshot of your deployed blog (截取部署博客的截图)
2. Save it as `blog-screenshot.png` or `blog-screenshot.jpg` (保存为 `blog-screenshot.png` 或 `blog-screenshot.jpg`)
3. Add the file to this repository (将文件添加到此仓库)

**Screenshot Requirements | 截图要求:**
- ✅ Shows URL bar with your GitHub Pages URL (显示带有 GitHub Pages URL 的 URL 栏)
- ✅ Shows your blog homepage content (显示博客首页内容)
- ✅ Clear and readable (清晰可读)
- ✅ File size under 5 MB (文件大小小于 5 MB)

---

### Step 3: Commit and Push
### 步骤3：提交并推送

Commit both files and push to GitHub:

提交两个文件并推送到 GitHub：

```bash
# Add both files
git add submission.json blog-screenshot.png

# Commit with a message
git commit -m "Submit Day 2 blog assignment"

# Push to GitHub
git push origin main
```

**That's it! The AI will automatically grade your submission within 2-3 minutes.**

**就是这样！AI 将在 2-3 分钟内自动评分你的提交。**

---

## What Happens Next? | 接下来会发生什么？

1. **GitHub Actions runs** (GitHub Actions 运行)
   - Automatically triggered when you push (推送时自动触发)
   
2. **AI checks your submission** (AI 检查你的提交)
   - Validates your GitHub Pages URL (验证 GitHub Pages URL)
   - Checks if your blog is accessible (检查博客是否可访问)
   - Verifies screenshot submission (验证截图提交)
   
3. **Feedback is posted** (反馈发布)
   - Check the **Issues** tab for AI feedback (查看 **Issues** 标签获取 AI 反馈)
   - Feedback appears within 2-3 minutes (反馈在 2-3 分钟内出现)

---

## Checking Your Submission | 检查你的提交

### See AI Grading Status | 查看 AI 评分状态

1. Go to the **Actions** tab in your repository (访问仓库的 **Actions** 标签)
2. Click on the latest workflow run (点击最新的工作流运行)
3. Watch the grading process (观看评分过程)

### Read AI Feedback | 阅读 AI 反馈

1. Go to the **Issues** tab (访问 **Issues** 标签)
2. Look for "📝 AI Grading Feedback | AI评分反馈" (查找"📝 AI Grading Feedback | AI评分反馈")
3. Read the feedback and scoring (阅读反馈和评分)

---

## Resubmission | 重新提交

**Need to fix something? No problem!**

**需要修复某些内容？没问题！**

1. Make your changes (进行更改)
2. Update `submission.json` if needed (如需要更新 `submission.json`)
3. Replace screenshot if needed (如需要替换截图)
4. Commit and push again (再次提交并推送)

The AI will automatically re-grade your updated submission!

AI 将自动重新评分你的更新提交！

---

## Troubleshooting | 故障排除

### ❌ "URL is not accessible"

**Problem**: Your blog URL returns an error

**问题**: 你的博客 URL 返回错误

**Solutions | 解决方案:**
1. Wait 5 minutes - GitHub Pages deployment takes time (等待 5 分钟 - GitHub Pages 部署需要时间)
2. Check GitHub Pages settings: Settings > Pages (检查 GitHub Pages 设置：Settings > Pages)
3. Verify `docusaurus.config.js` has correct `url` and `baseUrl` (验证 `docusaurus.config.js` 有正确的 `url` 和 `baseUrl`)
4. Make sure repository is public (确保仓库是公开的)

### ❌ "Invalid GitHub Pages URL"

**Problem**: URL format is incorrect

**问题**: URL 格式不正确

**Solutions | 解决方案:**
1. URL must start with `https://` (URL 必须以 `https://` 开头)
2. URL must contain `github.io` (URL 必须包含 `github.io`)
3. Don't submit `localhost` URLs (不要提交 `localhost` URL)
4. Format: `https://username.github.io/repo-name/` (格式：`https://username.github.io/repo-name/`)

### ❌ "Screenshot not found"

**Problem**: Screenshot file is missing

**问题**: 截图文件缺失

**Solutions | 解决方案:**
1. Make sure filename matches `submission.json` (确保文件名与 `submission.json` 匹配)
2. Filename should be `blog-screenshot.png` or `blog-screenshot.jpg` (文件名应为 `blog-screenshot.png` 或 `blog-screenshot.jpg`)
3. File must be in repository root directory (文件必须在仓库根目录)
4. Check that you committed and pushed the file (检查是否提交并推送了文件)

### ❌ "AI Grading Error"

**Problem**: AI grading failed

**问题**: AI 评分失败

**Solutions | 解决方案:**
1. Check if GitHub Actions ran successfully (检查 GitHub Actions 是否成功运行)
2. Review the Actions logs for detailed error messages (查看 Actions 日志了解详细错误消息)
3. Contact your instructor if error persists (如果错误持续，请联系讲师)

---

## Advanced: Using GitHub Web Interface | 高级：使用 GitHub Web 界面

**Don't have Git command line? You can submit via GitHub website:**

**没有 Git 命令行？你可以通过 GitHub 网站提交：**

### Step 1: Edit submission.json online

1. Click `submission.json` in your repository (点击仓库中的 `submission.json`)
2. Click the pencil icon ✏️ to edit (点击铅笔图标 ✏️ 编辑)
3. Update your URL and screenshot filename (更新 URL 和截图文件名)
4. Click "Commit changes" (点击"Commit changes")

### Step 2: Upload screenshot

1. Click "Add file" > "Upload files" (点击"Add file" > "Upload files")
2. Drag your screenshot or click "choose your files" (拖动截图或点击"choose your files")
3. Wait for upload to complete (等待上传完成)
4. Click "Commit changes" (点击"Commit changes")

**Done! AI grading will start automatically.**

**完成！AI 评分将自动开始。**

---

## Getting Help | 获取帮助

**Need assistance? | 需要帮助？**

- 📖 Check [README.md](./README.md) for full tutorial (查看完整教程)
- 📋 Review [SUBMISSION.md](./SUBMISSION.md) for detailed requirements (查看详细要求)
- 📊 Read [rubric.md](./rubric.md) for grading criteria (查看评分标准)
- 👨‍🏫 Ask your instructor or TAs (询问讲师或助教)
- 💬 Post in the course discussion forum (在课程讨论论坛发帖)

---

## Submission Checklist | 提交检查清单

Before pushing, verify:

推送前，验证：

- [ ] `submission.json` has your correct GitHub Pages URL (有你正确的 GitHub Pages URL)
- [ ] URL format is `https://username.github.io/repo-name/` (URL 格式正确)
- [ ] Your blog is deployed and accessible (博客已部署且可访问)
- [ ] Screenshot file is added to repository (截图文件已添加到仓库)
- [ ] Screenshot filename matches `submission.json` (截图文件名与 `submission.json` 匹配)
- [ ] Screenshot shows URL bar and blog content (截图显示 URL 栏和博客内容)
- [ ] Both files are committed and pushed (两个文件都已提交并推送)

---

**Good luck! We're excited to see your Maker blogs! 🚀**

**祝你好运！我们很期待看到你的 Maker 博客！🚀**


