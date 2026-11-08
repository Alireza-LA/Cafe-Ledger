# Cafe Ledger

A small, local-first sales tracker designed to install on an iPhone from Safari. It also runs on Android browsers.

## Run it

Serve this folder over HTTPS (or `localhost` while developing). For example, with Python installed:

```sh
python -m http.server 8000
```

Open `http://localhost:8000` on the computer. For an iPhone, publish the folder to any HTTPS static host, open its address in Safari, then choose **Share → Add to Home Screen**. The app shell is cached for offline use after its first load.

## Use it

Add the cafe's menu items and prices in toman. Tap an item to record a quick sale. Hold briefly to edit or remove it; hold for 2.25 seconds, then drag it to reorder the menu. Use **Export menu** to save a JSON menu backup and **Import menu** to restore it; import adds items whose names aren't already present. Choose **New invoice** to add several menu items and invoice-only custom items (with optional descriptions) to one customer invoice. Invoice lines are saved to sales only when you tap **Save invoice**; **Cancel** discards the draft. Each invoice gets an ID. Choose a date to view another day's entries; its Shamsi date is shown below the date picker. **Export Excel** downloads a formatted `.xlsx` workbook with bold, centered cells, Persian column names, export date and time, and one row per item sold with invoice number, Shamsi date, description, quantity, unit price, and line total in toman.

Sales and menu items are stored in this browser on this device. Clearing browser website data removes them, so export a spreadsheet backup regularly. This first version does not sync between devices.
