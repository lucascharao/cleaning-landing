# House Cleaning Service — Landing

Mobile-first landing page for a residential cleaning service in the US.
Reached via QR code on a yard sign. Single static HTML with CSS/SVG animations
(squeegee reveal, floating soap bubbles, sparkles, animated swooshes, shimmer CTA).

## Primary actions
- **Instant Estimate** → in-page calculator (service, beds/baths, sq ft, frequency, extras,
  contact, preferred payment). Submits via WhatsApp (`wa.me`) with all details prefilled.
- **Text us for a FREE quote** → opens SMS to `+1 (470) 707-1177`
- **Call** → dials `+1 (470) 707-1177`

## Pricing
All prices live in the `PRICING` object inside `index.html`.
Base = max(140, 95 + 17·beds + 30·baths, 0.0915·sqft). Deep = base × 1.65, Move In/Out = base × 2.
Recurring discounts (Standard only): weekly 20%, biweekly 15%, monthly 10%. Extras added after discount.

## Payments accepted
Zelle, Venmo, Cash, Check.

## Deploy
Static site. Drop on Vercel (no build step) — `index.html` at root.
