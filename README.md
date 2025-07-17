# 🔐 Password Strength Analyzer (Streamlit)

A web-based tool to analyze password strength using rule-based validation, entropy scoring, and real-world breach check via HaveIBeenPwned API.

## 📌 Features

- 🔍 Password strength score (zxcvbn)
- ✅ 9 Rule-based validations (length, character types, patterns)
- 🛡️ Real-time breach check via HaveIBeenPwned
- 🌐 Clean browser UI using Streamlit
- 🔒 Fully privacy-safe — no password stored or sent

---

## 📊 Rule-Based Checks (R1 to R9)

| Rule ID | Description                                      |
|---------|--------------------------------------------------|
| R1      | Minimum 8 characters                             |
| R2      | At least one uppercase letter                    |
| R3      | At least one lowercase letter                    |
| R4      | At least one digit                               |
| R5      | At least one special character (@#$%^&*)         |
| R6      | Avoid common patterns like '123', 'qwerty', etc. |
| R7      | Avoid repeated characters like 'aaa', '111'      |
| R8      | Avoid sequential patterns like 'abcd', '1234'    |
| R9      | Don't include your name/email in password        |



## 🚀 How to Run

pip install streamlit zxcvbn requests
streamlit run main.py

App will launch at: http://localhost:8501


## 📈 Sample Output

**Input:** `Dragon#9876`

- Strength: **91.11%**
- Breach: ✅ Not found in public breaches
- Suggestions: Avoid sequential characters like `1234`, `abcd`



# 📦 Tech Stack
Python 🐍

Streamlit 🌐

zxcvbn 🔐

Regex (re) for rule checks

HaveIBeenPwned API 🌍


# 🔮 Future Plans
Add password generator tab

Export to PDF or JSON

Deploy on Streamlit Cloud / Vercel

Add dark mode

