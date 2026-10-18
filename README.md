# ⭐ Star Catcher

A small 3D browser game built with **Three.js** and published on **start.ng**.
Catch as many stars as you can in 30 seconds, as your own start.ng character.

🎮 **Play it:** https://star-catcher.start.ng
🎥 **Demo video:** <YOUR_VIDEO_LINK>

## How to play
- Move with the **arrow keys** or **W A S D** (on a phone, use the on-screen buttons).
- Touch the golden stars to collect them.
- You have **30 seconds**. Your score is the number of stars you caught.

## How it uses start.ng
- **Logged-in users:** the game asks start.ng who is playing. Signed-in players see their name, @account and face on a profile card. Their best score is saved to the start.ng leaderboard, and their own row is highlighted.
- **Guests:** players who are not signed in get start.ng's guest look and a **Sign in** button.
- **Leaderboard:** `startng.json` defines one column, "Stars caught". Scores are saved after each round and the top 10 players are shown.

## Central styling affects the character
The character is built in Three.js from the player's start.ng style fields, so it looks like their character on start.ng:

| start.ng field | What it changes in the game |
|---|---|
| `body` | male (trousers) or female (skirt) |
| `primaryColor` | shirt / top colour |
| `secondaryColor` | trousers, skirt, scarf and backpack colour |
| `skinColor` | skin colour |
| `hairColor` + `hair` | hair colour and style (short, afro, braids, bun, ponytail, dreads, bald) |
| `hat` | none, cap, beanie, top hat or crown |
| `accessory` | none, glasses, earrings, beard, scarf or backpack |

Changing the character on start.ng changes the hero in the game. Unknown or missing values fall back to a default look.

## Files
- `index.html`: the whole game (HTML, CSS and JavaScript, with Three.js loaded from jsDelivr)
- `startng.json`: leaderboard column definition
- `cover.png`: the game card picture on start.ng

## Built with
Three.js · plain JavaScript · start.ng connect page and HTTP API · GitHub

Made for the HNG Internship by **Harshita Sharma** ([@Harshita24-hack](https://github.com/Harshita24-hack)).
