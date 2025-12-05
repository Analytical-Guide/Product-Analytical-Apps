# Contributing to Product Analytics Handbook

First off, thank you for considering contributing to the Product Analytics Handbook! 🎉

It's people like you that make this project such a great learning resource for the community. We welcome contributions from everyone, whether you're fixing a typo, adding a new feature, or improving documentation.

## 📋 Table of Contents

1. [Code of Conduct](#code-of-conduct)
2. [Getting Started](#getting-started)
3. [How Can I Contribute?](#how-can-i-contribute)
4. [Development Setup](#development-setup)
5. [Style Guidelines](#style-guidelines)
6. [Commit Message Guidelines](#commit-message-guidelines)
7. [Pull Request Process](#pull-request-process)
8. [Community](#community)

---

## 📜 Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to the project maintainers.

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Git
- A GitHub account

### First Time Contributors

Never contributed to an open source project before? Here are some helpful resources:
- [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
- [First Timers Only](https://www.firsttimersonly.com/)
- [GitHub Flow Guide](https://guides.github.com/introduction/flow/)

---

## 🤝 How Can I Contribute?

### Reporting Bugs 🐛

Before creating bug reports, please check existing issues to avoid duplicates. When creating a bug report, include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps to reproduce the problem**
- **Provide specific examples** (code snippets, screenshots, etc.)
- **Describe the behavior you observed** and what you expected
- **Include your environment details** (OS, Python version, browser, etc.)

**Bug Report Template:**
```markdown
**Description:**
A clear description of the bug.

**Steps to Reproduce:**
1. Go to '...'
2. Click on '...'
3. Scroll down to '...'
4. See error

**Expected Behavior:**
What you expected to happen.

**Actual Behavior:**
What actually happened.

**Environment:**
- OS: [e.g., macOS, Windows, Linux]
- Python Version: [e.g., 3.10]
- Browser: [e.g., Chrome, Firefox]

**Screenshots:**
If applicable, add screenshots.
```

### Suggesting Enhancements 💡

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- **Use a clear and descriptive title**
- **Provide a detailed description** of the suggested enhancement
- **Explain why this enhancement would be useful** to most users
- **List any alternative solutions** you've considered
- **Include mockups or examples** if applicable

**Enhancement Template:**
```markdown
**Feature Request:**
A clear description of the feature.

**Problem It Solves:**
Explain the problem this feature addresses.

**Proposed Solution:**
Describe how you envision this working.

**Alternatives Considered:**
Any alternative solutions you've thought about.

**Additional Context:**
Add any other context, screenshots, or examples.
```

### Adding Content 📚

We especially welcome contributions that add:

- **New analytical topics** (e.g., Bayesian analysis, causal inference)
- **Real-world case studies** with datasets
- **Interactive examples** and demonstrations
- **Additional visualizations** and insights
- **Improved explanations** of existing topics
- **Practice exercises** with solutions

### Improving Documentation 📖

Documentation improvements are always welcome:

- Fix typos and grammatical errors
- Clarify confusing explanations
- Add missing documentation
- Improve code comments
- Create tutorials and guides
- Add examples and use cases

---

## 💻 Development Setup

1. **Fork and Clone**
   ```bash
   # Fork the repository on GitHub, then:
   git clone https://github.com/YOUR_USERNAME/Product-Analytical-Apps.git
   cd Product-Analytical-Apps
   ```

2. **Create a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r streamlit_app/Product_Analytics/requirements.txt
   ```

4. **Create a Branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/your-bug-fix
   ```

5. **Make Your Changes**
   - Edit files as needed
   - Test your changes thoroughly

6. **Test Locally**
   ```bash
   streamlit run streamlit_app/Product_Analytics/main.py
   ```

7. **Commit and Push**
   ```bash
   git add .
   git commit -m "Your descriptive commit message"
   git push origin feature/your-feature-name
   ```

---

## 🎨 Style Guidelines

### Python Code Style

- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) guidelines
- Use meaningful variable and function names
- Add docstrings to functions and classes
- Keep functions focused and small
- Use type hints where appropriate

**Example:**
```python
def calculate_mean(data: list[float]) -> float:
    """
    Calculate the arithmetic mean of a list of numbers.
    
    Args:
        data: A list of numeric values
        
    Returns:
        The arithmetic mean of the values
        
    Raises:
        ValueError: If the data list is empty
    """
    if not data:
        raise ValueError("Cannot calculate mean of empty list")
    return sum(data) / len(data)
```

### Streamlit App Guidelines

- Keep UI clean and intuitive
- Use consistent styling across pages
- Add helpful tooltips and explanations
- Handle errors gracefully with user-friendly messages
- Use caching (`@st.cache_data`) for expensive operations
- Organize code into logical sections with headers

### Documentation Style

- Use clear, concise language
- Include examples where helpful
- Use proper markdown formatting
- Keep line length reasonable (80-100 characters)
- Use headers to organize content
- Include links to related resources

---

## 📝 Commit Message Guidelines

Write clear, descriptive commit messages following this format:

```
Type: Brief description (50 chars or less)

More detailed explanatory text, if necessary. Wrap it to about 72
characters. Explain the problem that this commit is solving.

- Bullet points are okay
- Use imperative mood ("Add feature" not "Added feature")

Resolves: #123
See also: #456, #789
```

### Commit Types:

- **Add:** New feature or content
- **Fix:** Bug fix
- **Update:** Update existing feature or content
- **Refactor:** Code restructuring without changing functionality
- **Style:** Formatting, missing semicolons, etc.
- **Docs:** Documentation changes
- **Test:** Adding or updating tests
- **Chore:** Maintenance tasks

**Examples:**
```
Add: Interactive histogram visualization for distributions

Fix: Correct calculation in variance function

Update: Improve explanation of hypothesis testing

Docs: Add examples to README installation section

Refactor: Reorganize utility functions for better modularity
```

---

## 🔄 Pull Request Process

1. **Ensure your changes work**
   - Test the application locally
   - Verify all pages load correctly
   - Check for any errors in the console

2. **Update documentation**
   - Update README.md if needed
   - Add docstrings to new functions
   - Update relevant comments

3. **Create a Pull Request**
   - Provide a clear title and description
   - Reference any related issues
   - Include screenshots for UI changes
   - List any breaking changes

4. **PR Template:**
   ```markdown
   ## Description
   Brief description of what this PR does.
   
   ## Type of Change
   - [ ] Bug fix
   - [ ] New feature
   - [ ] Documentation update
   - [ ] Code refactoring
   
   ## Related Issues
   Fixes #(issue number)
   
   ## Changes Made
   - Change 1
   - Change 2
   - Change 3
   
   ## Screenshots (if applicable)
   Add screenshots here
   
   ## Testing
   - [ ] I have tested these changes locally
   - [ ] All pages load without errors
   - [ ] Documentation is updated
   
   ## Checklist
   - [ ] My code follows the project's style guidelines
   - [ ] I have performed a self-review
   - [ ] I have commented my code where necessary
   - [ ] My changes generate no new warnings
   - [ ] I have updated the documentation accordingly
   ```

5. **Review Process**
   - Maintainers will review your PR
   - Address any requested changes
   - Once approved, your PR will be merged

---

## 👥 Community

### Getting Help

- 📖 Check the [README](README.md) and documentation first
- 🔍 Search [existing issues](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues)
- 💬 Start a [discussion](https://github.com/Analytical-Guide/Product-Analytical-Apps/discussions)
- 📧 Contact maintainers if needed

### Recognition

Contributors will be recognized in:
- GitHub contributors page
- Release notes (for significant contributions)
- Special mentions in documentation

---

## 🎯 What Makes a Good Contribution?

- **Clear purpose**: Solves a specific problem or adds clear value
- **Well tested**: Works correctly and doesn't break existing functionality
- **Well documented**: Includes necessary documentation and comments
- **Follows guidelines**: Adheres to the project's style and conventions
- **Focused**: Addresses one issue or feature at a time
- **Professional**: Maintains a respectful and collaborative tone

---

## 📚 Resources

- [Streamlit Documentation](https://docs.streamlit.io/)
- [Python Documentation](https://docs.python.org/3/)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Matplotlib Documentation](https://matplotlib.org/stable/contents.html)
- [GitHub Guides](https://guides.github.com/)

---

## ❓ Questions?

Don't hesitate to ask questions! You can:
- Open an issue with the "question" label
- Start a discussion on GitHub Discussions
- Reach out to the maintainers

---

<div align="center">

**Thank you for contributing to Product Analytics Handbook! 🙌**

Every contribution, no matter how small, makes a difference!

</div>
