# How to Use the Sky Servers Ledger

This page has three tabs across the top. Everything runs in your browser - nothing is sent anywhere, and no account or login is needed.

---

## Market

The full list of items scanned from the shop, with:

- **Buy 1x / 32x / 64x** - what it costs you to buy that quantity from the shop.
- **Sell 1x / 64x** - what the shop pays you for that quantity.
- A dash (`-`) means the shop doesn't buy or sell that item at that quantity.

**Search** - type any part of an item's name to filter the list instantly.

**Filter chips** - narrow the list to only items you can buy, or only items you can sell, using the buttons above the table.

**Sorting** - click any column header to sort by it. Click again to reverse the order. Items with no price for that column always sink to the bottom.

**The `/wtb` button** on each row jumps you straight to the Buy Command tool with that item already selected.

---

## Conversions & Buy Command

This tab has two tools stacked on top of each other.

### Conversions

Pick an item, type an amount, and choose a unit (Item, Stack, Shulker, Double Chest, or Inventory). The tool shows you that same quantity converted into every other unit, plus its total value.

- By default, value is calculated using the item's market **sell** price.
- If you want to price it differently (e.g. you're negotiating a different rate), type a **custom price per item** and the total updates to use that instead.
- If an item has no sell price at all, you'll need to enter a custom price to see a value - otherwise it'll just show the conversion with no dollar total.

### Buy Command

Pick an item and an amount, and this builds the exact command to paste in-game:

```
/wtb buy <item> <amount> <price>
```

- The price defaults to the item's market **buy** price × amount, rounded to a whole dollar (since `/wtb` takes a flat total, not a per-item rate).
- You can override this with a custom price per item if you want to offer a different rate.
- If the item isn't buyable on the market at all, the tool will tell you, but you can still type in a custom price to generate a command anyway.
- Hit **Copy** to copy the finished command straight to your clipboard.

---

## Shopping List

Build a list of everything you're planning to buy or make, with running totals.

### Adding items

1. Search for an item by name.
2. Type a quantity, and (optionally) pick a size multiplier from the dropdown - **x16 (Small Stack)**, **x64 (Big Stack)**, **x1,728 (Shulker)**, **x3,456 (Double Chest)**, or **x2,304 (Inventory)**. The multiplier multiplies whatever number you typed - so typing `3` and picking Big Stack adds 192.
3. Click **Add**.

Adding the same item twice just increases its quantity in the list rather than creating a duplicate row.

### Pricing

Each item's price is worked out automatically, in this order:

1. **Custom price** - if you've typed one in directly for that row, it always wins.
2. **Market price** - if the item is sellable in the shop, its sell price is used.
3. **Crafted cost** - if the item isn't sold directly but can be crafted, the tool works out what it would cost to buy all the raw materials needed to make it (recursively - a Chest needs Planks, which need Logs, and the tool prices the Logs).
4. **Not available** - if none of the above apply, the line shows "Not available," and you can type in your own price manually if you still want it counted in the total.

A small tag next to each item name (`market`, `crafted`, `custom`, or `unavailable`) shows you which of these applies.

### Viewing the crafting breakdown

Any craftable item shows a **show materials** link. Click it to see the exact raw materials and quantities needed, all the way down to base resources.

### Editing and removing

- Change the **amount** or **price** directly in the table at any time - the total updates live.
- Click **Remove** to delete a single row.
- Click **Clear list** (bottom right) to empty the whole list at once.

---

## A note on accuracy

- Prices reflect a snapshot of the shop at the time it was scanned - they are **not live**. If the shop's prices change in-game, this page won't know until it's re-scanned and re-published.
- Crafting costs are calculated using real game recipes, but only cover standard crafting/smelting/stonecutting recipes - a small number of special items (smithing-table upgrades, banner duplication, etc.) aren't priced this way.
- Item icons are pulled from the game's own textures. A small number of items use an approximate icon (one face of a multi-sided block) rather than a perfect render, and a handful of fully custom-modeled items (Chests, Shulker Boxes, etc.) may have no icon at all.
