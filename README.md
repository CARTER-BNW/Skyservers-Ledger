# Sky Servers Ledger

A live market price ledger and trading toolkit for the **Sky Servers** Minecraft server.

**[Open the live tool →](https://YOUR-USERNAME.github.io/skyservers-ledger/)**

*(Replace `YOUR-USERNAME` above with your actual GitHub username once this is live.)*

---

## What this is

A single-page web app, built from a real market scan of the Sky Servers shop, with four tools:

- **Market** - every scanned item with its live Buy/Sell prices, searchable and sortable.
- **Conversions & Buy Command** - convert any amount between items, stacks, shulkers, double chests, and inventories at current market value, and generate a ready-to-paste `/wtb` command.
- **Shopping List** - build a list of items you want, with quantity presets (stack, shulker, double chest, inventory), automatic pricing from the market, and a full crafting-cost breakdown for anything not directly sold (e.g. a Chest breaks down into Planks, then Logs).

All prices come from a real scan of the in-game shop GUI. Item names, icons, and crafting recipes come directly from the game's own data - not guesswork.

## Version

**v1.0** - first public release.

## How to use it

See [`HOW_TO_USE.md`](./HOW_TO_USE.md) for a full walkthrough of each tab.

## Offline copy

A self-contained, no-internet-required version is available in [`downloads/`](./downloads/) as a zip - download it, unzip, and open `index.html` directly in any browser. No installation needed.

## Updating the data

This ledger reflects a snapshot of the market at the time it was scanned. Prices in-game can change. If you spot something out of date, a new market scan and item-image extraction can be re-run and the data swapped in - see `HOW_TO_USE.md` for notes on where the data lives in `index.html`.

## License

This project's code is MIT licensed - see [`LICENSE`](./LICENSE). Minecraft item data and icons remain the property of Mojang Studios / Microsoft.

## Credits

Built by **xJBACx** for the Sky Servers community.
