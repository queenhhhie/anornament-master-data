# anornament · stall book

A single-file app for recording market and online sales, and tracking stock from what's at home
through to what's in the trolley. No build step, no dependencies, no server.

## Putting it online

1. Create a repository on GitHub — `stall-book` is a fine name.
2. Upload `index.html` to the root of the repository. That's the whole app.
3. Go to **Settings → Pages**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`, and save.
4. Wait a minute or two. The address will be `https://YOUR-USERNAME.github.io/stall-book/`.
5. Open it on your phone and add it to the home screen — it then opens like an app, full screen.

To update later, replace `index.html` in the repository. Your records are **not** in the file,
so updating never touches them.

## Where the data lives

Everything is saved in the browser on the device you're using, under that exact web address.
Nothing is sent anywhere and nothing is stored in the repository.

This means:

- **Same address, same browser, same device** — your records are there.
- **A different device** does not see them. Use the backup file to move records across
  (Dashboard → *Download full backup*, then *Load a backup from the other device* → **Merge**).
  Merging is safe in both directions: records are matched by ID, so nothing doubles up.
- **Clearing your browser data will delete your records.** Download a backup after every market.
- The repository is public, so the code and the product catalogue are visible to anyone with the
  link. Your sales, costs and stock are not — they never leave your device.

## First run, in this order

1. **Products** — download the CSV, add your material costs and reorder levels, upload it back.
2. **History** — type up past market sales (Sales → *Type up paper records*) and import your
   Shopify orders export (Online tab). Do this *before* counting.
3. **Count** — Inventory → *Cycle count* → *Everything*. This sets your true on-hand and absorbs
   anything the history couldn't explain.

Counting must come last. A count corrects the numbers as they stand at that moment, so history
added afterwards will pull them out again.

## The routine

- **Before a market** — Market tab → *Trolley* → load what you're taking (*Copy last load* helps).
- **At the market** — pick the market and date at the top, then sell. Tiles show what's in the trolley.
- **After** — *Bring it all home*, add the pitch fee under Dashboard → Costs, download a backup.
- **Weekly** — cycle count one category, so you never face a full stocktake.
- **When Shopify orders come in** — Online tab → upload the orders export. Re-uploading an
  overlapping file is safe; orders already imported are skipped.

## Files

- `index.html` — the entire app.
- `README.md` — this file.
