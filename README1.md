
# FedEx Tracking Number Generator Bot

## Overview
This Python bot automates the generation of FedEx tracking numbers using AI-powered serial estimation and checksum validation.  
It uses historical tracking data and a **Linear Regression** model to estimate future serial numbers, ensuring realistic and valid FedEx tracking number patterns.

The generated numbers are saved to a timestamped text file and automatically sent to a Telegram chat.

---

## Features
- Predicts next FedEx tracking serial numbers using **machine learning**.
- Generates valid tracking numbers with checksum logic.
- Saves generated numbers to a timestamped text file.
- Automatically sends the file to Telegram via Bot API.

---

## Requirements
- **Python 3.8+**
- Libraries:
  - pandas
  - numpy
  - requests
  - scikit-learn
- A Telegram Bot Token and Chat ID

Install dependencies:
```bash
pip install pandas numpy requests scikit-learn
```

---

## Configuration
1. Set the following values inside the script:
    ```python
    TELEGRAM_TOKEN = 'your_telegram_bot_token'
    CHAT_ID = 'your_chat_id'
    ACCOUNT_NUMBER = '320416272'
    TARGET_DATE = "2025-07-07"
    GENERATE_COUNT = 1000
    ```
2. Add your historical tracking numbers to `tracking_data` list.

---

## Usage
Run the script:
```bash
python fedex_tracking_generator.py
```
This will:
1. Predict serial numbers using machine learning.
2. Generate valid FedEx tracking numbers.
3. Save them into a timestamped text file.
4. Send the file automatically to your configured Telegram chat.

---

## Output
Example output file: `tracking_numbers_2025-07-26_14-30-00.txt`
```
FedEx Account Number: 320416272
Tracking Numbers Generated for Date: 2025-07-07
File Generated At: 2025-07-26_14-30-00
========================================
289282326015
289282329253
...
```

---

## Price
**One-time purchase price:** **$2000**  
Includes:
- Full bot script
- Documentation & setup assistance
- 1 month of basic support

---

## Disclaimer
This bot is for **educational and operational automation purposes only**. The author is not responsible for misuse or any violation of carrier terms.

---
