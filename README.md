# 🐛 Automated Bug Report Generator — Python + openpyxl

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![openpyxl](https://img.shields.io/badge/openpyxl-3.x-green)
![Excel](https://img.shields.io/badge/Output-Excel-217346?logo=microsoft-excel)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

## 📌 Description

An automated bug reporting tool that analyzes test results, detects failures, and generates a **professional multi-sheet Excel report** with color-coded severity levels, KPI summary, and full bug details — all with automatic logging.

---

## 📊 Report Structure (3 Excel Sheets)

| Sheet | Content |
|-------|---------|
| 📊 Summary | KPIs (Total, Passed, Failed, Pass Rate) + results by module |
| 🧪 All Tests | Full test results with color-coded status (green/red) |
| 🐛 Bug Report | Detailed bug list with severity, title, steps, and recommendations |

---

## 🎯 Features

- ✅ Automatic bug detection from test results
- ✅ Severity classification (Critical / High / Medium / Low)
- ✅ Color-coded Excel report (professional formatting)
- ✅ Automatic logging to `logs/bug_report.log`
- ✅ Timestamped report filenames
- ✅ Recommendations for each bug

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **openpyxl** — Excel file generation & formatting
- **logging** — Automatic log file creation

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/fatimazahrary/qa-bug-report-generator.git
cd qa-bug-report-generator
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the generator
```bash
python bug_report_generator.py
```

### 4. Open the report
The Excel report is saved in the `reports/` folder with a timestamp:
```
reports/bug_report_20240315_143022.xlsx
```

---

## 📁 Project Structure

```
qa-bug-report-generator/
│
├── bug_report_generator.py   # Main script
├── requirements.txt          # Dependencies
├── README.md
│
├── reports/                  # Generated Excel reports (auto-created)
└── logs/                     # Log files (auto-created)
    └── bug_report.log
```

---

## 📋 Sample Log Output

```
2024-03-15 14:30:22 [INFO] BUG REPORT GENERATOR — Started
2024-03-15 14:30:22 [INFO] Total tests : 20 | Passed : 13 | Failed : 7 | Pass rate : 65.0%
2024-03-15 14:30:22 [WARNING] BUG-001 | [Critical] Login — Login button unresponsive when password is empty
2024-03-15 14:30:22 [WARNING] BUG-002 | [Critical] Login — No error shown for invalid email format
2024-03-15 14:30:22 [WARNING] BUG-003 | [Medium] Search — App crashes with special chars in search bar
2024-03-15 14:30:22 [INFO] ✅ Report saved : reports/bug_report_20240315_143022.xlsx
```

---

## 👩‍💻 Author

**Fatima Zahra RIYAD**  
Junior QA Engineer | Test Automation | Bug Reporting  
📧 [fatimazahrary.12@gmail.com]  
🔗 [linkedin.com/in/fatimazahrary]

---

## 📄 License

MIT License — free to use and modify.
