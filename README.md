# UMANG Accessibility Audit & Full-Stack Architecture

![Accessibility](https://img.shields.io/badge/Accessibility-90%2F100-brightgreen)
![Status](https://img.shields.io/badge/Status-Completed-success)
![Repository](https://img.shields.io/badge/Repository-Public-blue)

## 📌 Project Overview

This project presents an accessibility audit and full-stack
repository architecture for the UMANG public service website.

The website was evaluated using Microsoft Edge Lighthouse
and a manual keyboard-navigation review.

The goal is to identify accessibility issues, document
evidence, define remediation priorities, and create a
maintainable foundation for future full-stack development.

## 🌐 Audited Website

**Website:** UMANG Public Service Portal

**URL:** https://web.umang.gov.in/

## 📊 Lighthouse Results

| Category | Score |
|---|---:|
| Performance | 6/100 |
| Accessibility | 90/100 |
| Best Practices | 96/100 |
| SEO | 100/100 |

> Note: Lighthouse performance results may vary depending
> on browser state, stored data, network conditions and
> device performance.

## ♿ Accessibility Findings

Five important areas were documented:

1. **Missing accessible names**
   - Some buttons, links and menu items do not have accessible names.

2. **Positive tabindex values**
   - Some elements use tabindex values greater than 0.

3. **Incorrect heading order**
   - Heading elements are not arranged in a sequential hierarchy.

4. **Missing main landmark**
   - The document does not have a main landmark.

5. **Keyboard navigation review**
   - Keyboard-only navigation requires manual verification
     for logical focus order and visible focus.

## 🎯 Remediation Priority

| Priority | Issue | Severity |
|---|---|---|
| 1 | Missing accessible names | High |
| 2 | Positive tabindex values | High |
| 3 | Incorrect heading hierarchy | Medium |
| 4 | Missing main landmark | Medium |
| 5 | Keyboard navigation review | Medium |

## 🏗️ Repository Architecture

```text
UMANG-Accessibility-Audit/
│
├── client/
│   └── README.md
│
├── server/
│   └── README.md
│
├── docs/
│   ├── accessibility-audit.md
│   ├── architecture.md
│   └── screenshots/
│
├── tests/
│   └── README.md
│
├── README.md
└── .gitignore
🔧 Technology Stack
Frontend
React
JavaScript
HTML
CSS
Backend
Python
Flask
REST API
Testing & Audit
Microsoft Edge Lighthouse
Keyboard-only navigation testing
Accessibility testing
🔄 Application Architecture
                    ┌───────────────┐
                    │     User      │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │ Client / React│
                    └───────┬───────┘
                            │
                       HTTP / REST
                            │
                            ▼
                    ┌───────────────┐
                    │ Server / Flask│
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │   Database    │
                    └───────────────┘
📁 Documentation
Accessibility Audit
Architecture Documentation
Client architecture → client/README.md
Server architecture → server/README.md
Testing documentation → tests/README.md
📸 Audit Evidence

Screenshots captured during the Lighthouse audit are
included in the repository as supporting evidence.

The evidence includes accessibility findings related to:

Accessible names
Keyboard navigation
Heading structure
Main landmarks
Lighthouse results
🚀 Future Development

The repository can be extended with:

Accessible React components
Flask REST APIs
User authentication
Database integration
Automated accessibility testing
Keyboard navigation improvements
Responsive design
CI/CD integration
👨‍💻 Author

Shubham Suryakant Biradar

GitHub: @shubhambiradar1618

📄 Project Status

Audit: Completed
Architecture: Documented
Repository: Public
Accessibility Score: 90/100
