# ITPM Assignment 1 — Option 1 (Test Automation)

Automated test script using **Python + Playwright** and test data from an **Excel** sheet.

## Prerequisites
- **Python 3.11+**
- **pip**
  
### Install dependencies


##Open terminal inside VS Code:

Terminal → New Terminal

```bash
python -m pip install --upgrade pip
pip install playwright openpyxl
playwright install
```

## How to Run

### Run in VS Code (recommended)
1. Open this project folder in **Visual Studio Code**.
2. Open the integrated terminal: **Terminal → New Terminal**.
3. In the terminal, `cd` into the folder that contains `test_automation.py`.
4. Run one of the commands below depending on your terminal type.

### Example command in VS code
```Terminal
python test_automation.py --excel "test_automation/Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 20000 --retries 25 --retry-wait-ms 2500 --type-delay-ms 0 --slow-mo-ms 400 --save-every 1 --keep-open
```

### Example command (Windows PowerShell)


 1. Open PowerShell

Press Win + X → Click Windows PowerShell

 2. Go to your project folder

```pwershell
cd D:\test_automation
```

```powershell
python test_automation.py `
  --excel "Assignment 1 - Test cases.xlsx" `
  --url "https://www.pixelssuite.com/chat-translator" `
  --wait-ms 20000 `
  --retries 25 `
  --retry-wait-ms 2500
```

### Parameters (quick reference)
- `--excel` : Path to the Excel file containing test cases
- `--url` : Target URL to test
- `--wait-ms` : Wait time (milliseconds) for page actions/load
- `--retries` : Number of retry attempts
- `--retry-wait-ms` : Wait time (milliseconds) between retries

## Project Structure
- `test_automation.py` — main automation script
- `Assignment 1 - Test cases.xlsx` — test case definitions
- `IT23569522.xlsx` - If you want to check each test case's sinhala input covered and evidance

## Notes / Troubleshooting
- If Playwright browsers are missing, run:
  ```bash
  playwright install
  ```
- If you’re on macOS/Linux and `python` doesn’t work, use `python3`.
