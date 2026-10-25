# Teaching Games Catalogue (GitHub Pages)

A free, static catalogue website for your HTML teaching games.

## Files
- `index.html` — catalogue homepage
- `games.json` — the list of games shown on the homepage
- `games/` — individual game HTML files

## Publish on GitHub Pages
1. Create a **public** repository on GitHub, for example `teaching-games-catalogue`.
2. Upload the contents of this folder (upload `index.html`, `games.json`, the `games` folder, and this README; do not upload the outer folder as a nested folder).
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then Save.
6. Wait for publishing, then open the website URL shown on the Pages settings page. It will look like `https://YOUR-USERNAME.github.io/teaching-games-catalogue/`.

## Add a new game later
1. Upload the new standalone HTML game into the `games/` folder, e.g. `games/festival-match.html`.
2. Edit `games.json` and add another object inside the outer square brackets. Keep commas between objects:
   {
     "title": "Festival Match",
     "description": "Match festival vocabulary with the correct meanings.",
     "category": "Vocabulary",
     "level": "Year 7–9",
     "language": "Mandarin Chinese",
     "file": "games/festival-match.html",
     "tags": ["Vocabulary", "Matching"],
     "emoji": "🏮"
   }
3. Commit/save the changes. GitHub Pages will republish the catalogue. The new game appears as a card on the same homepage.
4. Test the Play link on the live site.

## Notes
- GitHub Pages on GitHub Free requires a public repository. Published pages are publicly accessible.
- The catalogue is static and has no server or paid database.
- Keep each game as a self-contained HTML file when possible. If a game uses separate CSS, JS, images, or audio files, upload those assets too and preserve the relative folder paths.
