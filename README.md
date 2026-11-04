# Remodel bid comparison

Static page with two tabs:

- **Windows & doors**: window and door bids compared opening by opening (required size and operation, each bidder's drawing, price, match status, U-factor).
- **HVAC / heat pumps** (`#hvac`): heat pump bids checked requirement by requirement against the Skyline ductless spec (cassettes and floor units only). Shows each bidder's own spec sheet or quote, quoted price, and a meets / caveat / fails / not-documented status per requirement.

## Publish with GitHub Pages
1. Copy `index.html`, `img/` and `.nojekyll` to the repository root and push to `main`.
2. In the repository: Settings → Pages → Build and deployment → Source: "Deploy from a branch", Branch: `main`, folder `/ (root)` → Save.
3. The site appears at https://dmhenke.github.io/Remodel_WindowsDoors/ (HVAC tab: `.../#hvac`) within a minute or two.

All data is embedded in `index.html`; there is no build step. Window/door data is regenerated from `Window_Door_Bid_Comparison.xlsx`; HVAC data (the `hvacdata` JSON block) follows `hvac_work/bids_and_specs/HVAC_Bid_Evaluation.md`. HVAC images live in `img/hvac/`; customer details are cropped out of local contractor quotes because this repository is public.
