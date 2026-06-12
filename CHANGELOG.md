# Changelog

All notable changes to Bill Tracker are documented here.

## [2.0.0] — 2026-06-12
### Added
- Multiple accounts — add, rename, and delete named accounts (Checking, Savings, etc.)
- Account dropdown in header to switch between accounts instantly
- Combined current balance in header showing total across all accounts
- Current Balance per account — calculated from last paid entry, not future projections
- Blue "Current" badge and left border highlight on the entry that defines current balance
- Warning dialog when deleting an account that has transactions
- CSV now stores account definitions and an AccountId column per entry
- Old single-account CSVs still import correctly

### Changed
- Removed Future Balance from header — replaced with per-account Current Balance above ledger
- Starting balance now per-account, editable per account

## [1.5.0] — 2026-06-10
### Added
- End date field for recurring entries — leave blank to default to 2 years, or set a specific stop date
- End date field in edit modal for recurring entries — changing only the end date shows a warning and applies to the whole series without asking
- Form collapses after adding an entry so you return directly to the ledger
- ＋ Add Entry toggle button — form is hidden by default, tap to expand

### Changed
- Future Balance replaces Current Balance in header with a ? info button explaining what the number represents

## [1.4.0] — 2026-06-09
### Added
- +/− toggle button next to amount field for easy negative entry on iPhone number pad
- Toggle pre-fills correctly when editing an existing entry

## [1.3.0] — 2026-06-09
### Added
- Edit any entry via an edit button on each row
- Recurring transactions — Monthly or Every 2 Weeks
- Auto-generates entries from the start date through the end date (default 2 years)
- When editing a recurring entry, choose to update just that entry or all future unpaid entries
- When deleting a recurring entry, choose to remove just that entry or all future unpaid entries
- Past due flagging — unpaid entries past their due date show a PAST DUE badge and amber left border
- Past Due filter tab
- Entry count shows total, unpaid, and past due counts

### Changed
- Ledger sorts oldest date first so most urgent entries appear at the top
- Recurring and bi-weekly badges shown on each recurring entry row

## [1.2.0] — 2026-06-09
### Added
- Load Data button — import a CSV to restore your data
- Save Data button — export your data as bills.csv
- CSV filename is always bills.csv so you can overwrite the same file
- Paid/Unpaid checkbox on each entry
- Filter tabs: All, Unpaid, Paid
- Toast notifications for load and save actions

### Changed
- Prominent Load/Save buttons moved to top of page for easier access on mobile

## [1.1.0] — 2026-06-09
### Added
- Export CSV button
- Import CSV button
- localStorage persistence between sessions

## [1.0.0] — 2026-06-09
### Initial Release
- Starting balance with edit button
- Add entries with amount, date, and note
- Running balance calculated and displayed per row
- Current balance shown in sticky header
- Mobile-first dark UI
