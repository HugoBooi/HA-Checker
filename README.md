# 🐒 Cobblemon HA Collection Checker

A fast, responsive web application designed for **Cobblemon** players to search any Pokémon, view its **Hidden Ability (HA)** and types, and check whether it is in your collection via live Google Sheets auto-sync.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-22272E?style=for-the-badge&logo=github&logoColor=white)

---

## ✨ Features

- **Real-Time Google Sheet Syncing** Automatically fetches, parses, and updates inventory from a published Google Sheet CSV output.
- **Hidden Ability Lookup:** Uses PokéAPI to fetch official Hidden Abilities, types, and animated Gen 5 sprites from Pokémon Showdown.
- **Smart Autocomplete Suggestions** Pre-fetches PokéAPI species and form names on load to provide real-time top 5 search-engine-style suggestions as you type.
- **Direct Sheet Access** Features a centered shortcut button allowing players to open and browse the complete Google Sheet in a new tab.

---

## 💡 How Search Queries Work

- Multi-word names use hyphens: `iron-hands`, `tapu-koko`, `great-tusk`.
- Regional forms use region suffixes: `vulpix-alola`, `meowth-galar`, `growlithe-hisui`, `wooper-paldea`.
- Shorthand aliases like `darmanitan-galar` or `tauros-paldea` map directly to PokéAPI's default variety endpoints while checking exact ownership status in your sheet.

---

## 🚀 Live Demo

Check out the live webpage hosted on GitHub:
👉 **[Cobblemon HA Checker Live](https://hugobooi.github.io/HA-Checker/)**

---
