# Contributing Guide

Thank you for your interest in contributing to the Sociocultural Project Development Environment! We welcome contributions from everyone, regardless of experience level.

## 🌟 Ways to Contribute

There are many ways to contribute to this project:

- **Code**: Help implement features, fix bugs, or improve performance
- **Documentation**: Improve docs, write tutorials, or translate to other languages
- **Design**: Create UI mockups, icons, or improve user experience
- **Testing**: Report bugs, test new features, or write test cases
- **Feedback**: Share your experience and suggestions
- **Community**: Help others, answer questions, or organize events

## 📋 Getting Started

### 1. Understand the Project

Before contributing, please familiarize yourself with:

- [README](README.md) - Project overview
- [Workflow Design](docs/WORKFLOW_DESIGN.md) - Detailed workflow specification
- [Implementation Guide](docs/IMPLEMENTATION_GUIDE.md) - Technical details

### 2. Find Something to Work On

Check out our:
- [GitHub Issues](https://github.com/johanneskueng/community_based_project_dev/issues) - Bug reports and feature requests
- [GitHub Discussions](https://github.com/johanneskueng/community_based_project_dev/discussions) - Ideas and questions
- [Project Board](https://github.com/johanneskueng/community_based_project_dev/projects) - Roadmap and priorities

Look for issues labeled:
- `good first issue` - Great for beginners
- `help wanted` - Needs assistance
- `bug` - Bug fixes needed
- `enhancement` - Feature improvements
- `documentation` - Documentation tasks

### 3. Set Up Your Development Environment

See the [Development Setup](README.md#-development-setup) section in the README.

## 🍴 Forking and Creating Pull Requests

### 1. Fork the Repository

Click the "Fork" button at the top right of the repository page to create your own copy.

### 2. Clone Your Fork

```bash
git clone https://github.com/your-username/community_based_project_dev.git
cd community_based_project_dev
```

### 3. Set Up Upstream Remote

```bash
git remote add upstream https://github.com/johanneskueng/community_based_project_dev.git
```

### 4. Create a Branch

Always work on a new branch, not on `main`:

```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/your-bug-fix
# or
git checkout -b docs/your-documentation-update
```

Branch naming conventions:
- `feature/` - New features
- `fix/` - Bug fixes
- `docs/` - Documentation updates
- `refactor/` - Code refactoring
- `chore/` - Maintenance tasks

### 5. Make Your Changes

- Follow the [Coding Standards](#-coding-standards) below
- Write tests for your changes (if applicable)
- Update documentation (if applicable)

### 6. Commit Your Changes

Write clear, descriptive commit messages:

```bash
git commit -m "feat: add data clustering functionality"
git commit -m "fix: resolve offline sync conflict issue"
git commit -m "docs: update workflow design documentation"
```

Commit message format:
- Use the present tense ("Add feature" not "Added feature")
- Limit first line to 72 characters
- Use imperative mood
- Reference issue numbers (e.g., "Closes #123")

### 7. Push to Your Fork

```bash
git push origin feature/your-feature-name
```

### 8. Create a Pull Request

1. Go to the [original repository](https://github.com/johanneskueng/community_based_project_dev)
2. Click "New Pull Request"
3. Select your fork and branch
4. Fill out the PR template
5. Submit the pull request

### 9. Respond to Feedback

Maintainers may request changes. Please:
- Respond promptly to feedback
- Make requested changes in new commits
- Push the changes to the same branch
- The PR will update automatically

## 📝 Pull Request Template

When creating a pull request, please use this template:

```markdown
## Description

[Brief description of the changes]

## Related Issues

[Link to any related issues, e.g., Closes #123]

## Changes Made

- [ ] Feature implementation
- [ ] Bug fix
- [ ] Documentation update
- [ ] Test coverage
- [ ] Performance improvement
- [ ] Security fix
- [ ] Other (please specify)

## Testing

[Describe how you tested your changes]

- [ ] Unit tests pass
- [ ] Integration tests pass
- [ ] Manual testing completed
- [ ] Accessibility testing completed
- [ ] Offline functionality tested

## Screenshots (if applicable)

[Add screenshots or GIFs showing the changes]

## Checklist

- [ ] I have read the [Contributing Guide](CONTRIBUTING.md)
- [ ] I have followed the [Coding Standards](#-coding-standards)
- [ ] My changes are properly tested
- [ ] I have updated documentation (if needed)
- [ ] My commits have descriptive messages
- [ ] I have signed my commits (DCO)

## Additional Notes

[Any additional information]
```

## 🎨 Coding Standards

### General

- Use consistent indentation (2 or 4 spaces, no tabs)
- Keep lines under 100 characters when possible
- Use meaningful variable and function names
- Comment complex logic, not obvious code
- Remove commented-out code before committing
- Avoid console.log statements in production code

### JavaScript/TypeScript

- Use ES6+ features
- Prefer `const` over `let` when possible
- Use arrow functions for callbacks
- Use template literals for strings
- Use destructuring for objects and arrays
- Follow the [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript) as a reference

### Vue.js (if using Vue)

- Use Composition API for new components
- Use `<script setup>` syntax
- Keep components focused and small
- Use props for component communication
- Use emits for parent-child communication
- Use Pinia for state management

### CSS

- Use BEM (Block Element Modifier) methodology
- Keep styles scoped to components
- Use CSS variables for colors and common values
- Avoid `!important`
- Use flexbox/grid for layout
- Ensure sufficient color contrast

### HTML

- Use semantic HTML5 elements
- Ensure proper accessibility attributes
- Use valid HTML
- Keep markup clean and readable

### Accessibility

- Always include alt text for images
- Use semantic HTML elements
- Ensure keyboard navigation works
- Use ARIA attributes when needed
- Test with screen readers
- Follow WCAG 2.1 AA guidelines

## 🧪 Testing

### Unit Tests

- Write tests for new features
- Test edge cases
- Aim for 80%+ code coverage
- Use descriptive test names

### Integration Tests

- Test component interactions
- Test data flows
- Test API integrations

### End-to-End Tests

- Test complete user journeys
- Test on multiple browsers/devices
- Test offline functionality

### Accessibility Tests

- Run automated tests with axe-core
- Manual testing with screen readers
- Keyboard-only navigation testing
- Color contrast testing

## 📚 Documentation

### Code Documentation

- Use JSDoc for functions
- Document complex logic
- Document API endpoints
- Document component props and events

### User Documentation

- Keep user guides up to date
- Use clear, simple language
- Include screenshots and examples
- Document all features

### Technical Documentation

- Document architecture decisions
- Document database schema
- Document API contracts
- Document deployment processes

## 🔒 Security

- Never commit secrets (API keys, passwords, etc.)
- Use environment variables for configuration
- Sanitize user input
- Validate all data
- Follow secure coding practices
- Report security vulnerabilities privately

## 📜 License

By contributing to this project, you agree that your contributions will be licensed under the [MIT License](LICENSE).

## 🤝 Developer Certificate of Origin (DCO)

To ensure we can accept your contributions, we use the [Developer Certificate of Origin (DCO)](https://developercertificate.org/). This is a simple statement that you have the right to submit your contributions.

When you make a commit, you should include a `Signed-off-by` line:

```
git commit -m "Your commit message" --signoff
```

Or use `-s` for short:

```
git commit -m "Your commit message" -s
```

This adds a line like:

```
Signed-off-by: Your Name <your.email@example.com>
```

## 🌍 Community Guidelines

### Be Respectful

- Treat everyone with respect
- Be welcoming to newcomers
- Assume good intentions
- Disagree respectfully

### Be Inclusive

- Use inclusive language
- Consider different perspectives
- Be mindful of cultural differences
- Ensure accessibility

### Be Helpful

- Help others when you can
- Share knowledge
- Answer questions
- Review pull requests

### Be Patient

- Everyone learns at different speeds
- Not everyone has the same experience
- Maintainers are volunteers
- Good things take time

## 📞 Getting Help

If you need help:

1. Check the [documentation](docs/)
2. Search [existing issues](https://github.com/johanneskueng/community_based_project_dev/issues)
3. Ask in [GitHub Discussions](https://github.com/johanneskueng/community_based_project_dev/discussions)
4. Open a [new issue](https://github.com/johanneskueng/community_based_project_dev/issues/new)

## 🙏 Recognition

All contributions are valued and recognized. Contributors will be:

- Listed in the [CONTRIBUTORS.md](CONTRIBUTORS.md) file
- Recognized in release notes
- Invited to contribute to future roadmap discussions

---

*Thank you for contributing to the Sociocultural Project Development Environment!*

*Last Updated: 2024*
