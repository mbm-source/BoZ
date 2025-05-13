# Bank of Zambia Data Pipeline

A Python-based data pipeline that scrapes, downloads, and stores exchange rate and payment systems data from the official [Bank of Zambia](https://www.boz.zm/) website. Designed to automate data collection for use in analytics and Power BI dashboards.

---

## Features

- Scrapes daily ZMW/USD exchange rates from `https://www.boz.zm/`
- Downloads historical Payment Systems Statistics `.xlsx` reports
- Cleans and saves data to CSV files in a structured directory
- Logs all actions and errors to `.txt` log files
- Cron-compatible for daily automation on macOS
- Power BI-ready CSV outputs - COMING SOON

---

## 📂 Project Structure

BoZ/
├── boz_scraper.py # Scrapes daily exchange rates
├── boz_payment_systems_downloader.py # Downloads payment systems .xlsx files
├── logs/
│ ├── boz_cron_log.txt
│ └── payment_systems_log.txt
├── data/
│ ├── boz_usd_rates_YYYYMMDD.csv
│ └── payment_systems/ # Downloaded .xlsx files
├── LICENSE
├── README.md
└── .gitignore
