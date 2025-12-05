# Frequently Asked Questions (FAQ)

Find answers to common questions about the Product Analytics Handbook.

## Table of Contents

- [General Questions](#general-questions)
- [Installation & Setup](#installation--setup)
- [Usage & Features](#usage--features)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [Data & Privacy](#data--privacy)

---

## General Questions

### What is the Product Analytics Handbook?

The Product Analytics Handbook is an interactive learning platform built with Streamlit that helps users master product analytics concepts through hands-on exercises, real-world examples, and interactive visualizations.

### Who is this project for?

This project is designed for:
- **Product Managers** learning data-driven decision making
- **Data Analysts** expanding their product analytics skills
- **Data Scientists** applying analytics to product problems
- **Students** studying statistics and data science
- **Anyone** interested in learning product analytics

### Is this project free to use?

Yes! This project is completely free and open-source under the MIT License. You can use, modify, and distribute it freely.

### Do I need programming experience?

Basic Python knowledge is helpful but not required. The application is designed to be user-friendly with interactive elements that don't require coding. However, understanding the code examples will enhance your learning.

### Can I use this for commercial purposes?

Yes, the MIT License allows commercial use. However, we appreciate attribution and contributions back to the project.

---

## Installation & Setup

### What are the system requirements?

- **Python**: 3.8 or higher
- **RAM**: 4GB minimum, 8GB recommended
- **Disk Space**: ~500MB for application and dependencies
- **OS**: Windows 10+, macOS 10.14+, or Linux

### How do I install Python?

Download Python from [python.org](https://www.python.org/downloads/). Make sure to check "Add Python to PATH" during installation on Windows.

### The installation failed. What should I do?

1. Ensure Python 3.8+ is installed: `python --version`
2. Update pip: `pip install --upgrade pip`
3. Try installing in a virtual environment
4. Check our [Installation Guide](INSTALLATION.md) for detailed troubleshooting
5. If issues persist, [open an issue](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues)

### Do I need to install Git?

Git is only needed if you want to clone the repository. Alternatively, you can download the project as a ZIP file from GitHub.

### Can I use this with Anaconda/Conda?

Yes! Create a conda environment and install the requirements:
```bash
conda create -n product-analytics python=3.10
conda activate product-analytics
pip install -r streamlit_app/Product_Analytics/requirements.txt
```

---

## Usage & Features

### How do I start the application?

After installation, run:
```bash
streamlit run streamlit_app/Product_Analytics/main.py
```
The app will open in your default browser.

### The application isn't opening in my browser

1. Check the terminal for the URL (usually `http://localhost:8501`)
2. Manually open that URL in your browser
3. Try a different browser
4. Check if port 8501 is already in use

### Can I upload my own data?

Yes! Many sections support CSV file uploads. Look for the "Upload CSV" button. Ensure your data:
- Is in CSV format
- Has column headers
- Is under 200MB (default limit)

### How do I save my work?

The application doesn't automatically save progress. To preserve your work:
- Take screenshots of visualizations
- Download charts where available
- Export results to CSV (if supported)
- Bookmark specific pages

### Can I use this offline?

Yes, once installed, the application runs locally and works offline. However, some features require internet:
- FRED API (economic data)
- yfinance (financial data)
- Package updates

### What file formats are supported?

Currently, the application primarily supports:
- **CSV files** for data upload
- **PNG/JPEG** for screenshots and exports

### Can I export visualizations?

Yes! Most visualizations can be downloaded:
- Right-click on charts → "Save image as..."
- Use the camera icon (Plotly charts)
- Take screenshots

---

## Troubleshooting

### The page is loading very slowly

**Solutions:**
- Use smaller datasets (< 100K rows)
- Close unused browser tabs
- Restart the Streamlit server
- Check system resources (RAM, CPU)
- Clear browser cache

### I'm getting import errors

**Solutions:**
```bash
# Reinstall dependencies
pip install -r streamlit_app/Product_Analytics/requirements.txt --force-reinstall

# Or in a fresh environment
python -m venv fresh_env
source fresh_env/bin/activate  # Windows: fresh_env\Scripts\activate
pip install -r streamlit_app/Product_Analytics/requirements.txt
```

### Visualizations aren't displaying

**Solutions:**
- Enable JavaScript in your browser
- Try a different browser (Chrome, Firefox, Safari)
- Check browser console for errors
- Update Streamlit: `pip install --upgrade streamlit`

### Data upload isn't working

**Common issues:**
- **File too large**: Default limit is 200MB
- **Wrong format**: Must be CSV
- **Encoding issues**: Try UTF-8 encoding
- **Corrupted file**: Verify file opens in Excel/text editor

### Port 8501 is already in use

**Solutions:**
```bash
# Use a different port
streamlit run streamlit_app/Product_Analytics/main.py --server.port 8502

# Or find and kill the process using port 8501
# Linux/macOS:
lsof -ti:8501 | xargs kill -9
# Windows:
netstat -ano | findstr :8501
# Then use Task Manager to end the process
```

### The application crashed

**Steps:**
1. Check the terminal for error messages
2. Restart the application
3. If it persists, clear Streamlit cache
4. Try with a fresh virtual environment
5. Report the issue with error details

---

## Contributing

### How can I contribute?

See our [Contributing Guide](CONTRIBUTING.md) for detailed instructions. Common ways to contribute:
- Report bugs
- Suggest features
- Improve documentation
- Add new analytical topics
- Fix issues
- Share the project

### I found a bug. Where do I report it?

[Open an issue](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues/new/choose) on GitHub using the Bug Report template.

### I have a feature request

Great! [Open a feature request](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues/new/choose) using the Feature Request template.

### How do I submit a pull request?

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request using our [PR template](.github/PULL_REQUEST_TEMPLATE.md)

### Can I add my own analytical examples?

Absolutely! We welcome new examples and case studies. Please ensure they:
- Are well-documented
- Include sample data (or data generation code)
- Follow the existing code style
- Add educational value

---

## Data & Privacy

### Is my uploaded data secure?

The application processes data locally on your machine. No data is sent to external servers except when using specific APIs (FRED, yfinance).

### What data is collected?

The application doesn't collect any personal data. Standard Streamlit analytics may be collected by Streamlit Inc. (disable in settings).

### Can I use sensitive data?

**Recommendations:**
- Anonymize sensitive data before upload
- Don't commit data to the repository
- Be aware of your organization's data policies
- Use synthetic data for public demonstrations

### Do I need API keys?

**Optional API keys:**
- **FRED API**: For economic data features (free registration)
- **yfinance**: No key needed

Store keys in `.streamlit/secrets.toml` (see [SECURITY.md](SECURITY.md))

### Where is data stored?

- Uploaded data is in **browser memory** (cleared on page reload)
- The application doesn't persist data to disk
- Cache is temporary and cleared on restart

---

## Additional Questions

### Can I use this for teaching?

Yes! This is an excellent teaching resource. We encourage educators to use it. Please:
- Credit the project
- Share improvements back to the community
- Consider contributing educational content

### Is there a mobile version?

The application is responsive and works on tablets. Phone support is limited due to the complexity of visualizations. Desktop/laptop use is recommended.

### Can I deploy this online?

Yes! You can deploy to:
- **Streamlit Community Cloud** (free)
- **Heroku**
- **AWS, GCP, Azure**
- **Your own server**

See Streamlit's [deployment guide](https://docs.streamlit.io/streamlit-community-cloud/get-started/deploy-an-app) for instructions.

### How often is the project updated?

Updates are released as needed. Follow the repository and check the [Changelog](CHANGELOG.md) for version history.

### Can I translate this to another language?

Internationalization is on our roadmap. For now, you can fork the project and create a translated version. Consider contributing it back!

### Who maintains this project?

The project is maintained by Moshe Shamouilian and the community. See [AUTHORS.md](AUTHORS.md) for contributors.

---

## Still Have Questions?

- 💬 [Start a discussion](https://github.com/Analytical-Guide/Product-Analytical-Apps/discussions)
- 📧 [Open an issue](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues)
- 📖 Check our [documentation](docs/)

---

**Don't see your question here?** [Let us know](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues/new) and we'll add it!
