# Amazon Price Tracker

Tracks the price of an Amazon product and sends you an email alert when it drops below your target price.

## Features

- Scrapes the current price and product title from an Amazon product page
- Compares the price against a target buy price
- Sends an email alert via SMTP when the price drops below the target

## Setup

1. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

2. Set up your credentials in a `.env` file (or environment variables):

   ```
   SMTP_ADDRESS=smtp.gmail.com
   EMAIL_ADDRESS=your@gmail.com
   EMAIL_PASSWORD=your-app-password
   ```

3. Update the `url` and `BUY_PRICE` in `main.py`, then run:

   ```bash
   python main.py
   ```

## Requirements

```
beautifulsoup4==4.12.3
requests==2.32.3
python-dotenv==1.0.1
```