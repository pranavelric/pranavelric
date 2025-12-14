# Quick Start Guide - GitHub Profile Optimization

This is a quick reference for managing your optimized GitHub profile.

## 🚀 Features

✅ **Automated Updates**: All profile elements update automatically  
✅ **SEO Optimized**: Descriptive alt text and semantic HTML  
✅ **Accessible**: WCAG compliant with proper ARIA labels  
✅ **Rate Limit Friendly**: Optimized schedules to avoid API limits  
✅ **Modern Design**: Clean, professional, recruiter-friendly layout  

## 📁 Directory Structure

```
pranavelric/
├── .github/
│   ├── workflows/          # GitHub Actions automation
│   │   ├── metrics.yml     # Daily metrics update
│   │   ├── snake.yml       # Weekly snake animation
│   │   ├── Devcard.yml     # Weekly DevCard update
│   │   ├── profile-3d.yml  # Weekly 3D profile
│   │   └── fork_start.yml  # Star/fork counter
│   ├── dependabot.yml      # Dependency updates
│   └── FUNDING.yml         # GitHub Sponsors config
├── images/                 # All generated assets
│   ├── devcard.svg
│   ├── github-metrics.svg
│   ├── github-contribution-grid-snake.svg
│   ├── github-contribution-grid-snake-dark.svg
│   ├── profile-3d-contrib/ # 3D visualizations
│   ├── gif/                # Animated GIFs
│   └── webp/               # WebP images
├── README.md               # Main profile page
├── LICENSE                 # MIT License
├── .gitignore              # Git ignore rules
├── WORKFLOW_DOCUMENTATION.md  # Detailed workflow docs
└── QUICK_START.md          # This file
```

## ⚙️ Required Setup

### 1. GitHub Secrets

Add these in **Settings → Secrets → Actions**:

- `METRICS_TOKEN`: [Create Personal Access Token](https://github.com/settings/tokens/new)
  - Required scopes: `repo`, `read:org`, `read:user`, `read:packages`
  
- `DEVCARD_ID`: Get from [Daily.dev](https://app.daily.dev/devcard)

- `PAGESPEED_TOKEN`: (Optional) Get from [Google Cloud Console](https://console.cloud.google.com/)

### 2. Enable GitHub Actions

1. Go to **Settings → Actions → General**
2. Set "Workflow permissions" to **Read and write permissions**
3. Check **Allow GitHub Actions to create and approve pull requests**

### 3. Enable GitHub Pages (Optional)

If you have a portfolio website in another repo:
1. Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main` / `gh-pages`

## 🎯 Quick Actions

### Manually Trigger Workflows

```bash
# Go to Actions tab → Select workflow → Run workflow
```

Or use GitHub CLI:

```bash
# Install GitHub CLI: https://cli.github.com/
gh workflow run metrics.yml
gh workflow run snake.yml
gh workflow run Devcard.yml
gh workflow run profile-3d.yml
```

### Update Profile Content

Edit `README.md` and commit:

```bash
git add README.md
git commit -m "Update profile content"
git push
```

### Add New Technology Icons

Use [Skill Icons](https://skillicons.dev/) or [Shields.io](https://shields.io/):

```markdown
![Tech](https://skillicons.dev/icons?i=python,js,react)
![Badge](https://img.shields.io/badge/Tech-Name-color)
```

## 📊 Workflow Schedule

| Time (UTC) | Workflow | Frequency |
|------------|----------|-----------|
| 00:00 Daily | Metrics | Every day |
| 00:00 Sunday | Snake | Weekly |
| 01:00 Sunday | DevCard | Weekly |
| 02:00 Sunday | 3D Profile | Weekly |
| 03:00 Sunday | Star Counter | Weekly |

## 🔧 Customization

### Change Update Frequency

Edit the cron expression in workflow files:

```yaml
schedule:
  - cron: "0 0 * * 0"  # Weekly on Sunday
  - cron: "0 0 * * *"  # Daily
  - cron: "0 */12 * * *"  # Every 12 hours
```

Use [crontab.guru](https://crontab.guru/) to build cron expressions.

### Modify README Sections

The README is organized into sections:

1. **Header** - Banner and social links
2. **About** - Personal info and DevCard
3. **Statistics** - GitHub stats and achievements
4. **Technologies** - Skills and tools
5. **Activity** - Contribution graphs
6. **Humor** - Random jokes
7. **Visualizations** - 3D graph and snake
8. **Metrics** - Comprehensive metrics
9. **Connect** - Social links and automation diagram
10. **Footer** - Credits and badges

### Change Color Scheme

Update these values in README badges and widgets:

- Primary: `#00DCA8` (teal)
- Secondary: `#00ab75` (green)
- Background: `#0D1117` (dark)
- Text: `#FDFCFF` (light)

## 🐛 Troubleshooting

### Images Not Loading

1. Check file paths match: `./images/filename.svg`
2. Verify workflows completed successfully
3. Clear browser cache (Ctrl+F5)
4. Check repository permissions

### Workflow Failures

1. **Check Action logs**: Actions tab → Failed run → View logs
2. **Verify secrets**: Settings → Secrets → Actions
3. **Check token permissions**: Token needs correct scopes
4. **API rate limits**: Wait for reset or optimize schedules

### Metrics Not Updating

1. Manually trigger workflow: Actions → Metrics → Run workflow
2. Check `METRICS_TOKEN` is valid and not expired
3. Verify token has required permissions
4. Check for API rate limit issues

## 📈 SEO & Visibility Tips

1. **Use keywords**: Include relevant technologies in README
2. **Alt text**: All images have descriptive alt text
3. **Links**: Add portfolio, blog, and social links
4. **Topics**: Add repository topics (Settings → Topics)
5. **Description**: Update repo description with keywords
6. **Pin repos**: Pin best projects to profile

## 🎨 Design Best Practices

- ✅ Consistent color scheme throughout
- ✅ Responsive images with proper sizing
- ✅ Semantic HTML and proper headings
- ✅ Accessible with descriptive alt text
- ✅ Fast loading with optimized images
- ✅ Professional and clean layout

## 🔗 Useful Links

- [GitHub Profile README Guide](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
- [Awesome GitHub Profile READMEs](https://github.com/abhisheknaiidu/awesome-github-profile-readme)
- [Shields.io Badges](https://shields.io/)
- [Skill Icons](https://skillicons.dev/)
- [GitHub Stats](https://github.com/anuraghazra/github-readme-stats)
- [Metrics Action Docs](https://github.com/lowlighter/metrics)

## 💡 Pro Tips

1. **Regular updates**: Keep README current with latest projects
2. **Engage community**: Star, fork, and contribute to projects
3. **Quality over quantity**: Focus on meaningful contributions
4. **Document projects**: Good READMEs increase visibility
5. **Network**: Connect with developers in your field
6. **Stay active**: Regular commits show consistency

## 📞 Support

Need help? Check these resources:

- 📖 [Workflow Documentation](./WORKFLOW_DOCUMENTATION.md)
- 🐛 [GitHub Issues](https://github.com/pranavelric/pranavelric/issues)
- 💬 [GitHub Discussions](https://github.com/pranavelric/pranavelric/discussions)
- 📧 Email: pranavchoudhary500@gmail.com

---

**Happy Coding! 🚀**

Made with ❤️ by [Pranav Choudhary](https://github.com/pranavelric)
