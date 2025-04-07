# CoinBrowser

**CoinBrowser** is a desktop application built with **Qt and C++** that serves as a companion tool for the **Freqtrade** crypto trading bot. It allows users to manage cryptocurrency pairs, simulate investments, and visualize virtual portfolios using real-time data fetched from the **CoinMarketCap API**.

---

## 🔧 Features

- 🔁 **Crypto Pair Management**  
  Write selected trading pairs to a `.txt` file for use with Freqtrade on specific exchanges.

- 📈 **Investment Simulator**  
  Simulate fictional crypto buys/sells and manage a virtual portfolio. Supports partial sell amounts in USD.

- 🗂 **Database Management**  
  Automatically creates and updates a local SQLite database (`coinhistory.db`) from JSON files, maintaining historical data in versioned tables.

- 🧩 **Freqtrade Integration**  
  Compatible with Freqtrade via raw pairs file generation from Docker output. Example: `raw_binance.txt`.

---

## ⚙️ Getting Started

1. **Setup Freqtrade Pairs File**  
   Run the following command and copy the table output to a text file:
   ```bash
   docker-compose run --rm freqtrade list-pairs --exchange binance
