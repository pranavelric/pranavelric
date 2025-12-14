# Contributing to This GitHub Profile

Thank you for your interest in improving this GitHub profile! This document provides guidelines for contributing.

## 🌟 Ways to Contribute

- 🐛 Report bugs or issues
- 💡 Suggest new features or improvements
- 📝 Improve documentation
- 🎨 Enhance design and layout
- ⚡ Optimize workflows and automation
- 🔧 Fix bugs or issues

## 🚀 Getting Started

### Prerequisites

- Git installed on your machine
- GitHub account
- Basic knowledge of Markdown
- Familiarity with GitHub Actions (for workflow changes)

### Setup

1. **Fork the repository**
   ```bash
   # Click the "Fork" button on GitHub
   ```

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/pranavelric.git
   cd pranavelric
   ```

3. **Create a branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/your-bug-fix
   ```

## 📝 Making Changes

### README Updates

When updating `README.md`:

1. **Maintain structure**: Keep existing sections organized
2. **Test rendering**: Preview Markdown before committing
3. **Check links**: Ensure all URLs work correctly
4. **Optimize images**: Use appropriate sizes and formats
5. **Accessibility**: Add descriptive alt text to images

### Workflow Changes

When modifying workflows in `.github/workflows/`:

1. **Validate YAML**: Ensure syntax is correct
   ```bash
   python3 -c "import yaml; yaml.safe_load(open('.github/workflows/your-file.yml'))"
   ```

2. **Test locally**: Use [act](https://github.com/nektos/act) to test Actions locally
   ```bash
   act -l  # List workflows
   act -j job-name  # Run specific job
   ```

3. **Consider rate limits**: Avoid overly frequent schedules
4. **Add comments**: Explain complex workflow logic
5. **Update docs**: Reflect changes in WORKFLOW_DOCUMENTATION.md

### Adding New Features

1. **Check existing issues**: Avoid duplicate work
2. **Discuss first**: Open an issue for major changes
3. **Keep it focused**: One feature per PR
4. **Follow style**: Match existing code/content style
5. **Document**: Update relevant documentation

## ✅ Checklist Before Submitting

- [ ] Code/content follows existing style
- [ ] All links are working
- [ ] Images have descriptive alt text
- [ ] YAML files are valid (for workflow changes)
- [ ] Documentation is updated
- [ ] Changes are tested
- [ ] Commit messages are clear and descriptive
- [ ] Branch is up to date with main

## 📤 Submitting Changes

1. **Commit your changes**
   ```bash
   git add .
   git commit -m "feat: Add feature description"
   # or
   git commit -m "fix: Fix bug description"
   ```

2. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

3. **Create Pull Request**
   - Go to the original repository
   - Click "New Pull Request"
   - Select your fork and branch
   - Fill in PR template with details
   - Submit for review

## 📋 Commit Message Guidelines

Follow [Conventional Commits](https://www.conventionalcommits.org/):

- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `style:` Code style changes (formatting, etc.)
- `refactor:` Code refactoring
- `perf:` Performance improvements
- `test:` Adding or updating tests
- `chore:` Maintenance tasks

**Examples:**
```
feat: Add new technology icons section
fix: Correct broken DevCard link
docs: Update workflow documentation
style: Improve README formatting
refactor: Reorganize assets directory
```

## 🎨 Style Guide

### Markdown

- Use ATX-style headers (`#` not `===`)
- One blank line before and after headers
- Use relative links for internal files
- Prefer reference-style links for readability
- Use code blocks with language specification

### Images

- Descriptive alt text for accessibility
- Appropriate sizes (not too large)
- Organized in `/images/` directory
- Use SVG when possible for scalability

### Workflows

- Clear, descriptive job names
- Comments for complex logic
- Consistent indentation (2 spaces)
- Secure secret handling
- Minimal API calls to avoid rate limits

## 🔒 Security

- **Never commit secrets**: Use GitHub Secrets
- **Validate inputs**: Sanitize user inputs in workflows
- **Secure tokens**: Minimal required permissions
- **Review dependencies**: Check action versions
- **Report vulnerabilities**: Use private security advisories

## 🧪 Testing

### Testing README Changes

1. **Preview locally**: Use VS Code or another Markdown viewer
2. **Check rendering**: Push to your fork and view on GitHub
3. **Test links**: Click all links to verify they work
4. **Mobile view**: Check how it looks on mobile devices

### Testing Workflow Changes

1. **Syntax validation**: Validate YAML syntax
2. **Manual trigger**: Test with workflow_dispatch
3. **Check outputs**: Verify generated files are correct
4. **Monitor logs**: Review action logs for errors
5. **Rate limits**: Ensure you're not hitting API limits

## 📖 Documentation

When adding features, update:

- `README.md` - If it affects the main profile
- `WORKFLOW_DOCUMENTATION.md` - For workflow changes
- `QUICK_START.md` - For setup/usage changes
- `CONTRIBUTING.md` - For contribution process changes

## 🐛 Reporting Bugs

When reporting bugs, include:

1. **Description**: Clear description of the issue
2. **Steps to reproduce**: How to recreate the bug
3. **Expected behavior**: What should happen
4. **Actual behavior**: What actually happens
5. **Screenshots**: If applicable
6. **Environment**: Browser, OS, etc.
7. **Logs**: Relevant error messages or logs

**Bug Report Template:**
```markdown
## Bug Description
A clear and concise description of the bug.

## Steps to Reproduce
1. Go to '...'
2. Click on '...'
3. See error

## Expected Behavior
What should happen.

## Actual Behavior
What actually happens.

## Screenshots
If applicable, add screenshots.

## Environment
- Browser: [e.g., Chrome 96]
- OS: [e.g., Windows 11]
- Device: [e.g., Desktop]

## Additional Context
Any other relevant information.
```

## 💡 Feature Requests

When suggesting features, include:

1. **Problem statement**: What problem does this solve?
2. **Proposed solution**: How would you implement it?
3. **Alternatives**: Other approaches considered?
4. **Examples**: Similar implementations elsewhere?
5. **Impact**: Who benefits and how?

**Feature Request Template:**
```markdown
## Feature Description
A clear description of the feature.

## Problem Statement
What problem does this solve?

## Proposed Solution
How would you implement this?

## Alternatives Considered
Other approaches you've thought about.

## Additional Context
Any other relevant information.

## Examples
Links to similar implementations.
```

## 🤝 Code of Conduct

- **Be respectful**: Treat others with respect
- **Be collaborative**: Work together constructively
- **Be patient**: Everyone learns at their own pace
- **Be inclusive**: Welcome diverse perspectives
- **Be professional**: Maintain professional standards

## 📞 Getting Help

Need help contributing?

- 💬 [GitHub Discussions](https://github.com/pranavelric/pranavelric/discussions)
- 📧 Email: pranavchoudhary500@gmail.com
- 🐛 [Open an Issue](https://github.com/pranavelric/pranavelric/issues)

## 🎉 Recognition

Contributors will be:

- Listed in repository contributors
- Mentioned in release notes (for significant contributions)
- Acknowledged in documentation updates

## 📜 License

By contributing, you agree that your contributions will be licensed under the MIT License.

---

Thank you for contributing! 🚀

**Happy Contributing!**

Made with ❤️ by the community
