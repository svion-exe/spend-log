# Daily Spend Log

A small expense tracker that runs in your phone's browser and installs to the home screen like an app.
It works with no internet after the first open. Your entries are stored on your phone only.

## What the app does

- **Daily log** with one-tap item buttons that remember the last price.
- **Quick add:** one tap logs a regular item for today, with Undo.
- **Budget meter** with a pace marker and a per-day figure for the rest of the month.
- **Limits per group** (Settings): a group bar turns amber at 80% and red past the limit.
- **Shared items by number of people:** set how many people share an item (counting yourself). Your part is the bill divided by that number.
- **Balance with others:** tracks who paid at the shop and payments between you, and shows who owes whom.
- **Insights tab:** spending by day, comparison with last month, and your biggest items.
- **Monthly repeats** (Settings): items added to your log automatically on the day you choose.
- **Search and group filter** on the By day list.
- **Plain text and CSV downloads** for each month.
- **Meal nudge:** a reminder banner if lunch (after 2 pm) or dinner (after 9 pm) is not logged.
- **Appearance:** match your phone, light, or dark.
- **Backup and restore** in Settings.

## What is in this folder

| File | What it does |
| --- | --- |
| `index.html` | The app itself |
| `manifest.webmanifest` | Tells the phone the name, colors and icon for the home screen |
| `sw.js` | Lets the app open with no internet |
| `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` | Home screen icons |

## Put it online with GitHub Pages (one time, about 5 minutes)

1. On github.com, click **New repository**. Name it `spend-log`. Choose **Public** (free GitHub Pages needs a public repo). Tick **Add a README file** if you like, then create it.
2. In the repo, click **Add file**, then **Upload files**. Drag in every file from this folder except this README. Click **Commit changes**.
3. Open the repo's **Settings**, then **Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Set **Branch** to `main` and the folder to `/ (root)`. Click **Save**.
4. Wait a minute or two. The page shows your address: `https://YOUR-USERNAME.github.io/spend-log/`

The repo holds only the app. It never contains your expenses, so a public repo exposes nothing personal.

## Install it on your phone

Open your address once, with internet on. Then:

- **Android (Chrome):** menu (three dots), then **Install app** or **Add to Home screen**.
- **iPhone (Safari):** Share button, then **Add to Home Screen**.

Open it from the new icon from then on. Always use the same address, because your entries are tied to it.

## Keep your data safe

- Your entries exist only on this phone. Clearing the browser's site data, uninstalling, or losing the phone deletes them.
- In the app, open **Settings**, then **Backup**, then **Export backup**. Send the file to your email or Drive. Once a week is enough; the app reminds you.
- To restore on the same or a new phone, open **Settings**, then **Import backup**, and pick the file.
- Use **Plain text**, then **Download .txt** for a readable monthly record.

## Updating the app later

Upload the new `index.html` to the repo with **Add file**, **Upload files**, and commit. The app picks it up the next time you open it with internet. Your entries stay.
