# ESPP Contribution Calculator

A single-file HTML calculator for finding the right contribution rate in a two-period Employee Stock Purchase Plan (ESPP) with a $25K annual IRS limit, 15% discount, and lookback.

## What it does

Given your Period 1 results and Period 2 estimates, it tells you:

- How much of the $25K annual limit you have left for Period 2.
- The maximum shares you can buy in Period 2 before hitting the cap.
- For a chosen contribution rate (1–15%): shares bought, day-1 paper gain, and any auto-refund.
- Whether your rate is **Below**, **Just Under**, **Exact**, **Just Over**, or **Above** the sweet spot — i.e., the lowest rate that captures every available share.

A bar chart shows shares captured at every rate from 1–15%, with sweet-spot rates highlighted in green.

## How it works

- **$25K limit** is measured at grant-date FMV (the IRS rule).
- **Purchase price** = 85% × min(grant-date FMV, purchase-date FMV) — the lookback.
- **Sweet spot** is the contribution rate that buys all cap-allowed shares with the smallest auto-refund. Below it leaves shares on the table; above it just shrinks your paycheck and increases the refund without buying more.

## Usage

Open `index.html` in any modern browser. No build step, no server, no dependencies.

Inputs are saved to `localStorage` on your device. Nothing is transmitted.

## Disclaimer

Estimates only — not financial, tax, or legal advice. Verify against your plan documents and consult a qualified advisor before making contribution decisions.
