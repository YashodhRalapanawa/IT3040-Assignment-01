# IT3040 - ITPM Assignment 1 - Option 1

**Repository:** [https://github.com/YashodhRalapanawa/IT3040-Assignment-01.git](https://github.com/YashodhRalapanawa/IT3040-Assignment-01.git)

## Assignment Title
Transliteration Accuracy Testing for Chat Sinhala
## Description
This project contains Playwright automation tests for the Chat Sinhala transliteration feature available at:
https://www.pixelssuite.com/chat-translator
The purpose of this assignment is to identify negative test cases where chat-style Singlish input is not correctly converted into Sinhala output.
## Test Scope
This project tests only the Chat Sinhala transliteration function.
Out of scope:
- Standard Sinhala transliteration
- Backend API testing
- Performance testing
- Security testing
- Scalability testing
## Files Included
- IT23757936_test_automation.py - Playwright automation script
- IT23757936_Test_cases.xlsx - Completed Excel file with 50 negative test cases and execution results
- IT23757936_requirements - Project dependencies
- IT23757936_README.md - Project instructions
## Requirements
- Python 3.11 or above
- Google Chrome
- Playwright
- openpyxl
## Installation Steps
python3 -m venv venv
source venv/bin/activate
python -m pip install --upgrade pip
python -m pip install playwright openpyxl
python -m playwright install
## How to Run the Automation
python IT23757936_test_automation.py --excel "IT23757936_Test_cases.xlsx" --sheet "Test Cases" --input-col "Input" --expected-col "Expected output" --actual-col "Actual output" --status-col "Status" --url "https://www.pixelssuite.com/chat-translator" --wait-ms 5000 --type-delay-ms 80 --slow-mo-ms 200 --save-every 1 --keep-open
## Notes
- The Excel file contains 50 negative test cases.
- The test cases cover all required Singlish input types.
- The Actual output and Status columns were generated using the Playwright automation script.
