# GladargUI: Midnight Master Importer

**GladargUI** is a lightweight, high-performance profile management hub designed for the *World of Warcraft: Midnight* expansion. It allows you to store, import, and share your UI configurations for **QUI**, **Plater**, **Details**, and **Blizzard Edit Mode** from a single centralized menu.

## 🚀 Features

- **One-Click Injection:** Programmatically imports profiles into supported addons, automatically overwriting old data to prevent duplicates.
- **Auto-Select Sharing:** Dedicated "Copy String" buttons that pop up a pre-selected text box for instant `Ctrl+C` sharing.
- **Smart Reload:** A specialized Reload UI button that automatically re-opens the GladargUI menu upon logging back in.
- **Status Tracking:** Tracks exactly when you last imported each profile, with green checkmarks for your current session.
- **Error Protection:** Built-in logic to detect missing addons or corrupted strings before they cause Lua errors.

## 🛠 Usage

1. **Open the Menu:** Type `/gladui` in the in-game chat.
2. **Importing:** Click the **"Import [Addon Name]"** button to push your pre-configured string into that addon.
3. **Sharing:** Click **"Copy String"** to grab your current string to share with friends or on Discord.
4. **Finalizing:** Click **"Reload UI & Re-Open"** to ensure all textures and fonts are correctly loaded.

## ⚙️ Development Workflow (VS Code & GitHub)

This addon is designed to be updated via **GitHub Actions**. 

- **To Update Strings:** Edit the `MY_STRINGS` table in `Core.lua` and update the `FILE_LAST_UPDATED` date.
- **To Release:** 1. Update the `## Version` in `GladargUI.toc`.
    2. Commit and push your changes to GitHub.
    3. Tag the release (e.g., `git tag v1.1` and `git push origin v1.1`).
    4. The GitHub Action will automatically package and upload the update to CurseForge.

## 📦 Dependencies

To use all features, the following addons must be installed and enabled:
- [QUI (Quazii UI Midnight)](https://www.curseforge.com/wow/addons/qui)
- [Plater Nameplates](https://www.curseforge.com/wow/addons/plater-nameplates)
- [Details! Damage Meter](https://www.curseforge.com/wow/addons/details)

---
*Created by Gladarg.*