# Changelog

All notable changes to Bill Tracker are documented here.

## [1.4.0] — 2026-06-09
### Added
- +/− toggle button next to amount field for easy negative entry on iPhone number pad
- Toggle pre-fills correctly when editing an existing entry

## [1.3.0] — 2026-06-09
### Added
- Edit any entry via an edit button on each row
- Recurring transactions — Monthly or Every 2 Weeks
- Auto-generates 2 years of future entries from the start date
- When editing a recurring entry, choose to update just that entry or all future unpaid entries
- When deleting a recurring entry, choose to remove just that entry or all future unpaid entries
- Past due flagging — unpaid entries past their due date show a PAST DUE badge and amber left border
- Past Due filter tab
- Entry count shows total, unpaid, and past due counts

### Changed
- Ledger now sorts oldest date first so most urgent entries appear at the top
- Recurring and bi-weekly badges shown on each recurring entry row

## [1.2.0] — 2026-06-09
### Added
- Load Data button — import a CSV to restore your data
- Save Data button — export your data as bills.csv
- CSV filename is always bills.csv (no date suffix) so you can overwrite the same file
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
