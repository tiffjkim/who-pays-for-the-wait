# Who pays for the wait

A one-page, public-sources-only explainer (styled to match the 189–191 Hamilton tools: DM Sans, warm neutrals, badge and KPI-tile components) comparing how delay lands in market-rate and affordable housing deals: the two clocks, who carries the cost, and a $10M "what would you buy" calculator.

No build step. Open `index.html`, or publish with GitHub Pages:

```bash
git init && git add . && git commit -m "Who pays for the wait"
gh repo create who-pays-for-the-wait --public --source=. --push
# then: repo Settings > Pages > Deploy from branch > main / (root)
```

Every number on the page is either linked to a public source or labeled as an adjustable assumption. No deal files, models, or interview material are used.

## Connecting the $10M split form to a Google Sheet

In `index.html`, find `const FORM=` and fill in:

- `action`: the Google Form's `formResponse` URL
- `entry`: the `entry.NNNN` id for each question (name, role, a, b, c, need, mind)

Until then, the Submit button copies the answers instead of sending them.
