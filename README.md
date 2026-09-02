# CUCU TV Payments

Interactive prototype of the CUCU TV parent-insights paywall and its payment flow.

**Live preview:** https://ravi26design.github.io/CUCU-TV-Payments/paywall.html

## What's in it

A single self-contained `paywall.html` — no build step, no dependencies. Open it in any
browser, or use the link above.

### Paywall screen
- Auto-advancing image slider (4 panels, 3.4s interval) with tappable dots and swipe support
- Soft blue header block filling the top 60% of the screen
- Headline plus two feature cards
- Primary CTA — *Unlock Everything for Just ₹9*

### Payment screen
Slides in from the right when the CTA is tapped.
- UPI accordion — Google Pay and PhonePe, single-select
- Credit/Debit card accordion — number, expiry, CVV, name
- Coupon code field
- Sticky bottom bar with the amount and *Pay Now*

### Success modal
*Payment Successful* dialog over a dimmed backdrop; tap anywhere to dismiss.

## Notes

- The payment fields are **visual only** — nothing is submitted, validated, or stored, and
  no payment gateway is connected.
- Payment-method logos are hand-drawn SVG approximations, not official brand marks.
- Slider artwork lives in `images/` as `slide-1.jpg` … `slide-4.jpg`; keep the folder
  alongside `paywall.html`, since the page references the files relatively.
