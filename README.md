````markdown
# ============================================
# Clone Project from GitHub
# ============================================

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd bhawana
```

# ============================================
# Create Virtual Environment
# ============================================

```bash
python -m venv .venv
```

# ============================================
# Activate Virtual Environment
# ============================================

## Windows PowerShell

```powershell
.venv\Scripts\Activate.ps1
```

## Windows CMD

```cmd
.venv\Scripts\activate.bat
```

# ============================================
# Install Required Dependencies
# ============================================

```bash
pip install -r requirements.txt
```

# ============================================
# Generate Sample CSV & XML Files
# ============================================

```bash
python generate_mock_data.py
```

Generated files will be available inside:

```text
sample_data/
```

# ============================================
# Initialize & Seed SQLite Database
# ============================================

```bash
python database.py
```

This creates:

- Database tables
- Default users:
  - Admin
  - Finance
  - Read-Only

# ============================================
# Run Reconciliation Verification Tests
# ============================================

## Test CSV Reconciliation

```bash
python verify_reconciliation.py
```

## Test XML Reconciliation

```bash
python verify_xml.py
```

# ============================================
# Launch Web Application
# ============================================

```bash
python app.py
```

# ============================================
# Open Application in Browser
# ============================================

Navigate to:

```text
http://127.0.0.1:5000
```

# ============================================
# Recommended Project Structure
# ============================================

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

# ============================================
# Deactivate Virtual Environment (Optional)
# ============================================

```bash
deactivate
```
````
