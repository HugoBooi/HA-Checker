# 🐒 Cobblemon HA Collection Checker

A fast, responsive web application designed for **Cobblemon** players to search any Pokémon, view its **Hidden Ability (HA)** and types, and check whether it is in your collection via live Google Sheets auto-sync.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-22272E?style=for-the-badge&logo=github&logoColor=white)

---

## ✨ Features

- **Live Google Sheets Auto-Sync:** Fetches your owned Pokémon automatically from a published Google Sheet CSV feed on load (with CORS proxy fallback).
- **Hidden Ability Lookup:** Uses PokéAPI to fetch official Hidden Abilities, types, and animated Gen 5 sprites from Pokémon Showdown.
- **Smart Form & Regional Variant Support:** Handles special regional variants (Alolan, Galarian, Hisuian, Paldean), gendered forms (`nidoran-f`, `nidoran-m`), and multi-form species (`wormadam`, `pumpkaboo`, `toxtricity`).
- **Manual Input Backup:** Fallback modal allows manual pasting of inventory lists if network restrictions prevent automatic Google Sheet fetches.

---

## 🚀 Live Demo

Check out the live webpage hosted on GitHub:
👉 **[Cobblemon HA Checker Live](https://hugobooi.github.io/HA-Checker/)**

---

## 📊 Setting Up Your Google Sheet

To connect your own Pokémon collection to the app:

1. Create a **Google Sheet**.
2. List your owned Pokémon in **Column A** (one entry per row, e.g., `chimchar`, `monferno`, `darmanitan-galar`).
3. Publish your sheet:
   - Click **File** $\rightarrow$ **Share** $\rightarrow$ **Publish to web**.
   - Change "Entire Document" to your specific sheet tab.
   - Select **Comma-separated values (.csv)**.
   - Click **Publish** and copy the URL.
4. Replace the `CSV_LINK` constant in `index.html`:

```javascript
const CSV_LINK = 'YOUR_PUBLISHED_CSV_LINK_HERE';
