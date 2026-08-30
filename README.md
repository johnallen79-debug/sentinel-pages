# Sentinel site pages

Five pages, plain HTML. Upload the contents of this folder to a public GitHub
repository, turn on GitHub Pages, and point each Wix embed at the resulting
address using **Website address** mode rather than Code mode.

## Files

| File | Wix page |
|---|---|
| `homepage.html` | the home page |
| `cqc.html` | `/cqc` |
| `iso.html` | `/iso` |
| `ecos.html` | `/ecos` |
| `about.html` | `/about` |

`assets/hero/` holds all 22 hero images, web-sized to 1400px wide as JPEG,
about 88KB each. They are not yet wired into the pages.

All 22 come from the same model, generated from one prompt template where only
the subject, scene, accent colour and whether people appear change between
them. An earlier set made in ChatGPT was discarded: same wording, different
model, and side by side the two read as two sets rather than one.

They are normalised to a common brightness of 169 (spread of 1 across the set),
which is light enough to sit on the #F7F9FC page without reading as a hole
punched in the layout. Five have blown highlights above 3 per cent; all five
were already like that in the original, from bright windows in the scene, and
the normalisation did not cause it.

## What is finished

- All links absolute, so nothing resolves against the iframe's own address.
- A navigation fallback for a restrictive iframe sandbox: it tries the top
  window, then asks the parent to navigate, then opens a new tab.
- Height reporting, for the Velo snippet.
- Every price checked against the live Wix store. All 21 match.
- Product links use the real store slugs. Three do not follow the pattern
  their name suggests: `isoiec-27001`, `isoiec-20000-1`, `isoiec-42001`.
- ISO 9001 shows "Available 16 September" instead of a price. The store
  product is out of stock with a matching ribbon, so the page and the shop
  agree. The sixth edition publishes 16 September 2026.
- Document counts and guide pages current, including Adult Social Care at 56
  documents and a 104 page guide.

## What is not finished

**Five of sixteen ISO cards expand.** ISO 27001, 14001, 45001, 22301 and
13485 open to show what the standard is, key facts, who needs it and where
organisations get caught out. The other eleven are still plain cards. ISO 9001
is deliberately last, because its content changes on 16 September.

**The hero images are not in the pages yet.** All 22 are in `assets/hero/`,
ready to use, but nothing references them.

**Six links have no page behind them:** `/tools`, `/publications`,
`/contact`, `/privacy-policy`, `/terms` and `/cookies`. Left in place because
those pages are going to be built.

## Known, and not a fault of these files

The sixteen `/standards/...` pages all serve identical ISO 9001 content at the
wrong price. Nothing in these pages links to them; the expanding cards replace
them.
