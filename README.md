# 📊 Product Analytics Handbook

<div align="center">

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/streamlit-latest-red.svg)
![Status](https://img.shields.io/badge/status-active-success.svg)
![Contributions Welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)

**An interactive platform for mastering product analytics with hands-on learning and real-world applications**

[🚀 Get Started](#-quick-start) • [📖 Documentation](#-table-of-contents) • [🤝 Contributing](#-contributing) • [💡 Features](#-features) • [📋 Installation Guide](docs/INSTALLATION.md) • [📚 Usage Guide](docs/USAGE.md)

</div>

---

## 🌟 Overview

The **Product Analytics Handbook** is a comprehensive, interactive learning platform designed to help product managers, data analysts, and data scientists master the essential concepts and techniques of product analytics. Built with **Streamlit**, this application provides an engaging, hands-on approach to learning with practical examples, interactive demos, and real-world applications.

### 🎯 Why This Project?

- **🎓 Learn by Doing**: Interactive demos and exercises reinforce theoretical concepts
- **📈 Real-World Focus**: Examples drawn from actual product analytics scenarios
- **🔬 Comprehensive Coverage**: From fundamentals to advanced topics and specialized applications
- **💻 Open Source**: Free to use, modify, and contribute
- **🚀 Modern Stack**: Built with cutting-edge data science tools and libraries

---

## ✨ Features

### 📚 **Fundamentals**
- **Probability**: Master distributions, statistical inference, and probabilistic thinking
- **Descriptive Statistics**: Learn measures of central tendency, dispersion, and data summarization
- **Data Visualization**: Create compelling charts and graphs to communicate insights
- **Data Quality & Validation**: Ensure accuracy and reliability in your analyses
- **KPIs & Metrics**: Define and implement effective Key Performance Indicators
- **Effective Communication**: Present data insights to stakeholders with clarity

### 🎯 **Advanced Topics**
- **Hypothesis Testing**: Design and conduct rigorous statistical tests
- **Time Series Analysis**: Identify trends, patterns, and seasonality in temporal data
- **A/B Testing**: Optimize products through controlled experiments
- **Survival Analysis**: Analyze time-to-event data for customer lifecycle insights

### 🔥 **Real-World Applications**
- **Churn Analysis**: Identify and prevent customer attrition
- **Marketing Analytics**: Measure campaign effectiveness and ROI
- **Fraud Risk Analysis**: Detect and prevent fraudulent activities
- **Supply Chain Optimization**: Improve operational efficiency with data
- **Economic Demand Forecasting**: Predict future demand patterns

---

## 📖 Table of Contents

1. [Overview](#-overview)
2. [Features](#-features)
3. [Quick Start](#-quick-start)
4. [Installation](#-installation)
5. [Usage](#-usage)
6. [Documentation](#-documentation)
7. [Project Structure](#-project-structure)
8. [Technologies Used](#-technologies-used)
9. [Contributing](#-contributing)
10. [License](#-license)
11. [Acknowledgments](#-acknowledgments)

---

## 🚀 Quick Start

Get up and running in 3 simple steps:

```bash
# 1. Clone the repository
git clone https://github.com/Analytical-Guide/Product-Analytical-Apps.git
cd Product-Analytical-Apps

# 2. Install dependencies
pip install -r streamlit_app/Product_Analytics/requirements.txt

# 3. Launch the application
streamlit run streamlit_app/Product_Analytics/main.py
```

The application will open in your default browser at `http://localhost:8501` 🎉

---

## 💾 Installation

### Prerequisites

- **Python 3.8+** ([Download](https://www.python.org/downloads/))
- **pip** (Python package manager)

### Step-by-Step Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Analytical-Guide/Product-Analytical-Apps.git
   cd Product-Analytical-Apps
   ```

2. **Create a Virtual Environment** (Recommended)
   ```bash
   # On macOS/Linux
   python3 -m venv venv
   source venv/bin/activate
   
   # On Windows
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install Dependencies**
   ```bash
   pip install -r streamlit_app/Product_Analytics/requirements.txt
   ```

4. **Verify Installation**
   ```bash
   streamlit --version
   ```

---

## 🎮 Usage

### Running the Application

Start the Streamlit app:

```bash
streamlit run streamlit_app/Product_Analytics/main.py
```

### Navigation

- Use the **sidebar** to navigate between different topics
- Start with **Data Fundamentals** for the best learning experience
- Each section includes:
  - 📝 Theoretical concepts
  - 💡 Interactive demos
  - 🌍 Real-world applications

### Learning Path

**Recommended progression:**

1. **Foundations** → Probability, Statistics, Visualization
2. **Quality** → Data Quality, Validation, Metrics
3. **Analysis** → Hypothesis Testing, Time Series, A/B Testing
4. **Applications** → Churn, Marketing, Fraud, Supply Chain

---

## 📚 Documentation

Comprehensive guides to help you get the most out of the Product Analytics Handbook:

- 📋 **[Installation Guide](docs/INSTALLATION.md)** - Detailed setup instructions for all platforms
- 📖 **[Usage Guide](docs/USAGE.md)** - Learn how to navigate and use all features
- ❓ **[FAQ](docs/FAQ.md)** - Frequently asked questions and answers
- 🤝 **[Contributing Guide](CONTRIBUTING.md)** - Help improve this project
- 🔒 **[Security Policy](SECURITY.md)** - Report vulnerabilities and security best practices
- 📝 **[Changelog](CHANGELOG.md)** - Track all project changes and versions

### Quick Links

- **Need help installing?** → [Installation Guide](docs/INSTALLATION.md)
- **First time user?** → [Usage Guide](docs/USAGE.md)
- **Have questions?** → [FAQ](docs/FAQ.md)
- **Want to contribute?** → [Contributing Guide](CONTRIBUTING.md)
- **Found a bug?** → [Open an Issue](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues/new/choose)

---

## 📁 Project Structure

```
Product-Analytical-Apps/
├── streamlit_app/
│   └── Product_Analytics/
│       ├── main.py                 # Main application entry point
│       ├── requirements.txt        # Python dependencies
│       ├── pages/                  # Individual topic pages
│       │   ├── 1 1_Probability_Fundementals.py
│       │   ├── 1 2_Descriptive_Statistics_Fundementals.py
│       │   ├── 1 3_Data_visualization_Fundementals.py
│       │   ├── 1 4_Hypothesis_testing_Fundementals.py
│       │   ├── 1 5_Data-Quality_Fundementals.py
│       │   ├── 1 6_Metrics_Fundementals.py
│       │   ├── 1 8_Practial_Data-validation.py
│       │   ├── 1 9_Effective-Communication.py
│       │   ├── 3_Churn-Analytics-Intro.py
│       │   ├── 3_Fraud-Risk-Analytics-Intro.py
│       │   ├── 3_Marketing-Analytics-Into.py
│       │   ├── 7_survival_Analytics-Intro.py
│       │   └── 9_Feedback.py
│       ├── features/               # Advanced feature modules
│       │   ├── 6_A-B_Testing.py
│       │   ├── Combinatorics.py
│       │   ├── Economic-Demand-Forcasting.py
│       │   ├── Economic_dashboard.py
│       │   ├── Supply-Chain.py
│       │   └── Time-Series.py
│       ├── utils/                  # Utility functions
│       │   ├── data_utils.py
│       │   ├── stats_utils.py
│       │   ├── viz_utils.py
│       │   └── style_utils.py
│       └── data/                   # Sample datasets
├── docs/                           # Documentation
│   ├── FAQ.md                     # Frequently asked questions
│   ├── INSTALLATION.md            # Installation guide
│   ├── USAGE.md                   # Usage guide
│   └── images/                     # Screenshots and assets
├── .github/
│   ├── ISSUE_TEMPLATE/            # Issue templates
│   │   ├── bug_report.md
│   │   ├── feature_request.md
│   │   └── documentation.md
│   ├── PULL_REQUEST_TEMPLATE.md   # PR template
│   └── workflows/                  # CI/CD workflows
├── .gitignore                      # Git ignore rules
├── AUTHORS.md                      # Contributors list
├── CHANGELOG.md                    # Version history
├── CITATION.cff                    # Citation information
├── CODE_OF_CONDUCT.md             # Community guidelines
├── CONTRIBUTING.md                 # Contribution guide
├── LICENSE                         # MIT License
├── README.md                       # This file
└── SECURITY.md                     # Security policy
```

---

## 🛠️ Technologies Used

This project leverages modern data science and web technologies:

| Category | Technologies |
|----------|-------------|
| **Frontend** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) |
| **Data Analysis** | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white) ![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat&logo=scipy&logoColor=white) |
| **Visualization** | ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat) ![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat) ![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat&logo=plotly&logoColor=white) |
| **Machine Learning** | ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white) ![Statsmodels](https://img.shields.io/badge/Statsmodels-4B8BBE?style=flat) |
| **Specialized** | Lifelines (Survival Analysis), pmdarima (Time Series), imbalanced-learn (ML), Folium (Maps) |
| **Data Sources** | FRED API, yfinance |

---

## 🤝 Contributing

We welcome contributions from the community! Whether you're fixing bugs, adding features, or improving documentation, your help is appreciated.

### How to Contribute

1. **Fork the Repository**
   
   Click the "Fork" button at the top right of this page.

2. **Clone Your Fork**
   ```bash
   git clone https://github.com/YOUR_USERNAME/Product-Analytical-Apps.git
   cd Product-Analytical-Apps
   ```

3. **Create a Branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```

4. **Make Your Changes**
   
   - Follow the existing code style
   - Add comments where necessary
   - Update documentation if needed

5. **Test Your Changes**
   ```bash
   streamlit run streamlit_app/Product_Analytics/main.py
   ```

6. **Commit Your Changes**
   ```bash
   git add .
   git commit -m "Add: your descriptive commit message"
   ```

7. **Push to Your Fork**
   ```bash
   git push origin feature/your-feature-name
   ```

8. **Submit a Pull Request**
   
   Go to the original repository and click "New Pull Request"

### Contribution Guidelines

- **Code Quality**: Write clean, readable, and well-documented code
- **Testing**: Test your changes thoroughly before submitting
- **Documentation**: Update relevant documentation
- **Respect**: Follow our [Code of Conduct](CODE_OF_CONDUCT.md)

### Ideas for Contributions

- 📝 Add new analytical topics or case studies
- 🐛 Fix bugs or improve existing features
- 📚 Enhance documentation and examples
- 🎨 Improve UI/UX
- 🧪 Add unit tests
- 🌐 Add internationalization support

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 Moshe Shamouilian

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction...
```

---

## 🙏 Acknowledgments

- **Streamlit Team** - For creating an amazing framework for data apps
- **Open Source Community** - For the incredible libraries that power this project
- **Contributors** - Everyone who has helped improve this project
- **You** - For using and learning from this handbook!

---

## 📞 Contact & Support

- 📧 **Issues**: [GitHub Issues](https://github.com/Analytical-Guide/Product-Analytical-Apps/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/Analytical-Guide/Product-Analytical-Apps/discussions)
- ⭐ **Star this repo** if you find it helpful!

---

## 🗺️ Roadmap

### Upcoming Features

- [ ] Interactive quizzes and assessments
- [ ] More real-world case studies
- [ ] Video tutorials integration
- [ ] API for programmatic access
- [ ] Docker containerization
- [ ] Cloud deployment guides
- [ ] Multi-language support
- [ ] Mobile-responsive design enhancements

---

## 📊 Stats

![GitHub stars](https://img.shields.io/github/stars/Analytical-Guide/Product-Analytical-Apps?style=social)
![GitHub forks](https://img.shields.io/github/forks/Analytical-Guide/Product-Analytical-Apps?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/Analytical-Guide/Product-Analytical-Apps?style=social)

---

<div align="center">

**Made with ❤️ for the Product Analytics Community**

[⬆ Back to Top](#-product-analytics-handbook)

</div>
