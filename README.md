# Tent Hill Carrom Samaaj

Referee app for real-life carrom with friends. Track every board, fouls and the queen, and keep a running leaderboard.

**All data stays on the referee's phone.** Nothing is sent to any server.

## Use it

1. Open the app link on your phone (GitHub Pages, see below).
2. Chrome menu → **Add to Home screen** / **Install app**. It then opens like a normal app and works offline.
3. **Players** tab: add everyone.
4. **Match** tab: pick singles or doubles, put players on White and Black, tap **Start match**.
5. After each board: tap who cleared it, the opponent coins left, and whether the queen was covered → **Record board**.
6. When the match ends, tap **Save to leaderboard**.

## Scoring

- Board winner scores 1 point per opponent coin left on the board.
- Queen covered by the winner adds 3, only while the winner is below (target − 3), i.e. below 22 in a game to 25.
- First to the target wins. At the board limit the higher score wins; a tie plays another board.
- Leaderboard: 2 points per match win, ties broken by point difference.

## Backup

Scores live in the phone browser's storage. Use **Players → Save backup** now and then. **Restore backup** loads that file on any phone.

## Hosting on GitHub Pages

Repo → **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main`, folder `/ (root)` → Save.
The app will be at `https://<your-username>.github.io/<repo-name>/`.

## Files

- `index.html` – the whole app
- `sw.js` – offline support
- `manifest.webmanifest`, `icons/` – home-screen install
