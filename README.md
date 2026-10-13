# Bargain Chemist — Price Match Calculator

A lightweight, standalone web app that works out the price a customer pays under
Bargain Chemist's **Price Promise**: we match a competitor's price and give an
extra **10% off the difference**.

Optimised for mobile / touch-screen use — it looks and behaves like a calculator.

## Formula

```
Customer price = Competitor price − 10% × (BC price − Competitor price)
```

The price match only applies when the **competitor's price is lower** than
Bargain Chemist's price. If the competitor is not lower, the app shows a
"no price match" message.

## Features

- Two price inputs (Bargain Chemist price and Competitor price), entered with an
  on-screen numeric keypad.
- Live formula display showing the substituted numbers.
- Large result readout, with a "no price match" state.
- Brand colours from the Bargain Chemist logo (blue `#25408F`, red `#EB2A25`).
- No dependencies, no build step — a single static `index.html`.

## Tech

- **HTML + CSS + vanilla JavaScript** in one file (`index.html`).
- No frameworks, no bundler, no `node_modules`.

## Usage

Just open `index.html` in any browser. On a phone, tap a field to select it,
then use the keypad.

Physical keyboard is also supported: digits, `.`, `Backspace`, `Escape` (clear),
and `Tab` / arrow keys to switch between the two fields.

## Deploy to Vercel

This is a static site, so deployment needs no configuration:

1. Push this repository to GitHub.
2. In Vercel, **Import** the repository.
3. Framework preset: **Other**. Build command: *(none)*. Output directory: *(root)*.
4. Deploy — Vercel serves `index.html` at the root.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The entire app (markup, styles, logic). |
| `logo_2x.svg` | Bargain Chemist logo used in the header. |
| `idea.md` | Original brief. |
