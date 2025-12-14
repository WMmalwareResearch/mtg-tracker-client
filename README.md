# 🔮 MTG Manager (Hybrid)

A serverless, browser-based Magic: The Gathering collection manager that gives you full control over your data.

**Live App:** [Launch MTG Manager](https://wmmalwareresearch.github.io/mtg-tracker-client/)

![Version](https://img.shields.io/badge/version-2.0-blueviolet) ![Status](https://img.shields.io/badge/status-stable-success)

## 🌟 Features

* **☁️ Hybrid Architecture:** Frontend hosted on GitHub, Backend on your own Google Sheet.
* **💸 Real-Time Pricing:** Fetches live prices via Scryfall API.
* **📊 Analytics:** Interactive charts for Color Wheel, Rarity, and Financial Value.
* **📋 Deck Check:** Paste a decklist to see exactly which cards you own and which you need to buy.
* **📂 Bulk Tools:** Import/Export CSVs compatible with Moxfield/Archidekt.
* **🔒 Private & Secure:** Your data lives in *your* Google Drive. No external database.

---

## 🚀 Quick Start Guide

This app uses a **"Bring Your Own Backend"** model. You host the website (or use the link above), but you connect it to your own personal Google Sheet database.

### Step 1: Get the Database
1.  **[Click here to make a Copy of the Backend Sheet](LINK_TO_YOUR_BLANK_SHEET)** *(Replace this text with the actual link to your Google Sheet)*
    * *Note: Ensure the script code in `Extensions > Apps Script` is the V37.0 version.*

### Step 2: Deploy the API
1.  Inside your new Google Sheet, go to **Extensions** $\rightarrow$ **Apps Script**.
2.  Click the blue **Deploy** button (top right) $\rightarrow$ **New Deployment**.
3.  **Select type:** Click the Gear icon ⚙️ $\rightarrow$ **Web App**.
4.  **Configuration:**
    * **Description:** `MTG Tracker`
    * **Execute as:** `Me` (Your email)
    * **Who has access:** `Anyone` (Crucial for the app to talk to the sheet).
5.  Click **Deploy**.
6.  **Copy** the `Web App URL` (It starts with `https://script.google.com/...`).

### Step 3: Connect
1.  Open the [Live App](https://wmmalwareresearch.github.io/mtg-tracker-client/).
2.  Paste your **Web App URL** into the setup box.
3.  Click **Connect**.

**You're done!** You can now manage your collection. The app will remember your database for next time.

---

## 🛠️ For Developers

If you want to modify the frontend code or host your own version:

1.  **Fork** this repository.
2.  Edit `index.html` to change features or styles.
3.  Enable **GitHub Pages** in your repository settings (`Settings > Pages > Branch: main`).

### Tech Stack
* **Frontend:** Vanilla HTML5, CSS3, JavaScript.
* **Libraries:** Chart.js (Analytics), PapaParse (CSV).
* **Backend:** Google Apps Script (Serverless Node.js-like environment).
* **API:** Scryfall API (Card Data).

---

## ⚠️ Limitations & Quotas
Since this runs on free Google infrastructure:
* **Batch Limit:** Bulk imports are processed in chunks of 10 to prevent timeouts.
* **Execution Time:** Google Scripts timeout after 6 minutes. Large imports may take time.
* **Rate Limits:** Please be respectful of Scryfall's API limits when refreshing prices.

---

*Built with 🔮 by WM Malware Research*
