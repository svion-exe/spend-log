# Daily Spend Log

A small expense tracker that runs in your phone's browser and installs to the home screen like an app.
It works with no internet after the first open. Your entries are stored on your phone only.

## What the app does

- **Four tabs** at the bottom: Today, Log, Insights, More. A floating **+** button opens the Add expense form as a sheet.
- **Today:** budget meter, streak, quick add, and today's entries. "Where it went" is folded away until you tap it.
- **Quick add** with smart suggestions: items you usually buy around this time of day come first. Tap one and the amount field opens with the number pad. Amounts are never prefilled, since food court prices change.
- **Opens straight to the form** at your usual lunch or dinner time.
- **Catch-ups:** a banner if lunch (after 3:30 pm) or dinner (after 10:30 pm) is not logged today, and if yesterday's lunch or dinner was missed. Each has Add and Skip.
- **Repeat yesterday:** adds yesterday's entries to today in one tap, with Undo.
- **Under-budget streak:** counts days you logged and stayed within your budget spread evenly over the month.
- **Compact log:** tap an entry to edit, swipe left to delete. Only the last 7 days are open; older days are folded.
- **Home-screen shortcuts:** long-press the installed icon for Add lunch, Add dinner, Add expense. You may need to remove the icon and install again once for these to appear.
- **Monthly repeats**, **backup**, **theme** and the item list are in collapsible sections under More. Spending per group is shown under "Where it went".
- **Shared items by number of people:** your part is the bill divided by that number. The balance with others is tracked under More.
- **Duplicate guard:** adding the same entry twice within two minutes asks you to confirm.
- **Share summary:** under More, send your roommate a text of this month's shared items and who owes whom.
- **Left for today:** the big line on Today. Whatever you did not spend on earlier days carries over, so one cheap day gives you room the next.
- **Drag to close:** the add form is a bottom sheet with a grab handle. Pull it down to dismiss, or tap outside, press Close, or Escape. Pulling down slowly a short way snaps it back.
- **Price reference:** when you pick an item, the form shows what you paid last time and your usual range. The amount is still left empty for you to type.
- **Typo guard:** if an amount is about 3 times more or less than your usual for that item, the form shows a hint and asks you to tap again to confirm.
- **Last 6 months:** in Insights, monthly totals side by side.
- **Colour themes:** under More, Appearance. Original (the default look), Ocean, Sunset and Plum, each with its own light and dark version. Light or dark is chosen separately.
- **Month at a glance:** a calendar in Insights. Each day is tinted by how it compares with your daily allowance. Tap a day with entries to jump to it in the Log, or an empty day to add an entry for that date.
- **Month-end forecast:** from day 5, a line on Today says where the month will end at your current pace.
- **What your meals cost:** in Insights, your average lunch and dinner price, the cheapest and dearest weekday, and the time of day you paid least. It appears once you have 6 logged meals of a kind.
- **Fix amount:** after adding an entry, a button on the confirmation lets you correct it at once.
- **Insights:** spending by day, comparison with last month, biggest items.
- **Search all months:** in the Log, tick "Search all months" to find an entry in any month, such as when you last bought oats. Results show how many entries, in how many months, and the total.
- **Search and group filter**, plus **plain text and CSV downloads** in the Log tab.

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
- In the app, open **More**, then **Backup**, then **Share backup**. Send the file to Drive, email, or WhatsApp to yourself. **Download backup** saves it to your phone instead.
- To restore on the same or a new phone, open **Settings**, then **Import backup**, and pick the file.
- Use **Plain text**, then **Download .txt** for a readable monthly record.

## Updating the app later

Upload the new `index.html` to the repo with **Add file**, **Upload files**, and commit. The app picks it up the next time you open it with internet. Your entries stay.
