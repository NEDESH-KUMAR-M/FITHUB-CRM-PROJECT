<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=160&section=header&text=WorkForce%20Manager&fontSize=42&fontColor=ffffff&fontAlignY=38&desc=Employee%20Management%20System&descAlignY=58&descSize=16&descColor=a78bfa" width="100%"/>

[![Python](https://img.shields.io/badge/Python-3.10+-3b4cc0?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Flask](https://img.shields.io/badge/Flask-2.x-black?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com)
[![Google Sheets](https://img.shields.io/badge/Google_Sheets-DB-34a853?style=for-the-badge&logo=googlesheets&logoColor=white)](https://developers.google.com)
[![Google Drive](https://img.shields.io/badge/Google_Drive-Storage-4285f4?style=for-the-badge&logo=googledrive&logoColor=white)](https://developers.google.com)
[![2FA](https://img.shields.io/badge/2FA-TOTP-f97316?style=for-the-badge&logo=authy&logoColor=white)](https://pyauth.github.io/pyotp)
[![Vercel](https://img.shields.io/badge/Deployed-Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://work-force-manager.vercel.app)

<br/>

> **A full-stack HR platform** — manage employees, track time, handle leaves,
> upload payslips, and secure everything with 2FA.
> Powered by Google Sheets as the database. No SQL needed.


[⭐ &nbsp;Star](https://github.com/NEDESH-KUMAR-M/WORK-FORCE-MANAGER/stargazers)

</div>



---

## 🧩 &nbsp;What's Inside



### 🔐 &nbsp;Authentication & Security

- Email + password login with **role-based access** — Admin and Employee
- **Two-factor authentication** via Google Authenticator (TOTP using `pyotp`)
- QR code generation for first-time 2FA device setup
- Session-based route protection — `@login_required` and `@admin_required` decorators

<br/>

### 📊 &nbsp;Admin Dashboard

- Live HR stats — total employees, new joinings, pending leaves, project completions
- Full employee directory with **add, update, block, and delete** controls
- Duplicate employee ID and email validation on registration

<br/>

### 👥 &nbsp;Employee Management

- Register employees with complete details — name, ID, designation, department, joining date, salary, and role
- **Block / unblock** employees without permanent deletion
- View and manage all records in a clean structured table

<br/>

### 🏖️ &nbsp;Leave Management

- Employees apply for leave with date range, leave type, and reason
- **Auto-calculates total days** for every request
- Admins approve or reject in real time — status written back to Google Sheets instantly

<br/>

### ⏱️ &nbsp;Timesheet & Project Tracking

- Admins assign projects to specific employees with deadlines
- Employees **start and complete tasks** with live time capture
- Hours auto-calculated from start → end timestamps
- Tasks split into three states — `Not Started` · `In Progress` · `Completed`

<br/>

### 🧾 &nbsp;Payslip Management

- Employees request payslips by selecting month and year
- Admins **upload PDF payslips** directly to Google Drive
- Public download links auto-generated and stored back in Sheets
- Pending and fulfilled requests tracked separately

<br/>

### 📅 &nbsp;Holiday Management

- Admins add, edit, and delete public holidays
- Holiday calendar visible to all employees
- Full REST API — `GET` · `POST` · `PUT` · `DELETE`

<br/>

---

## ⚙️ &nbsp;Tech Stack

```yaml
Backend:     Flask (Python 3.10+)
Frontend:    HTML · CSS · JavaScript
Database:    Google Sheets  (via gspread)
File Store:  Google Drive API v3
Auth:        Google OAuth2 · pyotp (TOTP)
Deployment:  Vercel
Lines:       819 (app.py)
```

<br/>

---

## 📁 &nbsp;Project Structure

```
WORK-FORCE-MANAGER/
│
├── 📄 app.py              # Core — all routes, APIs, business logic (819 lines)
├── 📁 front/              # Frontend — HTML templates, CSS, JavaScript
├── 🔑 credentials.json    # Google Service Account key (not committed)
├── 📋 .gitignore
└── 📖 README.md
```

<br/>

---

## 🚀 &nbsp;Quick Start

```bash
# 1 · Clone
git clone https://github.com/NEDESH-KUMAR-M/WORK-FORCE-MANAGER.git
cd WORK-FORCE-MANAGER

# 2 · Install dependencies
pip install -r requirements.txt

# 3 · Add Google Service Account key
# Place credentials.json in the root directory

# 4 · Run
python app.py
# → http://localhost:2000
```

<br/>

---

## 📄 &nbsp;License

MIT © [Nedesh Kumar M](https://github.com/NEDESH-KUMAR-M)

<br/>

---

<div align="center">

### Built by

**Nedesh Kumar M**

[![GitHub](https://img.shields.io/badge/GitHub-NEDESH--KUMAR--M-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/NEDESH-KUMAR-M)

<br/>

*Found this useful? A ⭐ goes a long way.*

[![Star](https://img.shields.io/github/stars/NEDESH-KUMAR-M/WORK-FORCE-MANAGER?style=social)](https://github.com/NEDESH-KUMAR-M/WORK-FORCE-MANAGER/stargazers)

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f0c29,50:302b63,100:24243e&height=100&section=footer" width="100%"/>

</div>
