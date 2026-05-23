# Bank Reconciliation System

A lightweight reconciliation system built with Python and SQLite for matching bank transactions from CSV and XML files through an interactive web dashboard.

---

# Features

- Upload and process CSV/XML transaction files
- Automated reconciliation engine
- SQLite database integration
- Web dashboard interface
- Mock sample data generation
- Verification scripts for testing
- Role-based seeded users

---

# Project Setup

## 1. Clone Project from GitHub

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd bhawana
```

---

## 2. Create Virtual Environment

```bash
python -m venv .venv
```

---

## 3. Activate Virtual Environment

### Windows PowerShell

```powershell
.venv\Scripts\Activate.ps1
```

### Windows Command Prompt (CMD)

```cmd
.venv\Scripts\activate.bat
```

---

## 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# Generate Sample Files

Run the following command to create mock CSV and XML files for testing:

```bash
python generate_mock_data.py
```

Generated files will be stored inside:

```text
sample_data/
```

---

# Initialize Database

Run the database initialization script:

```bash
python database.py
```

This will:

- Create SQLite database tables
- Seed default system users:
  - Admin
  - Finance
  - Read-Only

---

# Run Verification Scripts

## Verify CSV Reconciliation

```bash
python verify_reconciliation.py
```

## Verify XML Reconciliation

```bash
python verify_xml.py
```

---

# Launch Web Application

Start the Flask application server:

```bash
python app.py
```

---

# Open Application

After the server starts, open your browser and navigate to:

```text
http://127.0.0.1:5000
```

---

# Recommended Project Structure

```text
bhawana/
│
├── app.py
├── database.py
├── generate_mock_data.py
├── verify_reconciliation.py
├── verify_xml.py
├── requirements.txt
├── sample_data/
├── templates/
├── static/
└── .venv/
```

---

# Useful Commands

## Deactivate Virtual Environment

```bash
deactivate
```

---

# Notes

> [!IMPORTANT]
> Make sure Python is installed and added to your system PATH before running the project.

> [!TIP]
> Use PowerShell for smoother virtual environment activation on Windows.

---

# Tech Stack

- Python
- Flask
- SQLite
- HTML/CSS
- CSV/XML Processing

---

# License

This project is for educational and internal development purposes.
