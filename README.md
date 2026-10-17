# SALTBURN CAPITAL — My Wallet

A small, installable progressive web app (PWA) for personal budgeting. It is designed to work offline after the first successful visit and stores data in the browser's local storage on the current device.

## Features
- Daily Budget and Leisure envelopes
- Monthly plan for income, essential costs, and envelope budgets
- Expenses and money received, categories, notes, dates, and deletion
- Monthly history and a six-month spending chart
- Currency display preference
- JSON backup export and restore
- No account, external analytics, or financial-data server

## Run locally
A PWA service worker requires localhost or HTTPS; opening `index.html` directly as a file is not sufficient for offline-install testing.

1. Install Node.js LTS from https://nodejs.org/ and Visual Studio Code from https://code.visualstudio.com/ if they are not already installed.
2. Unzip this folder.
3. In the folder, run a local static server. If Python is installed, open a terminal in this folder and run `python -m http.server 8000`.
4. Open `http://localhost:8000` in your browser.

## Host for phone installation
Deploy the contents of this folder to a static HTTPS host such as GitHub Pages. On iPhone, open the HTTPS site in Safari and use Share → Add to Home Screen. On Android, open it in Chrome and use Install app / Add to Home Screen.

## Privacy and important limitations
- Data is local to this browser profile and device; it is not synchronized between devices.
- Clearing browser site data may erase records. Export backups regularly.
- Importing a backup replaces current local data.
- The dashboard's available balance is calculated as planned income minus planned essential costs minus expenses plus recorded money received in both envelopes. The envelope balances are calculated from their own monthly plans and transactions.
- This app is a personal tracker, not a bank connection or accounting service.
