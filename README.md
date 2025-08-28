# 🔄 Identity Lifecycle Automation

[![Python](https://img.shields.io/badge/Python-3.10+-blue)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)]()

Automates **onboarding/offboarding** of users into **Okta / Microsoft Entra ID** from HR data (CSV/API).

## ✨ What it does
- Creates/updates/deactivates accounts based on HR feed
- Assigns roles & groups
- Writes audit logs + CSV reports
- Dry-run mode to preview changes

## ⚙️ Quickstart
```bash
git clone https://github.com/mraaron360/identity-lifecycle-automation.git
cd identity-lifecycle-automation
pip install -r requirements.txt
cp .env.example .env     # fill in credentials
python onboard.py data/users.csv
python offboard.py data/terminated.csv
