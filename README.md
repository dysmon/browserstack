# Robot Framework Tests on BrowserStack

This repository contains end-to-end UI tests for the [ParaBank](https://parabank.parasoft.com/parabank/index.htm) application using [Robot Framework](https://robotframework.org/) and [BrowserStack](https://www.browserstack.com/). The tests run on multiple browsers (Chrome, Firefox, Safari) via BrowserStack's cloud infrastructure.

## 📁 Project Structure

```
.
├── browserstack_config.py     # Configures BrowserStack remote options
├── requirements.txt           # Dependencies
├── run_tests.py               # Runs tests across multiple browsers
├── test_description.txt       # Description of test cases
├── tests.robot                # Robot Framework test suite
├── .gitignore                 # Git ignored files
└── results/                   # Test logs and reports (auto-generated)
```

## ✅ Test Cases

### 1. Successful Account Login
Verifies that a user can log in with valid credentials.

### 2. Balance Check
Verifies that the account balance is correctly displayed after login.

Details can be found in `test_description.txt`.

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2. Install Dependencies

It is recommended to use a virtual environment.

```bash
python -m venv .venv
source .venv/bin/activate  # on Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

### 3. Configure BrowserStack Credentials

Edit `browserstack_config.py` and replace:
```python
USERNAME = 'your_username_from_browserstack'
ACCESS_KEY = 'your_access_key_from_browserstack'
```

### 4. Run Tests

```bash
python run_tests.py
```

Test results (logs and reports) will be saved in the `results/` directory under subfolders for each browser.

## 🧪 Technologies Used

- Robot Framework
- SeleniumLibrary
- BrowserStack Automate
- Python

## 📋 Notes

- Tests run remotely on BrowserStack using Chrome, Firefox, and Safari on macOS Ventura.
- If a test fails, a screenshot is captured automatically.
- Logs and reports are named per browser and saved in organized folders.

## 📂 .gitignore

The following are excluded from version control:
```
__pycache__/
.venv/
.idea/
results/
```

Happy Testing! 🎯
