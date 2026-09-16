# Security Policy

## Supported Versions

DOJO is currently in active early-stage development. Security updates apply to the latest version only.

| Version | Supported          |
| ------- | ------------------ |
| 0.x.x   | :white_check_mark: |

## Reporting a Vulnerability

If you find a security vulnerability in DOJO, please report it privately rather than opening a public issue.

- **Where to report:** Open a private security advisory on GitHub, or contact the maintainer directly
- **Response time:** You can expect an initial response within 5 business days
- **What to expect:**
  - If the vulnerability is confirmed, a fix will be prioritized and you'll be updated on progress until it's resolved
  - If it's declined (e.g. not reproducible, out of scope), you'll get an explanation why

Please don't disclose the issue publicly until it's been addressed.

## Notes for This Project

- Secrets (Groq API key, Supabase key) are stored as environment variables and never committed to the repo
- Photo verification uses live camera capture only — no file uploads — to reduce risk of spoofed or malicious image submissions
- All external API calls (Groq, Supabase) are wrapped in try/except with logging, and rate-limited via Flask-Limiter
