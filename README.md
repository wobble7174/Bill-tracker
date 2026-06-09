# 💰 Bill Tracker

A lightweight, mobile-friendly personal bill tracker that runs entirely in your browser. No accounts, no subscriptions, no data ever leaves your device.

## Features

- **Running balance** — see your balance update in real time as you add entries
- **Recurring transactions** — set up monthly or bi-weekly bills that auto-generate 2 years of entries
- **Paid / Unpaid tracking** — tap the circle checkbox to mark a bill as paid
- **Past due flagging** — any unpaid entry past its due date is automatically flagged
- **Edit entries** — edit any entry individually, or update an entire recurring series at once
- **Filter view** — filter by All, Unpaid, Paid, or Past Due
- **Load / Save CSV** — your data lives as a CSV file you control; load it when you open the app, save it when you're done
- **Cross-device** — works on iPhone, desktop Chrome, Firefox, Edge — anywhere with a browser

## How to Use

### First Time
1. Open the app in your browser
2. Tap **edit** next to Starting Balance and enter your opening balance
3. Add your first entry — amount, date, note
4. Tap **Save Data** to download `bills.csv` to your device

### Daily Use
1. Open the app
2. Tap **Load Data** and select your `bills.csv`
3. Add or edit entries
4. Tap **Save Data** when done — save over the existing `bills.csv`

### Adding a Recurring Bill
1. Fill in the amount, date (use the actual due date, e.g. the 14th), and note
2. Toggle **Recurring** on
3. Choose **Monthly** or **Every 2 Weeks**
4. Tap **Add Entry** — 2 years of entries are created automatically

### Editing a Recurring Entry
- Tap **edit** on any recurring entry
- Choose **Just this entry** or **This and all future unpaid entries**

### Marking Bills as Paid
- Tap the circle on the left of any entry to toggle it paid/unpaid
- Paid entries are dimmed with a strikethrough
- Use the **Paid** filter to review what's been paid

## Your Data

All data is stored in a CSV file on your own device. The app also uses browser localStorage as a working session cache. Nothing is ever sent to any server. See [PRIVACY.md](PRIVACY.md) for full details.

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
