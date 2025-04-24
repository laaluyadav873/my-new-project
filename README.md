

# PhishNetAI - Real-Time AI-Powered Phishing Detection

Final project for the Building AI course

## Summary

PhishNetAI is an AI-powered system designed to detect and block phishing emails in real time using natural language processing (NLP) and anomaly detection. It protects users and organizations from cyber threats by identifying phishing attempts before they interact with harmful content.

## Background

Phishing is one of the most common and dangerous cyber threats today, where attackers impersonate trustworthy entities to steal sensitive information. Despite awareness, phishing attacks continue to bypass traditional spam filters, and human error remains a major factor.

This project solves the following problems:
* Difficulty in detecting sophisticated phishing emails
* Inadequate real-time phishing detection for everyday users
* A lack of tools for individuals to proactively avoid phishing scams

Motivation: 
* I've experienced phishing attacks firsthand, and I want to help mitigate the harm they cause to individuals and businesses.
* This project is important because phishing attacks are highly prevalent and can lead to significant financial and data security losses.

## How is it used?

PhishNetAI can be integrated as:
- A browser plugin or email client extension
- A cloud-based API for email providers or corporate security systems

### The process:
1. The user receives an email.
2. The model analyzes the email’s content, sender behavior, and embedded links.
3. A phishing risk score is calculated, and the email is flagged if deemed malicious.
4. The user is warned and given the option to take action.

**Target Users:**
* Everyday email users seeking enhanced protection from phishing emails.
* Companies and cybersecurity teams looking to safeguard their communication systems.
* Educational institutions wanting to train students on identifying phishing emails.

### Example Usage:
```python
def check_email(email):
    # process the email content
    phishing_score = model.predict(email.content)
    if phishing_score > threshold:
        print("Warning: This email is suspicious!")
    else:
        print("Safe: No phishing detected.")
