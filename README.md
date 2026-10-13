# PI Planning Bord

A browser tool for building PI planning slides: categories, cards, confidence votes, sprint spans and post-PI outcomes, with export to editable PowerPoint.

No build step. Everything runs in the browser, and boards are stored in the browser's local storage. Use **Meer → Bord opslaan als JSON** to share or back up a board.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole app (markup, styles, script) |
| `pptxgen.bundle.js` | PptxGenJS 4.0.1, loaded only when someone exports |
| `pptxgen.LICENSE.txt` | MIT license for PptxGenJS |

## Theming

All colors are at the top of the `<style>` block in `index.html`, under `:root`. The app, the slide, the category palette, the confidence scale and the outcome colors all read from there, including the PowerPoint export.

The font (Figtree) loads from Google Fonts. To self-host it instead, put the `.woff2` files next to `index.html`, replace the Google Fonts `<link>` with an `@font-face` rule, and keep the `--font` variable.
