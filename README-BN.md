# Daily Sale — Offline Sales App

এই project-এ আছে:
- Dashboard: total sets added/sold, total profit/SIT, available stock, today's sales and target progress
- Add Product: multiple product entries, price, profit per set, type
- Product House: remaining stock; sales save হলে stock automatically কমে
- Add Sale: shop details, multiple products, auto date/time, SIT calculation
- Sale History: date → shop → sale details
- Today Target: multiple stores and Done / Not Done status
- Backup/Restore: JSON file-এ data export/import
- Offline PWA cache

## Run locally
1. VS Code-এ এই folder open করো।
2. VS Code Extensions থেকে **Live Server** install করো।
3. `index.html`-এ right click → **Open with Live Server**।
4. Browser-এ app খুলবে। Mobile/PWA offline install-এর জন্য প্রথমে HTTPS hosting (যেমন GitHub Pages) থেকে একবার online open করে cache হতে দাও।

## Important
- Data browser localStorage-এ এই device/browser-এ save হয়। অন্য phone-এ auto-sync হয় না।
- Browser/site data clear করলে data হারাতে পারে। নিয়মিত **Backup** button ব্যবহার করো।
- Private/incognito window-এ ব্যবহার করো না।
- Profit per set × quantity = SIT / recorded profit. If business profit must be separate from seller income, formula needs customization.
- This is a starter version. Test carefully with sample data and backup before using for real business.
- PWA install/offline needs secure HTTPS hosting or localhost.
- APK build later: update Node.js to a supported current LTS (Capacitor 7 generally requires Node 20+), install Android Studio + Android SDK, then set up Capacitor. Current Node v18.16.1 is old for the modern Android packaging path.
