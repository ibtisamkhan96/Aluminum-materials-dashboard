# Aluminium, Materials Data Series #2

An interactive data dashboard and LinkedIn carousel on the world's #2 metal: who makes it, what the alloys do, why it flies, and the energy story behind every can.

Part of my Materials Data Series, where I take one material at a time and tell it as a materials engineer who works in data. Steel was #1. Copper is next.

**Live dashboard:** _(deploy `index.html` to Netlify/GitHub Pages)_

---

## What's inside

| File | What it is |
|------|-----------|
| `index.html` | Interactive Chart.js dashboard, 5 tabs: Production & Geography, What 72 Mt Looks Like, The Alloy Families, Strength-to-Weight, The Energy Story |
| `fetch_data.py` | Reproducible Python pipeline that compiles the cited figures into `data/*.csv` |
| `data/*.csv` | Tidy datasets (production, trend, metals comparison, primary vs recycled, CO₂ by power source, end-use, alloy properties, scale comparisons) |
| `carousel/index.html` | 9-slide LinkedIn carousel (1080×1080) |
| `Aluminium_Materials_Carousel.pdf` | Exported carousel, ready to upload |
| `linkedin-post.txt` | Post caption |

## Reproduce the data

```bash
python fetch_data.py      # writes data/*.csv
```

The dashboard embeds the same numbers in JS so it runs from `file://` with no server. `fetch_data.py` documents where each figure came from and makes them reproducible.

## What the data shows

- **72.3 Mt** of primary aluminium in 2024, the second most-produced metal, but steel still out-makes it about **25 to 1**.
- **China smelts ~59%** of it, because primary aluminium is effectively solid electricity (~15 MWh per tonne) and China has the cheapest power.
- Pure aluminium is weak; the **alloy series** (2xxx–7xxx) multiplies its strength up to tenfold. **7075 rivals structural steel at a third of the weight**, that's why it flies.
- A primary tonne carries **~16.5 t CO₂**; recycling the same metal takes **~5% of the energy** and loses no quality, so it cycles indefinitely.
- **Scale:** ~2.3 t/second → ~5.6 trillion drink cans, ~1 million Boeing 747s, or ~400 million cars' worth of aluminium a year.

## Sources

International Aluminium Institute (primary production, carbon-footprint FAQs) · USGS Mineral Commodity Summaries · Recycling Today · ASM Metals Handbook / MatWeb (typical alloy properties).

Production figures are primary metal in Mt, rounded and attributed. Property values are typical published datasheet figures for standard tempers, illustrative, not specification.

---

*Built by Ibtisam Ahmed Khan · June 2026 · [linkedin.com/in/ibtisam-ahmed-khan](https://linkedin.com/in/ibtisam-ahmed-khan)*
