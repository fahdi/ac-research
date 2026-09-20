# 2-ton inverter AC research, Rawalpindi/Islamabad, September 2026

Research for buying a 2.0 ton wall-mounted DC inverter AC for a 7 x 4 m hall. Requirements in priority order: wall split, WiFi app control (voice preferred), T3 tropical rating, highest EER, low indoor noise, copper condenser only if owner-confirmed, air purification as a bonus, brand irrelevant.

## Contents

- `docs/2-ton-ac-comparison-2026-09-20.md`: the main report. Combined 106-row table across Japan Electronics, Umar Electronics and Friends Electronics, shortlist, same-model price differences, contradictions with the shop's verbal quotes, owner-review summaries.
- `docs/follow-up-notes.md`: brand satisfaction ratings, best Gree model and where to buy it, store addresses, 1.5 vs 2 ton sizing.
- `docs/combined-table.md`: the raw price-sorted table on its own.
- `ac-faceoff.html`: interactive comparison tool. Open it in a browser, pick any two models, and read every captured spec side by side with differences highlighted. Also published at https://claude.ai/artifact/KzBfw2x5Nrnw7gbtDb1bno (private link).
- `data/`: raw captures used for the tables. Japan Electronics Shopify product feeds, Umar Electronics WooCommerce Store API responses, Friends Electronics category scrape, Kenwood Pakistan official product feed, plus the stripped spec text extracted from each listing.
- `scripts/build_table.py`: builds `docs/combined-table.md` from the hand-verified row data.

## Headline findings

- The shop's "KES 24522 at Rs 300,000" is the Kenwood KES-2452FHI Superia Smart, a floor-standing cabinet, so it fails requirement 1. Japan Electronics lists it at exactly Rs 300,000 (out of stock); Kenwood official Rs 365,000.
- The shop's "KES 24625 at Rs 200,000" is the Kenwood KES-2462S eSupreme Pro, Rs 220,000 at Umar. It has no WiFi, no T3 and no published EER, and is gone from Kenwood's current catalog.
- No 2-ton wall unit on sale publishes EER 4.0. Best with WiFi and T3 is 3.6 on paper (Midea Xtreme, Midea Breezeless, Kenwood eLuxury Pro) and about 3.7 derived for the Gree Airy Pro and Pular T3 15W.
- No owner or reviewer confirmed a copper condenser on any model; every copper mention is a seller claim.
- Only 10 of 106 listings publish indoor noise. Quietest published: Samsung 44/28, LG 46 to 28, Gree Airy series 19 dBA silent mode.
- Gree has the best owner satisfaction in Pakistan (3.8/5, 70 percent recommend); Midea and TCL match it on efficiency but score badly on after-sales.
- Final pick: Gree Airy Plus GS-24AITH21B-T3, Rs 264,900, in stock at Japan Electronics on Murree Road and Blue Area. Upgrade path: Gree Airy Pro GS-24AITH24W-T3 at Rs 294,900 from DWP Home if voice control and UVC purification are worth Rs 30,000.

## Method

Prices and stock were read from the stores' own machine-readable feeds (Shopify `products.json`, WooCommerce `wc/store/v1`) between 02:30 and 03:30 PKT on 20 September 2026, then cross-checked against Kenwood, Gree (DWP), Samsung, LG and Haier official pages. Owner sentiment comes from BrandReview.pk aggregate ratings and PakWheels forum threads. Values a seller never stated are marked "n/s"; derived EERs are marked "calc".
