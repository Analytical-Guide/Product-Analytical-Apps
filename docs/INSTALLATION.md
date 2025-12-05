# Installation Guide

This guide provides detailed instructions for installing and setting up the Product Analytics Handbook on various platforms.

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Installation Methods](#installation-methods)
3. [Platform-Specific Instructions](#platform-specific-instructions)
4. [Troubleshooting](#troubleshooting)
5. [Next Steps](#next-steps)

---

## Prerequisites

### Required Software

- **Python 3.8 or higher** - [Download Python](https://www.python.org/downloads/)
- **pip** - Python package manager (usually comes with Python)
- **Git** - [Download Git](https://git-scm.com/downloads)

### Recommended Software

- **Visual Studio Code** or another code editor - [Download VS Code](https://code.visualstudio.com/)
- **Virtual environment tool** (venv, virtualenv, or conda)

### System Requirements

- **Operating System**: Windows 10+, macOS 10.14+, or Linux
- **RAM**: 4GB minimum, 8GB recommended
- **Disk Space**: 500MB for application and dependencies

---

## Installation Methods

### Method 1: Quick Install (Recommended)

```bash
# Clone the repository
git clone https://github.com/Analytical-Guide/Product-Analytical-Apps.git
cd Product-Analytical-Apps

# Install dependencies
pip install -r streamlit_app/Product_Analytics/requirements.txt

# Run the application
streamlit run streamlit_app/Product_Analytics/main.py
```

### Method 2: Virtual Environment (Best Practice)

```bash
# Clone the repository
git clone https://github.com/Analytical-Guide/Product-Analytical-Apps.git
cd Product-Analytical-Apps

# Create virtual environment
python -m venv venv

# Activate virtual environment
# On macOS/Linux:
source venv/bin/activate
# On Windows:
venv\Scripts\activate

# Install dependencies
pip install -r streamlit_app/Product_Analytics/requirements.txt

# Run the application
streamlit run streamlit_app/Product_Analytics/main.py
```

### Method 3: Using Conda

```bash
# Clone the repository
git clone https://github.com/Analytical-Guide/Product-Analytical-Apps.git
cd Product-Analytical-Apps

# Create conda environment
conda create -n product-analytics python=3.10
conda activate product-analytics

# Install dependencies
pip install -r streamlit_app/Product_Analytics/requirements.txt

# Run the application
streamlit run streamlit_app/Product_Analytics/main.py
```

---

## Platform-Specific Instructions

### Windows

1. **Install Python**
   - Download from [python.org](https://www.python.org/downloads/)
   - ✅ Check "Add Python to PATH" during installation
   - Verify: Open Command Prompt and run `python --version`

2. **Install Git**
   - Download from [git-scm.com](https://git-scm.com/download/win)
   - Use default settings during installation
   - Verify: Run `git --version` in Command Prompt

3. **Follow Method 2** (Virtual Environment) above

**Windows-specific tips:**
- Use Command Prompt or PowerShell
- If you get execution policy errors, run: `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`

### macOS

1. **Install Homebrew** (if not already installed)
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

2. **Install Python**
   ```bash
   brew install python
   ```

3. **Install Git** (usually pre-installed)
   ```bash
   brew install git
   ```

4. **Follow Method 2** (Virtual Environment) above

**macOS-specific tips:**
- Use Terminal app
- You may need to install Xcode Command Line Tools: `xcode-select --install`

### Linux (Ubuntu/Debian)

1. **Update package list**
   ```bash
   sudo apt update
   ```

2. **Install Python and pip**
   ```bash
   sudo apt install python3 python3-pip python3-venv git
   ```

3. **Follow Method 2** (Virtual Environment) above

**Linux-specific tips:**
- Use `python3` instead of `python`
- Use `pip3` instead of `pip`
- You may need to install additional dependencies for some packages

---

## Troubleshooting

### Common Issues

#### Issue: "python: command not found"
**Solution:**
- Ensure Python is installed and added to PATH
- On some systems, use `python3` instead of `python`

#### Issue: "pip: command not found"
**Solution:**
```bash
# Install pip
python -m ensurepip --upgrade
# or
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py
```

#### Issue: "Permission denied" when installing packages
**Solution:**
- Use a virtual environment (recommended)
- Or use `pip install --user` flag
- On Linux/macOS, avoid using `sudo pip` (use virtual environment instead)

#### Issue: Dependency conflicts
**Solution:**
```bash
# Create fresh virtual environment
python -m venv fresh_env
source fresh_env/bin/activate  # or fresh_env\Scripts\activate on Windows
pip install --upgrade pip
pip install -r streamlit_app/Product_Analytics/requirements.txt
```

#### Issue: Streamlit doesn't open in browser
**Solution:**
1. Check if the application is running (look for URL in terminal)
2. Manually open: `http://localhost:8501` in your browser
3. Check if port 8501 is already in use:
   ```bash
   # On Linux/macOS
   lsof -i :8501
   # On Windows
   netstat -ano | findstr :8501
   ```
4. Use a different port:
   ```bash
   streamlit run streamlit_app/Product_Analytics/main.py --server.port 8502
   ```

#### Issue: Module import errors
**Solution:**
```bash
# Reinstall dependencies
pip install -r streamlit_app/Product_Analytics/requirements.txt --force-reinstall
```

### Getting Help

If you encounter issues not covered here:

1. Check the [GitHub Issues](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues)
2. Search for existing solutions
3. Open a new issue with:
   - Your operating system and version
   - Python version (`python --version`)
   - Full error message
   - Steps you've already tried

---

## Verifying Installation

After installation, verify everything works:

```bash
# Check Python version
python --version  # Should be 3.8 or higher

# Check Streamlit installation
streamlit --version

# Test the application
streamlit run streamlit_app/Product_Analytics/main.py
```

The application should open in your browser at `http://localhost:8501`

---

## Next Steps

Once installed successfully:

1. 📖 **Read the [Usage Guide](USAGE.md)** to learn how to navigate the application
2. 🎯 **Start with "Data Fundamentals"** in the sidebar
3. 💡 **Explore interactive demos** in each section
4. 🤝 **Consider contributing** - see [CONTRIBUTING.md](../CONTRIBUTING.md)

---

## Advanced Configuration

### Custom Port

```bash
streamlit run streamlit_app/Product_Analytics/main.py --server.port 8080
```

### Custom Theme

Create `.streamlit/config.toml`:
```toml
[theme]
primaryColor = "#1f77b4"
backgroundColor = "#ffffff"
secondaryBackgroundColor = "#f0f2f6"
textColor = "#262730"
font = "sans serif"
```

### Performance Optimization

For large datasets:
```toml
# .streamlit/config.toml
[server]
maxUploadSize = 200
```

---

## Updating

To update to the latest version:

```bash
cd Product-Analytical-Apps
git pull origin main
pip install -r streamlit_app/Product_Analytics/requirements.txt --upgrade
```

---

**Need more help?** Join the discussions on [GitHub](https://github.com/Analytical-Guide/Product-Analytical-Apps/discussions)!
