# IT3040 – ITPM Assignment 1  
## Playwright Automation – Chat Sinhala Transliteration Testing

---

 Project Overview

This project automates testing of the Chat Sinhala Transliteration System available at:

https://www.pixelssuite.com/chat-translator

The automation framework executes test cases from an Excel file and automatically:

- Reads Singlish input test cases
- Sends input to the web application
- Captures actual Sinhala output
- Compares expected vs actual output
- Updates Excel file with:
  - Actual Output
  - Pass/Fail Status

---
 Technologies Used

- Python
- Playwright
- OpenPyXL (Excel automation)

---
prerequisites

Ensure Python 3.8 or above is installed.
Install Google Chrome (recommended) or let Playwright install Chromium


Installation Steps


pip install -U pip
pip install playwright openpyxl
playwright install



How to Run the Tests

Run the automation script using the following command:
python test_automation.py --excel "Assignment 1 - Test cases.xlsx" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open



Reopen the Excel file and verify whether the values automatically recorded under the ‘Actual
output’ and ‘Status(FAIL/PASS)’ columns are correct.
