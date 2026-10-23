# Palladium Melee Tracker for Owlbear Rodeo

Prototype v0.1.0. Free static hosting; no paid database required.

## Deploy using GitHub Pages
1. Create a **public** GitHub repository (e.g. `palladium-owlbear-tracker`).
2. Upload `index.html`, `manifest.json`, and `icon.svg` to the repository root.
3. In repository **Settings → Pages**, select **Deploy from a branch**, branch `main`, folder `/ (root)`, and Save.
4. Wait for your Pages site. Its URL should be `https://YOUR_USERNAME.github.io/palladium-owlbear-tracker/`.
5. In Owlbear Rodeo, install a custom extension using `https://YOUR_USERNAME.github.io/palladium-owlbear-tracker/manifest.json`.
6. Open the extension from the room toolbar. Have a second participant open it to test synchronization.

## Important
- The code is public on GitHub Pages, but live room data is held in Owlbear room metadata, not GitHub.
- All combatant HP/SDC/PPE/ISP in the tracker is shared with players. **Do not put secret enemy statistics in this prototype.**
- Only the GM can edit combat state. Any participant can send a public dice roll.
- Dice history is ephemeral and not restored when joining later.
- Room metadata has a 16 KB limit. This prototype keeps up to 25 log entries and rejects saves over approximately 14 KB.
- Concurrent writes from multiple GM sessions may conflict; use one GM editing session.
- This is a prototype; test with two browsers before using it in a live campaign.
- The original local HTML tracker remains unchanged.
