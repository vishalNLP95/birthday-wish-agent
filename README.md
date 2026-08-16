# Birthday Wish Agent

This repository contains a Python project that generates personalized birthday emails with a short fun fact and sends them via SMTP using Azure OpenAI for content generation.

Repository structure
- src/                    Python package with modules
  - src/data_loader.py    Load Excel or Google Sheets
  - src/azure_openai.py   Azure OpenAI wrapper using the openai SDK (AzureOpenAI)
  - src/emailer.py        SMTP sending utilities and HTML renderer
  - src/templates/        HTML templates and theme variants
- data/                   sample input files and saved previews (ignored from git)
- scripts/                utility scripts to generate and send emails
- requirements.txt        Python dependencies
- example.env             Example environment variables (redacted)

Quick start
1. Copy `example.env` to `.env` and fill required variables (do not commit `.env`).
2. Create a virtualenv and install dependencies:
   python -m venv .venv
   .venv\Scripts\activate
   pip install -r requirements.txt
3. Run scripts/send_one_vishal.py to generate and send a sample email (ensure SMTP and Azure envs are set).

Security
- Secrets are redacted in `example.env`. Do NOT commit real credentials. Use environment variables or a secrets manager.

License: MIT

Co-authored-by: Copilot <223556219+Copilot@users.noreply.github.com>

