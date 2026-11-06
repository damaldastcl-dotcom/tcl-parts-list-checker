# Parts List Checker

Main published link: https://damaldastcl-dotcom.github.io/tcl-parts-list-checker/

Open the link in a browser. It works offline once it is open. No search is sent anywhere.

## What is in this repo

- index.html: the checker, current build. Search by serial number, model number, part number, or remote.
- Parts_Checker_Master.xlsx: the own Excel file for this checker. Sheets: README_Sources, Serial_Lookup, ASP_TV_Parts, BOM_Fallback_Parts, Remote_HQ.
- builds/: dated builds of the checker. Only the last 5 builds are kept. Older builds are removed when a new build is added.
- README.md: this note.

## How to use it

- Serial number: characters 5 to 14 are the Mid SN. That gives the exact model and BOM.
- Model number: all BOMs for that model are shown at a glance, with key boards and remote first, then the full parts list for each BOM. Hover a BOM button to preview its key parts. No Show parts click is needed.
- Part number: reverse lookup, sorted by model number.
- Remote finder: enter a model to see its main remote first, then its alternative remotes, with a picture when the HQ remote file has one for that remote code. Enter a remote part to see models sorted by model number first, then alternative matches.
- Price and stock: Unit Price and Stock A and B come from the ASP Pricing sheet. A blank stock means that sheet did not list a stock number for that row. This is the stock in that file, not a live ITI check.
- Main board PID: ASP main board parts carry a suffix after a colon, for example G0301-000609-Z00:11292. That suffix is the Project ID. Send ITI the PID for main boards.

## Sources

- BOM_Table_2026-09-15_1.xlsx, merged Nov 2, Nov 5 and Nov 6, 2026: serial to BOM lookup and fallback BOM parts. Serials 35,792 as of Nov 6, 2026.
- Parts_Prices_Stock - (Internal) - Team Share.xlsx: ASP Pricing, TV division. Upload dates in that file: USA 2026-10-27, Canada 2026-10-26.
- Remote_control_HQ_-_Team_Share.xlsx: remote pictures and HQ remote notes.

Current build: 2026-11-06, merged Nov 6 BOM file. Models 1,016, serials 35,792, ASP TV rows 98,182.
