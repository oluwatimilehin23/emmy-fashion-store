# Emmy Fashion Store

A one-page shop for Emmy: bags, shoes, clothes and accessories that you can turn 360° in 3D.

- The hero bag repaints itself in six colours as you scroll.
- Every product opens a 3D quick view: drag to turn, pinch to zoom, pick a colour and a size.
- A cart that adds up items, colours and sizes.

Everything is in one file, `index.html`. It needs no build step. Open it in a browser to see it.

## Editing the shop

Open `index.html` in a text editor (for example the free VS Code) and search for these:

| What | Search for |
|---|---|
| Products, prices, descriptions, colours | `const PRODUCTS = [` |
| The six hero bag colours and their names | `const COLOURS = [` |
| Shoe and clothing sizes | `const SIZES = {` |
| Bag details on the page (size, leather, weight) | `class="specs"` |

Each product looks like this:

```js
{ id: 'ballet-flat', art: 'flat', cat: 'shoes', name: 'Bow Ballet Flat', price: 120, sizes: 'shoes',
  colours: pick('cherry', 'cream', 'night'),
  desc: 'Soft leather with a small bow and a flexible rubber sole.' },
```

- `name`, `price` and `desc` are what shoppers see.
- `cat` is the category tab: `bags`, `shoes`, `clothes` or `accessories`.
- `tag: 'New'` puts it under "New in"; `tag: 'Bestseller'` shows a badge.
- `art` picks the drawing and 3D model, so keep it as one of the existing ones.

## Not connected yet

- Products, prices and details are placeholders.
- Checkout and the email sign-up don't save anything or take payments.
- Prices are shown in US dollars.
