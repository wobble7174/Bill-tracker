# 💰 Bill Tracker

A lightweight, mobile-friendly personal bill tracker that runs entirely in your browser. No accounts, no subscriptions, no data ever leaves your device.

## Features

- **Multiple accounts** — set up separate accounts (Checking, Savings, etc.) each with their own ledger and starting balance
- **Combined balance** — see the total current balance across all accounts at a glance in the header
- **Current balance per account** — shows the balance as of your last paid entry, not future projections
- **Running balance** — see your balance update in real time as you add entries
- **Recurring transactions** — set up monthly or bi-weekly bills that auto-generate entries through an optional end date
- **Paid / Unpaid tracking** — tap the circle checkbox to mark a bill as paid
- **Past due flagging** — any unpaid entry past its due date is automatically flagged
- **Edit entries** — edit any entry individually, or update an entire recurring series at once
- **Filter view** — filter by All, Unpaid, Paid, or Past Due
- **Load / Save CSV** — your data lives as a single CSV file you control; load it when you open the app, save it when you're done
- **Cross-device** — works on iPhone, desktop Chrome, Firefox, Edge — anywhere with a browser

## How to Use

### First Time
1. Open the app in your browser
2. Tap **Manage** to set up your accounts and give them names
3. Select an account from the dropdown
4. Tap **edit** next to Starting Balance and enter your opening balance
5. Add your first entry — amount, date, note
6. Tap **Save Data** to download `bills.csv` to your device

### Daily Use
1. Open the app
2. Tap **Load Data** and select your `bills.csv`
3. Add or edit entries
4. Tap **Save Data** when done — save over the existing `bills.csv`

### Managing Accounts
- Tap **Manage** in the header to open the accounts manager
- Add accounts with a name — each gets its own ledger and starting balance
- Rename any account at any time
- Delete an account — you will be warned how many transactions will also be deleted

### Switching Accounts
- Use the dropdown in the top left to switch between accounts
- The ledger and current balance update immediately
- The **All Accounts** total in the top right always reflects all accounts combined

### Understanding Current Balance
The **Current Balance** shown above the ledger is the balance as of your last paid entry. It is not a future projection. If no entries are paid yet, it shows the starting balance. The entry that defines the current balance is highlighted with a blue **Current** badge in the ledger.

### Adding a Recurring Bill
1. Fill in the amount, date (use the actual due date, e.g. the 14th), and note
2. Toggle **Recurring** on
3. Choose **Monthly** or **Every 2 Weeks**
4. Optionally set an **End Date** — leave blank to default to 2 years out
5. Tap **Add Entry** — entries are created automatically through the end date

### Editing a Recurring Entry
- Tap **edit** on any recurring entry
- If you changed the **End Date** only — a confirmation warning appears and the change applies to the whole series
- If you changed other fields — you are asked: **Just this entry** or **This and all future unpaid entries**

### Marking Bills as Paid
- Tap the circle on the left of any entry to toggle it paid/unpaid
- Paid entries are dimmed with a strikethrough
- Use the **Paid** filter to review what's been paid

## Your Data

All data is stored in a single CSV file on your own device called `bills.csv`. The app also uses browser localStorage as a working session cache. Nothing is ever sent to any server. See [PRIVACY.md](PRIVACY.md) for full details.

## Accessing on iPhone

1. Open the app URL in Safari
2. Tap the Share button → **Add to Home Screen**
3. It will appear as an app icon on your home screen

## Saving Your CSV on iPhone

When you tap **Save Data** on iPhone, the iOS Share Sheet will appear. Choose **Save to Files** and select your preferred location (iCloud Drive, Google Drive, etc). Always save over the same `bills.csv` file so you have one source of truth.

## Tech Stack

- Plain HTML, CSS, and JavaScript — no frameworks, no dependencies
- Browser localStorage for session caching
- CSV for persistent storage
- Hosted on GitHub Pages
