# Product page: purchase options change (spec for the website session)

Page: cocoonsupplements.com/products/balance (Shopify, product "BALANCE").
Written Oct 16, 2026 by the ads agent, approved by Rachel before building.

## Why
In June 2026 the page was changed to open on the 3-month supply (Subscribe & Save, CA$159.73). Shopify data for visitors from search (the steadiest traffic source):

| Period | Price | Default | Add-to-cart rate | Purchase rate |
|---|---|---|---|---|
| Nov 2025–Jan 2026 | CA$60 | 1-month | 7.2% | 2.9% |
| Feb–May 2026 | CA$68 (from Mar 1) | 1-month | 5.1% | 2.9% |
| Jun–Oct 15, 2026 | CA$68 | 3-month | 3.1% | 1.8% |

The price increase didn't change the purchase rate. The 3-month default cut it by about 38%. Average order value only rose about 5–10% after June, so revenue per visitor fell by roughly a third. Goal now: more first-time buyers, while keeping subscription as the default and the 3-month offer easy to find.

## What to build

### 1. Default selection on page load
- Pill: **1-month supply** selected.
- Radio: **Subscribe & Save** selected.
- Price block at the top of the page reflects that selection:
  - Canada: **CA$61.20**, with ~~CA$68.00 CAD~~ struck through and the "SAVE 10%" badge.
  - US: **US$45.00**, with ~~US$50.00~~ struck through and "SAVE 10%".
- The price block must always update to match whatever is selected (pill + radio).

### 2. Pill order and labels
- Put **1-month supply** first (left) and **3-month supply** second (right).
- Give the 3-month pill a small badge: **"Best value"**.
- Keep "3-month supply" as the pill text.

### 3. Upsell to 3 months from the 1-month view
Directly under the 1-month radio cards (Subscribe & Save / One-Time Purchase), add one line:

> **Want 3 months? CA$53.24/month, save 22% →**

(US: "US$39.15/month".) Clicking it selects the **3-month supply** pill with **Subscribe & Save** selected. This replaces "3-month right next to it", since the current layout hides 3-month offers behind the pill.

"Save 22%" = CA$53.24 vs CA$68.00 one-time per month. Check the math against live prices; if prices change, compute it, don't hard-code.

### 4. Links from ads must win over the default
Ads and Google price assets link to specific options. If the URL has `?variant=` and/or `selling_plan=`, preselect exactly that option instead of the default:
- `variant=39429510135872` = 1-month supply
- `variant=40492143312960` = 3-month supply
- `selling_plan=578879552` = Subscribe & Save
Check this works today too. If the current 3-month default overrides the URL, ads that link to the 1-month option have been landing on 3-month.

### 5. Prices (for checking only; read them from Shopify, never hard-code)
| | Canada (CAD) | US (USD) |
|---|---|---|
| 1-month, Subscribe & Save | 61.20 | 45.00 |
| 1-month, one-time | 68.00 | 50.00 |
| 3-month, Subscribe & Save | 159.73 (53.24/mo) | 117.45 (39.15/mo) |
| 3-month, one-time | 177.48 (59.16/mo) | 130.50 (43.50/mo) |

### 6. Don't change
Product text, images, reviews, quiz link, guarantee link, subscription app (Appstle) behaviour, checkout. Don't remove the 3-month offers or one-time purchase.

### 7. Tracking must keep working
Use the theme's normal variant and selling-plan selection so Shopify's add-to-cart and checkout events still fire for the Google & YouTube and Facebook & Instagram apps. Don't add custom add-to-cart code that skips the standard cart.

## Check before publishing (desktop and mobile, Canada and US)
1. Fresh visit to /products/balance opens on 1-month + Subscribe & Save, CA$61.20 (US$45.00).
2. Clicking each pill and radio updates the top price correctly.
3. The "Want 3 months?" line switches to 3-month + Subscribe & Save.
4. `/products/balance?variant=40492143312960&selling_plan=578879552` opens on 3-month + Subscribe & Save.
5. `/products/balance?variant=39429510135872` opens on 1-month.
6. Add to cart works for all four options, and the cart shows the right price and subscription.

## After it's live
Tell the ads agent the date and time it went live. It will compare search-traffic add-to-cart rate, purchase rate, average order and new customers for 3 weeks after vs. Jun 1–Oct 15.
