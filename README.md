# MOEX Data Loader
Asynchronous Python module for downloading historical price data from the Moscow Exchange (MOEX) API. Returns data as a ready-to-use Pandas DataFrame with a datetime index.

## Features
- Asynchronous data loading using aiohttp
- Historical data from the MOEX ISS API
- Automatic ticker normalization
- Validation of API responses
- Ready-to-use pandas.DataFrame

## Project Structure
moex-data-loader/
├── notebooks/
├── src/
│   └── loader.py
├── requirements.txt
└── README.md

## Installation
git clone ...
cd moex-data-loader

pip install -r requirements.txt

## Requirementz
aiohttp==3.11.10
aiomoex==2.1.2
pandas==2.3.2

## Usage
from src.loader import load_history

df = await load_history("GAZP")

print(df.head())