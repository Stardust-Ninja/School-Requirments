# School-Requirements – Setup Guide

This project uses **Python + Flask** and a shared `requirements.txt` to ensure everyone runs the **same environment**, regardless of OS.

---

## 📦 Prerequisites

Make sure you have installed:

* **Python 3.9+**
* **pip** (comes with Python)
* **Git**

Check installation:

```bash
python --version
pip --version
git --version
```

---

## 🚀 First-time setup

### 1️⃣ Clone the repository

```bash
git clone <REPO_URL>
cd School-Requirements
```

---

### 2️⃣ Create a virtual environment

#### macOS

```bash
python3 -m venv venv
```

#### Windows (PowerShell)

```powershell
python -m venv venv
```

---

### 3️⃣ Activate the virtual environment

#### macOS

```bash
source venv/bin/activate
```

#### Windows (PowerShell)

```powershell
venv\Scripts\Activate.ps1
```

⚠️ If PowerShell blocks activation:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
```

Then activate again.

---

### 4️⃣ Install project dependencies

(Same command for macOS & Windows)

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the application

Depending on the project setup:

```bash
python app.py
```

or

```bash
flask run
```

---

## ✅ Verification

You should see:

* `(venv)` in your terminal
* No errors during installation
* The app running locally

---

## ❌ What NOT to do

* ❌ Do NOT install Flask globally
* ❌ Do NOT commit the `venv/` folder
* ❌ Do NOT skip activating the virtual environment

---

## 🧠 Notes for group work

* `requirements.txt` defines **exact dependencies**
* Only update it if you intentionally add or upgrade packages
* After updating dependencies:

```bash
pip freeze > requirements.txt
git commit -m "Update dependencies"
```

---

## 🧹 Troubleshooting

If something breaks:

```bash
deactivate
rm -rf venv
python -m venv venv
source venv/bin/activate  # or Windows equivalent
pip install -r requirements.txt
```

---

Happy coding 🚀

