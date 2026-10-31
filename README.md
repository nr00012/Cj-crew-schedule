# CJ Crew Schedule

Weekly crew schedule for CJ Coffeehouse. It runs as an installable web app (PWA) on iPhone, with hour totals per person and per day, break rules, and offline support.

The schedule is stored **on the phone** (browser storage). This repository holds only the app code, never crew names or hours.

## Install on iPhone

1. Open the GitHub Pages link in **Safari**.
2. Tap **Share** → **Add to Home Screen** → **Add**.
3. Open **CJ Schedule** from your Home Screen.
4. Tap **Restore from backup** and pick your `cj-schedule-backup-….json` file. Do this inside the Home Screen app, because Safari and the installed app keep separate data.

## Weekly use

- Use the arrows to move to next week, then tap **Copy last week** or **Use standard schedule**.
- Tap a shift to edit or delete it. Tap **+ Add shift** to add one.
- **Copy for group text** copies the week to paste into a group chat.
- **Export CSV** gives you a file for payroll.
- **Back up now** every couple of weeks, and save the file to iCloud Drive.

## Hours rules used

- Rest break (paid, 10 min): 1 for shifts of 3.5–6 h, 2 for shifts over 6 h up to 10 h.
- Meal break (unpaid, 30 min): shifts over 6 h. **Paid hours** = scheduled hours minus this meal.
- Flags: shift over 8 h, over 40 paid hours in a week, double-booking, and gaps with nobody scheduled.

## Updating the app

Edit `index.html`, then bump `VERSION` in `sw.js` so installed copies pick up the change on next launch.

## Hosting

GitHub Pages: **Settings → Pages → Build and deployment → Deploy from a branch → `main` / `(root)`**.
