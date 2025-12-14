# 🩸 The Grimoire: Dark Edition

**The Arcane MTG Collection and Ritual (Deck) Tracker**

The Grimoire provides a dark, cohesive interface for tracking relic acquisitions, calculating portfolio value, and performing deep statistical analysis on your potent Rituals (decks).

This is the public repository showcasing the **client-side HTML, CSS, and JavaScript structure** of the application interface. The live application utilizes a proprietary, protected backend infrastructure based on Supabase and PostgreSQL.

## 🔗 Access the Live Grimoire

You can access and use the live application here:

**https://wmmalwareresearch.github.io/mtg-tracker-client/**

---

## 🌟 Arcane Features

* **Dark Grimoire Theme:** A custom, immersive UI featuring deep violet, crimson, and black hues.
* **Relic Vault (Collection Tracking):** Quickly add cards and their acquisition costs using fuzzy search powered by Scryfall.
* **Portfolio Analysis:** Track the total count, acquisition cost, current market value, and Arcane Gain/Loss (Profit/Loss).
* **Intelligent Ritual Analysis:** Paste a decklist into the editor to instantly view the full list, generating visualizations for:
    * **Mana Value (CMC) Curve**
    * **Card Type Breakdown**
    * **Card Name Validation** (Identifies typos using Scryfall's bulk API).
* **Seamless Workspace:** Integrated editing, validation, and analytics all within a single, dynamic Rituals tab.

## ⚙️ Technology Stack

* **Front-end:** HTML5, CSS3, Vanilla JavaScript (for speed and portability).
* **Key Libraries:** Supabase Client Library, Chart.js.
* **External APIs:** Scryfall API (for card metadata and bulk validation).
* **Backend (Proprietary):** Supabase (PostgreSQL, Authentication, Realtime).

## ⚠️ Note on Source Code

This repository contains only the front-end code required to display the UI. The proprietary backend configuration, API keys, and server deployment scripts are **not included**.

## 🔒 Licensing

**All Rights Reserved.**

This software is **Proprietary**. You may not copy, distribute, or modify this code without the express written permission of the author.

---
*Created by [wmmalwareresearch]*
