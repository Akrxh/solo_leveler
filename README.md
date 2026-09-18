# solo_leveler

A black and red daily routine tracker with Solo Leveling style levels and ranks.
Plain HTML plus a JSON config. No build step, no dependencies.

## Files
- `index.html` : the app
- `config.json` : goals, XP, penalty and rank settings (edit this to customise)

## Put it on GitHub Pages
1. Create a new repository and upload `index.html`, `config.json` and `README.md`.
2. Go to Settings > Pages.
3. Under Source choose "Deploy from a branch", pick `main` and `/ (root)`, then Save.
4. Open `https://YOUR-USERNAME.github.io/REPO-NAME/` after a minute.

## Customising
Open `config.json` to change goal minutes, XP rewards, the daily bonus, the penalty, level curve or rank names and thresholds.
If you change it, also update `DEFAULT_CONFIG` near the top of the script in `index.html` (it is only used when the JSON file can't load).

## How progress works
- Each quest earns XP in proportion to the time you log. Clear all four for a bonus.
- Finish a past day below 50% and you lose 150 XP.
- Progress is stored in your browser. Use Export / Import to back it up.
