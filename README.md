# Tent Hill Carrom Samaaj

Referee app for real-life carrom with friends. Track every board, fouls and the queen, and keep a running leaderboard.

**All data stays on the referee's phone.** Nothing is sent to any server.

## Install on Android (APK)

Every push to `main` builds the app automatically. Open the repo's **Releases**, download the latest `TentHillCarromSamaaj-*.apk` on your phone, and tap it to install.

## Use it in a browser instead

1. Open the app link on your phone (GitHub Pages, see below).
2. Chrome menu → **Add to Home screen** / **Install app**. It then opens like a normal app and works offline.
3. **Squad** tab: add everyone, and create teams of 2 if you play team matches.
4. **Match** tab: pick Singles, Doubles or Teams, choose who plays White and Black, tap **Start match**.
5. Every time a side pockets something, tap **Coin**, **Queen** or **Foul** under that side.
6. When the match ends, tap **Save to leaderboard**.

## Scoring

- Coin pocketed: +1. Queen pocketed: +3. Foul: −1.
- First side to the target (25 by default) wins, or tap **Finish match** any time.
- **Undo last tap** fixes a mis-tap.
- Leaderboard: 2 points per match win, ties broken by point difference. Separate Players and Teams tables.

## Edit, delete, reset

- **Squad** tab: **Edit** renames a player, or renames a team and changes its players. **Delete** removes one (tap twice). Old match history keeps their names.
- **Squad → Reset**: reset the leaderboard (deletes saved matches), delete all teams, or reset everything. Tap twice to confirm.

## Backup

Scores live in the phone browser's storage. Use **Squad → Save backup** now and then. **Restore backup** loads that file on any phone.

## Hosting on GitHub Pages

Repo → **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
The app will be at `https://<your-username>.github.io/<repo-name>/`.

## Files

- `index.html` – the whole app
- `android/` – Android wrapper, built by `.github/workflows/build-apk.yml`
- `sw.js` – offline support
- `manifest.webmanifest`, `icons/` – home-screen install
