# Security Policy

## 🔒 Reporting Security Vulnerabilities

We take the security of the Product Analytics Handbook seriously. If you discover a security vulnerability, please follow these steps:

### ⚠️ Please DO NOT:
- Open a public GitHub issue for security vulnerabilities
- Discuss the vulnerability in public forums or social media
- Exploit the vulnerability beyond what is necessary to demonstrate it

### ✅ Please DO:

1. **Report privately**: Email the maintainers or use GitHub's private vulnerability reporting feature
2. **Provide details**: Include as much information as possible:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if you have one)
   - Your contact information

### 🕐 Response Timeline

- **Initial Response**: Within 48 hours of receiving your report
- **Status Update**: Within 7 days with an initial assessment
- **Resolution**: We aim to address critical vulnerabilities within 30 days

### 🎖️ Recognition

We appreciate responsible disclosure and will:
- Acknowledge your contribution in our security advisories (unless you prefer to remain anonymous)
- Keep you informed of the progress toward resolving the issue
- Credit you in release notes when the fix is published (with your permission)

## 🛡️ Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| Latest  | ✅ Yes             |
| Older   | ⚠️ Best effort     |

We recommend always using the latest version of the application.

## 🔐 Security Best Practices for Users

When using the Product Analytics Handbook:

1. **Keep Dependencies Updated**
   - Regularly update Python packages: `pip install -r requirements.txt --upgrade`
   - Check for security updates: `pip list --outdated`

2. **Protect Sensitive Data**
   - Never commit API keys or credentials to the repository
   - Use environment variables for sensitive configuration
   - Use `.streamlit/secrets.toml` for local secrets (already in `.gitignore`)

3. **Data Upload Safety**
   - Be cautious when uploading sensitive data to the application
   - Remember that uploaded data is processed locally in your browser/server
   - Clear browser cache if you're concerned about data persistence

4. **Environment Security**
   - Use virtual environments to isolate dependencies
   - Review dependencies before installation
   - Keep Python and system packages up to date

## 🔍 Known Security Considerations

### Data Privacy
- This application processes data locally
- No data is sent to external servers (except when using specific APIs like FRED or yfinance)
- Users are responsible for ensuring compliance with their data protection requirements

### Third-Party Dependencies
- We use reputable, well-maintained packages
- Dependencies are specified in `requirements.txt`
- We recommend reviewing security advisories for:
  - Streamlit
  - Pandas
  - NumPy
  - Scikit-learn
  - Other data science libraries

### API Usage
Some features use external APIs:
- **FRED API**: Economic data from Federal Reserve Economic Data
- **yfinance**: Financial data from Yahoo Finance

Users should:
- Review the terms of service for these APIs
- Use their own API keys when required
- Be aware of rate limits and usage policies

## 🚨 Security Updates

We will:
- Monitor dependencies for known vulnerabilities
- Update dependencies when security patches are released
- Announce security updates in release notes
- Use GitHub Security Advisories for critical issues

## 📚 Additional Resources

- [GitHub Security Best Practices](https://docs.github.com/en/code-security)
- [Python Security Guidelines](https://python.readthedocs.io/en/stable/library/security_warnings.html)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)

## 📧 Contact

For security-related inquiries that are not vulnerabilities, please open a discussion on GitHub or contact the maintainers through the repository.

---

**Thank you for helping keep Product Analytics Handbook and our users safe! 🙏**
