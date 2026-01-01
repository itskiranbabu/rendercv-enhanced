# 🤝 Contributing to RenderCV Enhanced

First off, thank you for considering contributing to RenderCV Enhanced! It's people like you that make this project better for everyone.

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*

---

## 📋 Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Development Setup](#development-setup)
- [Contribution Guidelines](#contribution-guidelines)
- [Style Guidelines](#style-guidelines)
- [Commit Messages](#commit-messages)
- [Pull Request Process](#pull-request-process)
- [Community](#community)

---

## 📜 Code of Conduct

This project and everyone participating in it is governed by our Code of Conduct. By participating, you are expected to uphold this code.

### Our Pledge

We pledge to make participation in our project a harassment-free experience for everyone, regardless of:
- Age, body size, disability, ethnicity
- Gender identity and expression
- Level of experience, education
- Nationality, personal appearance, race, religion
- Sexual identity and orientation

### Our Standards

**Positive behavior includes:**
✅ Using welcoming and inclusive language
✅ Being respectful of differing viewpoints
✅ Gracefully accepting constructive criticism
✅ Focusing on what is best for the community
✅ Showing empathy towards others

**Unacceptable behavior includes:**
❌ Trolling, insulting/derogatory comments
❌ Public or private harassment
❌ Publishing others' private information
❌ Other conduct which could reasonably be considered inappropriate

---

## 🎯 How Can I Contribute?

### 1. **Report Bugs** 🐛

Found a bug? Help us fix it!

**Before submitting:**
- Check if the bug has already been reported
- Collect information about the bug
- Test with the latest version

**Submit a bug report:**
- Use the bug report template
- Provide clear title and description
- Include steps to reproduce
- Add screenshots if applicable
- Mention your environment (OS, Python version)

[Report a Bug](https://github.com/itskiranbabu/rendercv-enhanced/issues/new?template=bug_report.md)

### 2. **Suggest Features** 💡

Have an idea? We'd love to hear it!

**Before suggesting:**
- Check if it's already suggested
- Ensure it aligns with project goals
- Consider if it benefits most users

**Submit a feature request:**
- Use the feature request template
- Explain the problem it solves
- Describe your proposed solution
- Provide examples if possible

[Request a Feature](https://github.com/itskiranbabu/rendercv-enhanced/issues/new?template=feature_request.md)

### 3. **Improve Documentation** 📚

Documentation is crucial!

**You can help by:**
- Fixing typos and grammar
- Adding examples
- Clarifying confusing sections
- Translating to other languages
- Adding tutorials
- Improving code comments

### 4. **Add AI Learning Resources** 🤖

Share valuable AI/ML resources!

**Contribute:**
- Online courses
- Books and papers
- YouTube channels
- Tutorials and guides
- Tools and frameworks
- Career resources

### 5. **Create Themes** 🎨

Design new CV themes!

**Requirements:**
- Professional appearance
- ATS-friendly
- Well-documented
- Example CV included

### 6. **Write Code** 💻

Contribute code improvements!

**Areas to contribute:**
- Bug fixes
- New features
- Performance improvements
- Code refactoring
- Test coverage

---

## 🚀 Getting Started

### Prerequisites

- **Python**: 3.12 or higher
- **Git**: Version control
- **GitHub Account**: For pull requests
- **Text Editor**: VS Code recommended

### Fork and Clone

1. **Fork the repository**
   - Click "Fork" button on GitHub
   - This creates your copy

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/rendercv-enhanced.git
   cd rendercv-enhanced
   ```

3. **Add upstream remote**
   ```bash
   git remote add upstream https://github.com/itskiranbabu/rendercv-enhanced.git
   ```

4. **Verify remotes**
   ```bash
   git remote -v
   # origin    https://github.com/YOUR_USERNAME/rendercv-enhanced.git (fetch)
   # origin    https://github.com/YOUR_USERNAME/rendercv-enhanced.git (push)
   # upstream  https://github.com/itskiranbabu/rendercv-enhanced.git (fetch)
   # upstream  https://github.com/itskiranbabu/rendercv-enhanced.git (push)
   ```

---

## 🛠️ Development Setup

### 1. Create Virtual Environment

```bash
# Create virtual environment
python -m venv venv

# Activate (Windows)
venv\Scripts\activate

# Activate (macOS/Linux)
source venv/bin/activate
```

### 2. Install Dependencies

```bash
# Install in development mode
pip install -e ".[full]"

# Install development dependencies
pip install -r requirements-dev.txt
```

### 3. Install Pre-commit Hooks

```bash
# Install pre-commit
pip install pre-commit

# Set up hooks
pre-commit install
```

### 4. Verify Setup

```bash
# Run tests
pytest

# Check code style
ruff check .

# Format code
black .
```

---

## 📝 Contribution Guidelines

### Branch Naming

Use descriptive branch names:

```bash
# Feature branches
git checkout -b feature/add-new-theme
git checkout -b feature/ai-resources-nlp

# Bug fix branches
git checkout -b fix/yaml-parsing-error
git checkout -b fix/pdf-generation-issue

# Documentation branches
git checkout -b docs/update-installation-guide
git checkout -b docs/add-examples

# Enhancement branches
git checkout -b enhance/improve-performance
git checkout -b enhance/add-validation
```

### Making Changes

1. **Create a branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes**
   - Write clear, readable code
   - Follow style guidelines
   - Add tests if applicable
   - Update documentation

3. **Test your changes**
   ```bash
   # Run tests
   pytest
   
   # Check coverage
   pytest --cov=rendercv
   
   # Lint code
   ruff check .
   
   # Format code
   black .
   ```

4. **Commit your changes**
   ```bash
   git add .
   git commit -m "feat: add new theme for designers"
   ```

5. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create Pull Request**
   - Go to your fork on GitHub
   - Click "New Pull Request"
   - Fill in the PR template
   - Submit for review

---

## 🎨 Style Guidelines

### Python Code Style

We follow **PEP 8** with some modifications:

```python
# Good: Clear, descriptive names
def generate_cv_from_yaml(yaml_file_path: str) -> str:
    """Generate CV PDF from YAML file.
    
    Args:
        yaml_file_path: Path to YAML file
        
    Returns:
        Path to generated PDF
    """
    pass

# Bad: Unclear names
def gen(f):
    pass
```

**Key points:**
- Use 4 spaces for indentation
- Maximum line length: 88 characters
- Use type hints
- Write docstrings for functions
- Use meaningful variable names

### Documentation Style

```markdown
# Good: Clear, structured

## Installation

### Prerequisites

- Python 3.12+
- pip

### Steps

1. Install package
   ```bash
   pip install rendercv
   ```

2. Verify installation
   ```bash
   rendercv --version
   ```

# Bad: Unclear, unstructured

install it with pip install rendercv and check version
```

### YAML Style

```yaml
# Good: Consistent, clear
cv:
  name: John Doe
  email: john@example.com
  
  sections:
    experience:
      - company: Tech Corp
        position: Engineer
        highlights:
          - "Achievement 1"
          - "Achievement 2"

# Bad: Inconsistent
cv:
  name: John Doe
  email:john@example.com
  sections:
    experience:
    - company:Tech Corp
      position:Engineer
```

---

## 💬 Commit Messages

We follow **Conventional Commits** specification:

### Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: New feature
- **fix**: Bug fix
- **docs**: Documentation changes
- **style**: Code style changes (formatting)
- **refactor**: Code refactoring
- **test**: Adding or updating tests
- **chore**: Maintenance tasks

### Examples

```bash
# Feature
git commit -m "feat(themes): add modern designer theme"

# Bug fix
git commit -m "fix(yaml): resolve parsing error for nested sections"

# Documentation
git commit -m "docs(readme): update installation instructions"

# Multiple lines
git commit -m "feat(ai-resources): add NLP learning section

- Added Stanford CS224N course
- Added Hugging Face tutorials
- Added NLP books and papers

Closes #123"
```

### Good Commit Messages

✅ **Good:**
```
feat(themes): add minimalist theme for designers

- Created new minimalist theme
- Added example CV
- Updated documentation
- Added theme preview image

Closes #45
```

❌ **Bad:**
```
updated stuff
```

---

## 🔄 Pull Request Process

### Before Submitting

**Checklist:**
- [ ] Code follows style guidelines
- [ ] Tests pass locally
- [ ] Documentation updated
- [ ] Commit messages follow convention
- [ ] Branch is up to date with main
- [ ] No merge conflicts

### PR Template

When creating a PR, include:

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Code refactoring

## Testing
How to test these changes

## Screenshots (if applicable)
Add screenshots

## Checklist
- [ ] Code follows style guidelines
- [ ] Tests added/updated
- [ ] Documentation updated
- [ ] No breaking changes
```

### Review Process

1. **Automated checks run**
   - Tests must pass
   - Linting must pass
   - Coverage must not decrease

2. **Code review**
   - Maintainer reviews code
   - Feedback provided
   - Changes requested if needed

3. **Approval and merge**
   - Once approved, PR is merged
   - Branch is deleted
   - Changes go live

### After Merge

- Your contribution is live! 🎉
- You're added to contributors list
- Thank you message posted

---

## 🧪 Testing Guidelines

### Writing Tests

```python
# tests/test_yaml_parser.py
import pytest
from rendercv import parse_yaml

def test_parse_valid_yaml():
    """Test parsing valid YAML file."""
    result = parse_yaml("examples/valid_cv.yaml")
    assert result is not None
    assert result["cv"]["name"] == "John Doe"

def test_parse_invalid_yaml():
    """Test parsing invalid YAML raises error."""
    with pytest.raises(ValueError):
        parse_yaml("examples/invalid_cv.yaml")
```

### Running Tests

```bash
# Run all tests
pytest

# Run specific test file
pytest tests/test_yaml_parser.py

# Run with coverage
pytest --cov=rendercv

# Run with verbose output
pytest -v

# Run in parallel
pytest -n auto
```

---

## 📚 Documentation Guidelines

### Adding Documentation

**Structure:**
```markdown
# Title

Brief introduction

## Section 1

Content with examples

### Subsection

More details

## Section 2

More content
```

**Code Examples:**
````markdown
```python
# Example code
def hello_world():
    print("Hello, World!")
```
````

**Tips:**
- Use clear headings
- Add code examples
- Include screenshots
- Link to related docs
- Keep it concise

---

## 🌟 Recognition

### Contributors

All contributors are recognized in:
- README.md contributors section
- CHANGELOG.md for each release
- GitHub contributors page

### Hall of Fame

Top contributors get:
- Special mention in README
- Contributor badge
- Shoutout on social media
- Early access to new features

---

## 💬 Community

### Get Help

- **Documentation**: [Read the docs](DOCUMENTATION.md)
- **Discussions**: [GitHub Discussions](https://github.com/itskiranbabu/rendercv-enhanced/discussions)
- **WhatsApp Channel**: [Join Channel](https://whatsapp.com/channel/0029VbCCj7FGJP8EeBLXzD1C)
- **WhatsApp Group**: [Join Group](https://chat.whatsapp.com/IfIKh4bVhCc1qjPEOFKQeh)

### Stay Updated

- **Watch** the repository for updates
- **Star** to show support
- **Follow** [@itskiranbabu](https://github.com/itskiranbabu)
- **Join** our WhatsApp communities

---

## 🎁 First-Time Contributors

New to open source? Welcome! 🎉

### Good First Issues

Look for issues labeled:
- `good first issue` - Easy to start
- `help wanted` - Need assistance
- `documentation` - Doc improvements

### Resources

- [First Contributions Guide](https://github.com/firstcontributions/first-contributions)
- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)

---

## 📞 Contact

**Maintainer**: [itskiranbabu](https://github.com/itskiranbabu)

**Email**: itskeyrun.ai@gmail.com

**LinkedIn**: [itskiranbabu](https://linkedin.com/in/itskiranbabu)

---

## 🙏 Thank You!

Thank you for contributing to RenderCV Enhanced! Your contributions help thousands of developers create professional CVs and learn AI/ML.

Every contribution, no matter how small, makes a difference! 🌟

---

**Happy Contributing!** 🚀

*Curated by [itskiranbabu](https://github.com/itskiranbabu) | Powered by KeyRun AI*
