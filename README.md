# ============================================
# Clone Project from GitHub
# ============================================

git clone <YOUR_GITHUB_REPOSITORY_URL>
cd bhawana

# ============================================
# Create Virtual Environment
# ============================================

python -m venv .venv

# ============================================
# Activate Virtual Environment
# ============================================

# Windows PowerShell
.venv\Scripts\Activate.ps1

# Windows CMD
# .venv\Scripts\activate.bat

# ============================================
# Install Required Dependencies
# ============================================

pip install -r requirements.txt

# ============================================
# Generate Sample CSV & XML Files
# ============================================

python generate_mock_data.py

# Generated files will be available inside:
# sample_data/

# ============================================
# Initialize & Seed SQLite Database
# ============================================

python database.py

# This creates:
# - Database tables
# - Default users:
#   1. Admin
#   2. Finance
#   3. Read-Only

# ============================================
# Run Reconciliation Verification Tests
# ============================================

# Test CSV reconciliation engine
python verify_reconciliation.py

# Test XML reconciliation engine
python verify_xml.py

# ============================================
# Launch Web Application
# ============================================

python app.py

# ============================================
# Open Application in Browser
# ============================================

# Navigate to:
# http://127.0.0.1:5000

# ============================================
# Recommended Project Structure
# ============================================

# bhawana/
# ├── app.py
# ├── database.py
# ├── generate_mock_data.py
# ├── verify_reconciliation.py
# ├── verify_xml.py
# ├── requirements.txt
# ├── sample_data/
# ├── templates/
# ├── static/
# └── .venv/

# ============================================
# Deactivate Virtual Environment (Optional)
# ============================================

deactivate
