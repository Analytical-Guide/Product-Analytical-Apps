# Usage Guide

Welcome to the Product Analytics Handbook! This guide will help you get the most out of this interactive learning platform.

## Table of Contents

1. [Getting Started](#getting-started)
2. [Navigation](#navigation)
3. [Learning Paths](#learning-paths)
4. [Interactive Features](#interactive-features)
5. [Working with Data](#working-with-data)
6. [Tips and Tricks](#tips-and-tricks)

---

## Getting Started

### First Launch

When you first run the application:

```bash
streamlit run streamlit_app/Product_Analytics/main.py
```

You'll see the home page with an overview of all available topics.

### Interface Overview

The application has three main areas:

1. **Sidebar** (left): Navigation menu with all topics
2. **Main Content** (center): Lessons, visualizations, and interactive elements
3. **Settings** (top-right): App settings and options

---

## Navigation

### Sidebar Menu

The sidebar contains all available topics organized by category:

- **1.x - Fundamentals**: Core concepts and foundations
- **3.x - Applications**: Real-world use cases
- **Features**: Advanced topics and specialized analysis

### Topic Organization

Topics are numbered for suggested learning order:
- **1 1** - Probability Fundamentals
- **1 2** - Descriptive Statistics
- **1 3** - Data Visualization
- And so on...

### Quick Navigation

- Click any topic in the sidebar to jump to it
- Use your browser's back/forward buttons
- Bookmark specific pages for quick access

---

## Learning Paths

### For Beginners

**Recommended sequence:**

1. **Probability Fundamentals** - Start here to understand the basics
2. **Descriptive Statistics** - Learn to summarize and describe data
3. **Data Visualization** - Understand how to present data visually
4. **Data Quality** - Learn about ensuring data accuracy
5. **Metrics Fundamentals** - Understand KPIs and metrics

### For Intermediate Users

Skip to these advanced topics:

1. **Hypothesis Testing** - Statistical inference
2. **A/B Testing** - Controlled experiments
3. **Time Series Analysis** - Temporal data analysis
4. **Survival Analysis** - Time-to-event analysis

### For Specific Applications

Choose based on your interest:

- **Product Analytics** → Start with Churn Analysis
- **Marketing** → Marketing Analytics
- **Risk Management** → Fraud Risk Analytics
- **Operations** → Supply Chain Analysis
- **Finance** → Economic Demand Forecasting

---

## Interactive Features

### Data Upload

Many sections allow you to upload your own data:

1. Look for the **"Upload CSV"** button
2. Select a CSV file from your computer
3. The app will analyze and visualize your data

**Supported formats:**
- CSV files with headers
- Numeric and categorical columns
- Missing values are handled automatically

### Interactive Visualizations

Each visualization is interactive:

- **Hover** over data points for details
- **Zoom** in/out on charts (Plotly charts)
- **Pan** across large datasets
- **Download** charts as images

### Parameter Adjustment

Many examples let you adjust parameters:

- Use **sliders** to change numeric values
- Use **dropdowns** to select options
- Use **checkboxes** for toggles
- See results update in real-time

### Code Examples

Code sections show you how things work:

- **With explanations**: Learn the theory
- **With code**: See the implementation
- **Try it yourself**: Modify parameters

---

## Working with Data

### Sample Datasets

Many topics include built-in sample datasets:

- **Economic data** (via FRED API)
- **Financial data** (via yfinance)
- **Synthetic data** for demonstrations

### Using Your Own Data

To analyze your own data:

1. **Prepare your CSV file**:
   - Include column headers
   - Use consistent formatting
   - Clean obvious errors

2. **Upload via the interface**:
   - Click "Browse files" or drag-and-drop
   - Select your CSV file
   - Wait for processing

3. **Explore the results**:
   - View summary statistics
   - See automatic visualizations
   - Adjust parameters as needed

### Data Privacy

⚠️ **Important**: 
- Data uploaded is processed locally in your browser/server
- No data is sent to external servers (except for API features)
- Sensitive data should be anonymized before upload
- Clear browser cache if concerned about data retention

---

## Tips and Tricks

### Maximize Learning

1. **Follow the sequence**: Topics build on each other
2. **Try examples**: Don't just read - interact!
3. **Upload your data**: Apply concepts to real problems
4. **Take notes**: Document insights and learnings
5. **Experiment**: Change parameters and see what happens

### Performance Tips

1. **Use smaller datasets**: For initial exploration (< 100K rows)
2. **Close unused tabs**: If the app feels slow
3. **Clear cache**: In Streamlit settings if needed
4. **Restart app**: If you encounter issues

### Keyboard Shortcuts

- **`C`**: Toggle sidebar (in some browsers)
- **`R`**: Rerun the application
- **`Ctrl/Cmd + Enter`**: In code cells

### Bookmarking Pages

Save your favorite pages:
1. Navigate to the page
2. Bookmark the URL
3. Return directly to that topic later

### Sharing Insights

To share what you've learned:
1. Take screenshots of visualizations
2. Download charts as images
3. Export results to CSV (where available)
4. Share links to specific pages

---

## Common Workflows

### Exploratory Data Analysis

```
1. Upload your dataset
2. Start with Descriptive Statistics
3. Move to Data Visualization
4. Check Data Quality
5. Define relevant Metrics
```

### Hypothesis Testing

```
1. Review Probability Fundamentals
2. Study Hypothesis Testing theory
3. Try A/B Testing examples
4. Apply to your data
5. Interpret results
```

### Predictive Analysis

```
1. Load time series data
2. Explore Time Series Analysis
3. Try Economic Forecasting
4. Build your own models
5. Validate predictions
```

### Customer Analytics

```
1. Start with Churn Analysis
2. Explore Survival Analysis
3. Review Marketing Analytics
4. Apply to customer data
5. Create actionable insights
```

---

## Troubleshooting

### Application Issues

**Page won't load:**
- Check console for errors
- Refresh the page
- Restart the Streamlit server

**Data upload fails:**
- Check file format (must be CSV)
- Verify file size (< 200MB default)
- Ensure proper encoding (UTF-8)

**Charts not displaying:**
- Enable JavaScript in browser
- Check browser compatibility
- Try a different browser

**Slow performance:**
- Reduce dataset size
- Close other applications
- Check system resources

### Getting Help

1. **Check documentation**: Start here
2. **Review error messages**: Often self-explanatory
3. **Search issues**: On GitHub
4. **Ask for help**: Open a new issue
5. **Join discussions**: Community support

---

## Best Practices

### Learning Strategy

- ✅ Start with fundamentals
- ✅ Practice with examples
- ✅ Use your own data
- ✅ Take breaks between topics
- ✅ Review and revise

### Data Management

- ✅ Keep data files organized
- ✅ Document data sources
- ✅ Validate data quality
- ✅ Backup important files
- ✅ Respect data privacy

### Analysis Approach

- ✅ Define clear objectives
- ✅ Understand your data
- ✅ Choose appropriate methods
- ✅ Validate assumptions
- ✅ Interpret results carefully

---

## Advanced Features

### API Integration

Some features use external APIs:

**FRED API (Economic data):**
- Free API key required
- Set in `.streamlit/secrets.toml`
- See documentation for setup

**yfinance (Financial data):**
- No API key needed
- Rate limits may apply
- Use responsibly

### Custom Configuration

Customize the app experience:

**Create `.streamlit/config.toml`:**
```toml
[theme]
primaryColor = "#your-color"
backgroundColor = "#ffffff"

[server]
port = 8501
maxUploadSize = 200
```

---

## Additional Resources

### Within the App

- 📝 **Feedback page**: Share your thoughts
- 💡 **Interactive demos**: In each section
- 📊 **Sample datasets**: Pre-loaded examples

### External Resources

- 📖 [Streamlit Documentation](https://docs.streamlit.io/)
- 📚 [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/)
- 🎓 [Statistics Resources](https://www.khanacademy.org/math/statistics-probability)

---

## Next Steps

After mastering the basics:

1. **Contribute**: Share your knowledge ([CONTRIBUTING.md](../CONTRIBUTING.md))
2. **Share**: Tell others about this resource
3. **Apply**: Use these skills in real projects
4. **Expand**: Explore related topics and tools

---

**Happy Learning! 📊**

For more information, see:
- [Installation Guide](INSTALLATION.md)
- [Contributing Guidelines](../CONTRIBUTING.md)
- [GitHub Repository](https://github.com/Analytical-Guide/Product-Analytical-Apps)
