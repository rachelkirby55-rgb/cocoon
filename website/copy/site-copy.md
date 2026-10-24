# cocoonsupplements.com: site copy

**Version:** draft 1, 21 Oct 2026 · **For:** Rachel (review), then Yuliia (design) and the developer
**Built on:** `website/site-structure.md` (approved 21 Oct 2026), the product briefs and US label copy in `website/product-briefs/source/`, the live-site copy capture (13 Oct 2026), the SEO audit and the navigation/conversion audit.
**Status:** nothing here is live. Every change to Shopify, Typeform or Klaviyo still needs your sign-off.

**Revision note (24 Oct 2026):** this draft predates two decisions, which the next revision applies once Logan's keyword input is in. Balance is now **Estrogen Balance** (`/products/estrogen-balance`), and the brand is just **Cocoon**: no "Cocoon Supplements" and no "formerly Cocoon Skincare" anywhere on the site. The three new-article rows in the blog section are out of scope for now.

---

## How to read this doc

**Legend**

| Tag | Meaning | Who acts |
|---|---|---|
| `[CLAIM CHECK]` | A health, safety, results or combination claim that your regulatory reviewer (and, for safety or stacking, your naturopath) should approve before launch. I'm not a lawyer; these are my best structure/function wordings, not legal clearance. | Rachel + reviewer |
| `[NEED FROM RACHEL: …]` | A fact I don't have and won't invent (prices for bundles, shipping terms, final timeline and so on). | Rachel |
| `[IMAGE: … US packaging]` | Art direction for Yuliia. Every product image uses **US packaging**. | Yuliia |
| `*` | Marks a structure/function claim. Every page with a `*` shows the supplement disclaimer (see Global elements). | Developer |
| `[TIMELINE]` | Short for `[NEED FROM RACHEL: one results timeline]`. The site currently gives three different ones. Once you pick one, paste it everywhere this tag appears. | Rachel |

**Page format.** Each page has: URL · page goal · keywords · SEO title (≤60 characters) · meta description (≤155 characters) · then the copy, top to bottom, in the order it appears on the page. On-page headings are labelled **H1**, **H2**, **H3**. Buttons look like this: **[Button text]** → destination.

**House rules applied throughout**
- Canadian spelling (colour, fibre, favourite, centre).
- "Acne" is used, paired with "supports", "helps maintain" or "targets a root cause of". The words treat, treatment, cure and heal are never used (they appear only inside the legally required disclaimer and in existing blog URLs we must keep).
- "Naturopath-formulated" only. The formulator is never named.
- No mention of an NPN, Health Canada licensing or a "Health Canada licensed facility".
- "Internal skincare" is a brand line, not an SEO keyword (US Keyword Planner: 20 searches a month).
- No reviews, ratings, results or before/afters for Androgen Balance or Liver Support until real customers have them. Those pages use a launch/waitlist angle instead.
- Mobile first (82% of sessions): short paragraphs, one idea per block, buttons high on the page.
- Prices on product pages come from Shopify. New products use the same structure and prices as Balance (1-month or 3-month, one-time or Subscribe & Save).

**Contents**
- Global elements (announcement bar, header, footer, disclaimers)
1. Home `/`
2. Shop All `/collections/skin-supplements`
3. Balance `/products/balance`
4. Androgen Balance `/products/androgen-balance`
5. Liver Support `/products/liver-support`
6. Quiz `/pages/quiz` (plus outcome mapping and result screens)
7. Results `/pages/results`
8. Learn hub `/pages/learn`
9. Concern hubs: estrogen (retitle), androgens (new), liver (new)
10. Blog: new SEO titles and meta descriptions
11. About `/pages/about`
12. FAQ `/pages/faq`
13. Money-back guarantee `/pages/money-back-guarantee`
- Appendix A: How competitors word their claims
- Appendix B: Product names (Keyword Planner)
- Open items

---

## Global elements

### Announcement bar (rotating, sitewide)
Rotate 2 to 3 messages. Swap the first one by launch phase.

| Phase | Message 1 (links to) | Message 2 | Message 3 |
|---|---|---|---|
| Now to Jan 2027 | Coming January 2027: Androgen Balance. **Join the waitlist** → `/products/androgen-balance` (pre-launch page) | Free shipping on orders $70+ and all subscriptions `[NEED FROM RACHEL: confirm this applies to both US and Canada; the live site says "domestic"]` | Not sure where to start? **Take the 2-minute quiz** → `/pages/quiz` |
| Jan to Apr 2027 | New: Androgen Balance is here. **Shop now** → `/products/androgen-balance` | (as above) | Coming April 2027: Liver Support. **Join the waitlist** → `/products/liver-support` |
| From Apr 2027 | New: Liver Support, the booster for your formula. **Shop now** → `/products/liver-support` | (as above) | Try it risk-free: 30-day money-back guarantee → `/pages/money-back-guarantee` |

### Header (menus as already built: "NEW SITE – Main menu (draft)")
- Logo → `/`
- **Shop** ▾: All Supplements · Balance · Androgen Balance · Liver Support · Bundles *(show each new product only from its launch; show Bundles only if you offer them)*
- **Reviews** → `/pages/results`
- **Learn** ▾: How Hormonal Acne Works → `/pages/learn` · Articles → `/blogs/learn`
- **About** → `/pages/about`
- **[Find Your Formula]** → `/pages/quiz`: styled as a button at the right of the header (on mobile, a button at the top of the menu drawer), so it reads as the main action rather than a fifth menu word
- Icons: Search · **Account** ▾ (Log in / My orders · Manage subscription → Appstle portal) · Cart

Search box placeholder text: *Search supplements, ingredients, FAQs*
(40% of site searches were for skincare Cocoon doesn't sell, so the placeholder says "supplements".)

### Footer (menus as already built: "NEW SITE – Footer menu (draft)")

**Brand blurb (footer, left column)**
> **Cocoon Supplements**, formerly Cocoon Skincare. Naturopath-formulated supplements for hormonal acne-prone skin. Internal skincare that gets to a root cause.* `[CLAIM CHECK]`

**Columns**
- **Shop:** All Supplements · Balance · Androgen Balance · Liver Support · Find Your Formula
- **Learn:** How Hormonal Acne Works · Articles · Reviews
- **Help:** FAQ · Money-back guarantee · Shipping · Contact · Manage subscription
- **Company:** About · Affiliates · Wholesale
- **Policies:** Terms · Privacy · Refund policy

**Newsletter block**
- **H3:** Be first to know
- Body: New formulas, members-only offers, and skin and hormone tips. No spam.
- Field placeholder: Your email
- **[Sign me up]**

**Social:** Instagram · TikTok

**Legal line:** © 2026 Cocoon Supplements. `[NEED FROM RACHEL: legal entity name for the footer; labels and Terms say "Cocoon Skincare Inc.", Privacy says "Cocoon Inc."]`

### Sitewide supplement disclaimer (footer, every page; also directly under the buy box and on quiz result screens)
> \*These statements have not been evaluated by the Food and Drug Administration. This product is not intended to diagnose, treat, cure, or prevent any disease. Our content is for education and isn't medical advice. Talk to your healthcare practitioner before starting any supplement, especially if you're pregnant, breastfeeding or taking medication.

### Reviews disclosure (anywhere customer quotes, ratings or before/afters appear)
> Reviews and photos are from real Cocoon customers and reflect their own experience. Individual results vary. `[CLAIM CHECK]` `[NEED FROM RACHEL: typical-results data, e.g. from a customer survey, so we can state what most customers see; FTC]`

### Developer notes (not visible copy)
- Organization schema: `name: "Cocoon Supplements"`, `alternateName: "Cocoon Skincare"`.
- Product type in Shopify: "Supplements". Remove the "Hormonal Acne Treatment" and "Hormonal Pimples Treatment" tags.
- Image alt text: write it from the image notes below, not filenames.

---

## 1. Home

- **URL:** `/` (keep)
- **Page goal:** Send every visitor to the right formula in one tap, or to the quiz if unsure.
- **Primary keyword:** supplements for hormonal acne `[CLAIM CHECK]`
- **Secondary:** hormonal acne supplements; natural supplements for hormonal acne; hormone balance supplements for women (US 2,400/mo); acne supplements for women; Cocoon Supplements; Cocoon Skincare
- **SEO title:** Supplements for Hormonal Acne-Prone Skin | Cocoon
- **Meta description:** Naturopath-formulated supplements that target root causes of hormonal breakouts. Find your formula in 2 minutes. 30-day money-back guarantee.

### Hero
- `[IMAGE: the three bottles side by side, US packaging, warm natural light, soft shadows; mobile crop shows the bottles above the headline. Before Jan 2027: Balance alone.]`
- Eyebrow: Cocoon Supplements, formerly Cocoon Skincare
- **H1:** Internal skincare for hormonal acne `[CLAIM CHECK]`
- Body: Naturopath-formulated supplements that target a root cause of hormonal breakouts: estrogen, androgens, or a liver that needs backup.*
- **[Find my formula]** → `/pages/quiz`
- **[Shop supplements]** → `/collections/skin-supplements`

### Trust strip (4 icons, one line each)
- ★ 4.6 from 92 reviews *(Okendo, pulled live; Balance only)*
- Naturopath-formulated
- 30-day money-back guarantee
- Free shipping on subscriptions

### H2: Supplements for hormonal acne, matched to the root cause `[CLAIM CHECK]`
Intro: Breakouts that keep coming back usually have a reason inside. Pick the formula that fits yours.

**Card 1: Balance**
- `[IMAGE: Balance bottle, US packaging]`
- **H3:** Balance
- Label: For estrogen-linked breakouts
- Body: DIM, glutathione and calcium D-glucarate to support healthy estrogen metabolism.* 1 capsule a day.
- Rating: ★ 4.6 (92 reviews)
- **[Shop Balance]** → `/products/balance`

**Card 2: Androgen Balance**
- `[IMAGE: Androgen Balance bottle, US packaging]`
- **H3:** Androgen Balance
- Label: For androgen-linked breakouts
- Body: Berberine, saw palmetto, zinc, sarsaparilla and NAC to support healthy androgen balance from four angles.* 3 capsules a day.
- Badge: New
- **[Shop Androgen Balance]** → `/products/androgen-balance`

**Card 3: Liver Support**
- `[IMAGE: Liver Support bottle, US packaging]`
- **H3:** Liver Support
- Label: The booster. Pairs with Balance or Androgen Balance `[CLAIM CHECK]`
- Body: Milk thistle, schisandra, dandelion, burdock and R-alpha lipoic acid to support every phase of your liver's natural detox process.* 2 capsules a day. `[CLAIM CHECK]`
- Badge: New
- **[Shop Liver Support]** → `/products/liver-support`

### H2: Not sure which one is yours?
Body: Answer a few questions about your skin, your cycle and your routine. We'll match you to a formula and send your results by email, with 10% off your first order.
- **[Take the 2-minute quiz]** → `/pages/quiz`
- Small print: The quiz is a guide, not a diagnosis.

### H2: Why creams can't reach it
Body: Topicals work on the surface. Hormonal breakouts start further in.
- **Hormones set your oil levels.** When estrogen or androgens run high, skin can make more oil, and pores clog more easily.
- **Your liver clears used hormones.** When it's busy, hormones can hang around longer than they should.
- **That's why breakouts return.** If the root cause hasn't changed, the cycle repeats.

Cocoon formulas work from the inside, alongside your skincare.*
- **[Learn how it works]** → `/pages/learn`

### H2: Fewer ingredients. Meaningful doses.
- **Targeted:** each formula is built around one root cause, not a long list of extras.
- **Naturopath-formulated:** 3 to 5 active ingredients per formula, chosen for what they do.
- **Clean:** vegan, gluten-free, no fillers, no sugar or dyes. `[CLAIM CHECK: confirm free-from claims for the new products; their labels say "made in a facility that handles milk products, gluten, shellfish, soy, peanuts and other tree nuts"]`
- **Plastic-free:** amber glass bottles, to keep plastics away from your hormones.

`[IMAGE: flat lay of capsules and the raw botanicals (milk thistle, saw palmetto berries, broccoli for DIM) next to a US-packaging bottle]`

### H2: Real customers, real skin
Three Balance quotes (chosen to reflect gradual, typical progress):
> "Throughout this past month, I have noticed I am experiencing less new breakouts forming." **Karley, Balance customer**

> "The fourth week is where my acne started to calm down. I get it if you're skeptical, I was too." **Melissa R., Balance customer**

> "My skin is much less inflamed and redness has gone down drastically… I still get breakouts here and there, but nowhere near the level of severity as before." **Alexis, Balance customer**

Reviews disclosure (see Global elements).
- **[See all results]** → `/pages/results`

### H2: Try it for 30 days, risk-free
Body: If your formula isn't the right fit, tell us within 30 days of delivery and we'll refund you. No need to send it back.
- **[How the guarantee works]** → `/pages/money-back-guarantee`

### H2: Learn the root cause
Three article cards:
- Estrogen dominance & acne: signs and natural support → estrogen hub
- High androgens in women: signs, acne and support → androgen hub
- Does coffee cause acne? → coffee post
- **[Visit the Learn hub]** → `/pages/learn`

### Email capture (above footer)
- **H2:** Get 10% off your first order
- Body: Plus tips on skin, hormones and new formulas.
- **[Get my 10%]**

Disclaimer (sitewide version).

### Before each launch (what to show)
| Phase | Hero | Product cards | Extra module |
|---|---|---|---|
| **Now to Jan 2027** | Balance alone. H1 stays. | Balance card only, full width. | **Waitlist module** under the Balance card: "**H3:** Coming January 2027: Androgen Balance. For breakouts linked to high androgens: jawline breakouts, oily skin, unwanted hair. Be first to know, and get early access. **[Join the waitlist]**" `[NEED FROM RACHEL: launch offer for waitlist members, if any]` |
| **Jan to Apr 2027** | Balance + Androgen Balance. | Two cards. | Waitlist module: "**H3:** Coming April 2027: Liver Support. The booster that pairs with Balance or Androgen Balance. **[Join the waitlist]**" |
| **From Apr 2027** | All three. | Three cards. | None. |

Waitlist sign-ups go to a Klaviyo list per product (I haven't created anything; needs your OK).

---

## 2. Shop All

- **URL:** `/collections/skin-supplements` (new; built, unpublished)
- **Page goal:** Help her choose between the three formulas and add one to cart.
- **Primary keyword:** clear skin supplements (US 1,000/mo)
- **Secondary:** acne supplements `[CLAIM CHECK]`; supplements for pimples (US 2,900); vitamins for pimples (2,400); best skin supplements (1,600); skin supplements (1,000); acne supplements canada (GSC 796 impressions)
- **SEO title:** Clear Skin Supplements for Acne-Prone Skin | Cocoon
- **Meta description:** Shop naturopath-formulated supplements for acne-prone skin. Compare Balance, Androgen Balance and Liver Support, or take the 2-minute quiz.

### Header block
- **H1:** Clear skin supplements
- Body: Three naturopath-formulated supplements, each built around a root cause of hormonal breakouts.* Find yours below, or let the quiz match you.
- **[Take the quiz]** → `/pages/quiz`

### Product grid
Shopify product cards (image, name, one-liner, rating where it exists, price "from", **[Add to cart]**). One-liners:
- **Balance:** For estrogen-linked breakouts. 1 capsule a day.
- **Androgen Balance:** For androgen-linked breakouts. 3 capsules a day.
- **Liver Support:** The booster. Pairs with either formula. 2 capsules a day. `[CLAIM CHECK]`

Before launch: show the new products as "Coming January 2027" / "Coming April 2027" cards with **[Join the waitlist]** instead of a price.

### H2: Which formula is right for me?
Mobile: three swipeable columns, or one accordion per row.

| | **Balance** | **Androgen Balance** | **Liver Support** |
|---|---|---|---|
| **Best for** | Breakouts linked to high estrogen | Breakouts linked to high androgens | Extra support alongside either formula `[CLAIM CHECK]` |
| **Common signs** | Breakouts around your chin and jawline that flare before your period; breast tenderness, bloating or mood swings before your period; heavy or painful periods | Breakouts on your jawline or body; oily skin; unwanted hair on your face or body; thinning hair on your head; cycles longer than 35 days; blood sugar swings | A routine with plenty of caffeine, alcohol, medication, packaged foods or sugar; low-protein meals `[CLAIM CHECK]` |
| **Root cause it targets** | Estrogen metabolism* | Androgens, from four angles: blood sugar, DHT conversion, stress and liver processing* | Every phase of your liver's natural detox process* `[CLAIM CHECK]` |
| **Key ingredients** | DIM, glutathione, calcium D-glucarate | Berberine, saw palmetto, zinc, sarsaparilla, NAC | Milk thistle, schisandra, dandelion, burdock, R-alpha lipoic acid |
| **How to take** | 1 capsule a day | 1 capsule, 3 times a day, with food | 1 capsule, twice a day |
| **Bottle** | 30 capsules (1 month) | 90 capsules (1 month) | 60 capsules (1 month) |
| **Pairs with** | Liver Support; Androgen Balance if both are high `[CLAIM CHECK]` | Liver Support; Balance if both are high `[CLAIM CHECK]` | Balance or Androgen Balance `[CLAIM CHECK]` |
| | **[Shop Balance]** | **[Shop Androgen Balance]** | **[Shop Liver Support]** |

Under the table:
- Still unsure? Your answers to the quiz decide it in about 2 minutes. **[Find my formula]**

### H2: Can I take more than one?
Body: Yes, they're designed to work together, and some customers will need two. If the quiz shows both estrogen and androgens are high, it will suggest Balance with Androgen Balance. Liver Support is a booster that pairs with either. Check with your healthcare practitioner before combining supplements. `[CLAIM CHECK: naturopath to confirm all combinations, and how to space them. The Androgen Balance label says to take it "a few hours before or after taking other medication or dietary supplements".]`

### Bundles (only if offered)
`[NEED FROM RACHEL: bundle/stack pricing, or confirm no bundles at launch]`
- **H2:** Build your stack
- Body: Pair your formula with Liver Support and save. `[NEED FROM RACHEL: discount]`

### H2: Every order includes
- Free shipping on subscriptions and orders $70+ `[NEED FROM RACHEL: confirm for Canada]`
- 30-day money-back guarantee
- Subscribe & save 10%. Skip or cancel anytime.

Disclaimer.

---

## 3. Balance

- **URL:** `/products/balance` (keep)
- **Page goal:** Sell Balance to someone with estrogen-linked breakouts, without her needing to leave the page.
- **Primary keyword:** DIM supplement for women (US 5,400/mo; "DIM supplement" 27,100)
- **Secondary:** DIM and calcium D-glucarate (390); DIM estrogen (1,000); DIM supplement for estrogen dominance (390); estrogen balance supplement; Cocoon Balance (brand); DIM supplement for acne `[CLAIM CHECK]`
- **SEO title:** Balance: DIM Supplement for Women | Cocoon Supplements
- **Meta description:** Balance supports healthy estrogen metabolism with DIM, glutathione and calcium D-glucarate, for clearer-looking skin from within. 30-day guarantee.

### Section 1: Buy box
- `[IMAGE gallery, in order: (1) Balance bottle, US packaging, on white; (2) bottle in hand; (3) capsule close-up; (4) Supplement Facts panel, US label; (5) to (7) customer before/afters (Hanna, Hailee, Taylor) with "Individual results vary" caption; (8) "Which formula?" graphic linking to the quiz]`
- **H1:** Balance: DIM supplement for healthy estrogen balance
- One-liner: Naturopath-formulated support for breakouts linked to high estrogen.* `[CLAIM CHECK]`
- Rating: ★ 4.6 · 92 reviews (Okendo, links to Section 6)
- Short description: DIM, glutathione and calcium D-glucarate in meaningful doses, to support healthy estrogen metabolism and clearer-looking skin from within.* One capsule a day.
- **Purchase options (Appstle; Subscribe & Save shown first):**
  - Subscribe & save 10%: 1-month or 3-month delivery. Skip or cancel anytime.
  - One-time purchase: 1-month supply (1 bottle, 30 capsules) or 3-month supply (1 bottle + 2 refill pouches). Badge on 3-month: Best value.
- **[Add to cart]**
- Under the button (3 short lines with icons):
  - Free shipping on subscriptions and orders $70+
  - 30-day money-back guarantee → `/pages/money-back-guarantee`
  - Not sure Balance is for you? **Take the 2-minute quiz →**
- Disclaimer (short form, directly under the buy box): \*These statements have not been evaluated by the FDA. This product is not intended to diagnose, treat, cure, or prevent any disease.

### Section 2: H2: Is Balance for you?
Body: Balance is for adults whose breakouts are linked to high estrogen. You might recognize:
- Breakouts around your chin, jawline or mouth
- Flare-ups in the week or two before your period
- Breast tenderness, bloating or mood swings before your period
- Heavy or painful periods
- Skin that hasn't responded to topicals or prescriptions

`[CLAIM CHECK: these are listed as signs, not as things Balance relieves. The old list's ovarian cysts, fibroids, anxiety, depression, migraines and insomnia are removed because they're disease states.]`

If your breakouts come with oily skin, unwanted hair or long cycles, androgens may be involved. → **Compare formulas** (`/collections/skin-supplements`)
- **[Not sure? Take the quiz]**

### Section 3: H2: How Balance works
Body: Your body is always making estrogen and clearing it out. When it can't keep up, estrogen runs high compared with progesterone. That shift can raise oil production and clog pores. Balance supports the three steps of clearing estrogen:*
1. **Convert.** DIM supports healthy estrogen metabolism, turning estrogen into forms your body can clear more easily.*
2. **Package.** Glutathione supports your liver's normal process of binding substances so they can leave the body.*
3. **Eliminate.** Calcium D-glucarate supports your body's normal process of clearing estrogen through the gut.*

`[IMAGE: simple 3-step diagram, convert → package → eliminate, Cocoon colours]`
- **[Read: estrogen dominance & acne]** → estrogen hub

### Section 4: H2: What's inside
Per capsule (from the Supplement Facts panel):

| Ingredient | Amount | What it does |
|---|---|---|
| **DIM** (3,3'-diindolylmethane) | 150 mg | A compound from cruciferous vegetables like broccoli. Supports healthy estrogen metabolism.* |
| **L-Glutathione** (from 200 mg S-acetyl glutathione) | 176 mg | An antioxidant your liver makes naturally. Supports your body's normal clearing process.* |
| **Calcium D-glucarate** | 150 mg (calcium 13 mg) | A form of glucaric acid, found naturally in the body. Supports the normal elimination of estrogen through the gut.* |

- Other ingredients: vegetable capsule (hypromellose).
- Formulated without: animal-derived ingredients, nuts, soy, gluten, sugar, dyes and GMOs. Never tested on animals.
- Made in Canada under GMP standards. Third-party tested for purity.
- Packaged in amber glass bottles and paper-based refill pouches.
- **[View Supplement Facts]** (opens the US label image)

### Section 5: H2: What to expect
Body: Hormones shift gradually, so Balance works best taken every day. [TIMELINE]

Three steps (layout as a timeline; fill in from [TIMELINE]):
- **Weeks [ ]:** Stay consistent. Some people notice mild, short-lived changes such as darker urine, gas or a headache as their body adjusts. `[CLAIM CHECK]`
- **Weeks [ ]:** Be patient. Many customers start to notice fewer new breakouts.* `[CLAIM CHECK]`
- **Month [ ] and beyond:** Keep going. `[CLAIM CHECK]`

Tip: take it with food at the same time each day.

### Section 6: H2: Results and reviews
- Okendo widget: rating summary (4.6, 92 reviews, 93% would recommend) and all reviews.
- Before/after carousel: Hanna (2 months), Hailee (1 month), Taylor. Caption on every image: "Individual results vary."
- Reviews disclosure.

### Section 7: H2: Safety questions
Accordion.

**Can I take Balance on birth control?**
Talk to your healthcare practitioner first. They can look at your full picture, including the type of birth control you use. `[NEED FROM RACHEL: naturopath's position on Balance with hormonal birth control and IUDs; a 2026 review asked about this]` `[CLAIM CHECK]`

**Can I take it if I'm pregnant or breastfeeding?**
No. Don't use Balance if you're pregnant or breastfeeding.

**Can I take it with other supplements or medication?**
Check with your healthcare practitioner before combining Balance with any medication or supplement.

**Are there side effects?**
Most people take Balance without issues. Some notice mild, short-lived changes in the first weeks, such as darker urine, gas, headaches, tiredness or changes in stool. Your skin may also get a little worse before it gets better. Taking it with food and drinking plenty of water can help. If it bothers you, take 1 capsule every 2 or 3 days for 2 weeks, then return to daily. If it continues, stop and talk to your practitioner. `[CLAIM CHECK]`

**Can men take Balance?**
Yes. Balance is for adults over 18, and men can take it too.

**Who shouldn't take it?**
Anyone under 18, pregnant or breastfeeding. If you're approaching or in menopause, talk to your practitioner before starting.

### Section 8: H2: Pairs well with
- **Liver Support:** a booster for your liver, which does a lot of the work of clearing estrogen.* **[Add Liver Support]** `[CLAIM CHECK]` (from Apr 2027)
- **Androgen Balance:** if your quiz results show high androgens as well as high estrogen.* **[See Androgen Balance]** `[CLAIM CHECK]` (from Jan 2027)
- Before launch: "Coming soon" with **[Join the waitlist]**.

### Section 9: H2: Risk-free, and flexible
- **30-day money-back guarantee.** Not the right fit? Tell us within 30 days of delivery for a refund. No need to send it back. **[Read the terms]**
- **Subscribe & save 10%.** Delivered every 1 or 3 months. Skip, swap or cancel anytime from your account.
- **Free shipping** on subscriptions and orders $70+.

### Section 10: Disclaimer
Full sitewide disclaimer.

---

## 4. Androgen Balance

- **URL:** `/products/androgen-balance` (new)
- **Page goal:** Sell Androgen Balance to someone with androgen-linked breakouts (and capture waitlist sign-ups before Jan 2027).
- **Primary keyword:** anti-androgen supplement (US 590/mo, CA 70) `[CLAIM CHECK: "anti-androgen" names a drug class; reviewer to confirm we can use it in the title. Fallback: "supplement for high androgens".]`
- **Secondary:** DHT blocker for women (US 8,100, CA 320; mostly hair-loss intent); saw palmetto for women (US 12,100, CA 1,000); androgen blocker supplement (140); supplements to lower androgens (50); berberine and NAC (40)
- **SEO title:** Androgen Balance: Anti-Androgen Supplement | Cocoon
- **Meta description:** Berberine, saw palmetto, zinc, sarsaparilla and NAC to support healthy androgen balance and clearer-looking skin. Naturopath-formulated.

*Keyword note: Keyword Planner suppresses every term containing "acne", so acne-specific volumes are unknown. Data: Google Keyword Planner via Windsor, US and Canada, English, pulled 21 Oct 2026.*

### Section 1: Buy box
- `[IMAGE gallery: (1) Androgen Balance bottle, US packaging, on white; (2) bottle in hand; (3) capsule close-up; (4) Supplement Facts panel, US label; (5) "4 angles" graphic (blood sugar, DHT, stress, liver); (6) "Which formula?" graphic. NEED FROM RACHEL: Yuliia's packaging design. No before/afters until real customers have them.]`
- **H1:** Androgen Balance: support for androgen-linked breakouts `[CLAIM CHECK]`
- One-liner: Naturopath-formulated to support healthy androgen balance from four angles: blood sugar, DHT, stress and liver.*
- Badge: New
- *(No star rating until reviews exist. Okendo shows "Be the first to review" from launch.)*
- Short description: Five ingredients in meaningful doses, for breakouts on your jawline or body, oily skin and other signs of high androgens.* 3 capsules a day, with food. `[CLAIM CHECK]`
- **Purchase options** (same as Balance): Subscribe & save 10% (1-month or 3-month) · One-time 1-month (1 bottle, 90 capsules) or 3-month. Badge on 3-month: Best value. `[NEED FROM RACHEL: is the 3-month option 3 bottles, or 1 bottle + 2 refills like Balance?]`
- **[Add to cart]**
- Under the button: Free shipping on subscriptions and orders $70+ · 30-day money-back guarantee · Ships to Canada from our US warehouse `[NEED FROM RACHEL: confirm wording and Canadian shipping terms]` · Not sure? **Take the 2-minute quiz →**
- Short disclaimer.

**Pre-launch version (publish about 4 to 6 weeks before Jan 2027)** `[NEED FROM RACHEL: go-ahead and date]`
- Same H1 and one-liner, with eyebrow "Coming January 2027".
- Replace price and Add to cart with: "Be first to know when it launches. **[Join the waitlist]**" `[NEED FROM RACHEL: any waitlist offer]`
- Keep Sections 2, 3, 4 and 7. Hide Sections 5 and 6.

### Section 2: H2: Is Androgen Balance for you?
Body: Androgen Balance is for adults whose breakouts are linked to high androgens, such as testosterone and DHT. You might recognize:
- Breakouts on your jawline, chin or body
- Oily skin
- Unwanted hair on your face, chin or body
- Thinning hair on your head
- Long cycles (35 days or more) or irregular ovulation
- Blood sugar swings, or cravings that feel hard to manage

`[CLAIM CHECK: listed as signs, not as things the product relieves. Ovarian cysts and ovulation pain from the brief are left out as disease/medical states.]`

High androgens are common with PCOS. If you have PCOS, or think you might, talk to your healthcare practitioner, who can test your hormone levels. `[CLAIM CHECK]`

If your breakouts flare mainly before your period, with breast tenderness or bloating, estrogen may be the bigger factor. → **See Balance**
- **[Not sure? Take the quiz]**

### Section 3: H2: How Androgen Balance works
Body: Androgens are hormones everyone makes. When they run high, or more testosterone turns into DHT, skin can make more oil and pores clog more easily. Androgen Balance supports healthy androgen levels from four angles at once:*

1. **Blood sugar: Berberine.** High insulin can push your body to make more androgens. Berberine supports healthy blood sugar balance, the anchor of the formula.* `[CLAIM CHECK]`
2. **DHT: Saw palmetto + zinc.** Help reduce the conversion of testosterone into DHT, the androgen most linked to oily, breakout-prone skin.* Zinc also supports healthy skin.* `[CLAIM CHECK]`
3. **Stress: Sarsaparilla.** Supports a healthy stress response, so cortisol doesn't keep nudging androgens higher.* `[CLAIM CHECK]`
4. **Liver: NAC.** Supports phase 2 liver detoxification and healthy insulin sensitivity.* `[CLAIM CHECK]`

`[IMAGE: 4-angle diagram (blood sugar, DHT, stress, liver) around the bottle, US packaging]`
- **[Read: high androgens in women]** → androgen hub

### Section 4: H2: What's inside
Per serving (3 capsules), from the US label:

| Ingredient | Amount | What it does |
|---|---|---|
| **N-Acetyl-L-cysteine (NAC)** | 600 mg | Supports phase 2 liver detoxification and healthy insulin sensitivity.* `[CLAIM CHECK]` |
| **Berberine HCl** | 500 mg | Supports healthy blood sugar balance.* `[CLAIM CHECK]` |
| **Saw palmetto extract** (*Serenoa repens*, fruit) | 320 mg | Helps reduce the conversion of testosterone into DHT.* `[CLAIM CHECK]` |
| **Sarsaparilla extract** (*Smilax officinalis*, root) | 120 mg | Supports a healthy stress response.* `[CLAIM CHECK]` |
| **Zinc** (as zinc gluconate) | 20 mg (182% DV) | Supports healthy skin and works with saw palmetto.* `[CLAIM CHECK]` |

- Other ingredients: vegetable shell (hypromellose).
- Only 5 active ingredients. No fillers or additives. Plastic-free glass bottle.
- Made in Canada from imported ingredients.
- Free-from and testing claims: `[CLAIM CHECK: brief says "same as Balance" (vegan, gluten-free, third-party tested, GMP). Confirm with the manufacturer, and note the label's allergen line: "made in a facility that handles milk products, gluten, shellfish, soy, peanuts and other tree nuts".]`
- **[View Supplement Facts]**

### Section 5: H2: What to expect
Body: Androgens shift gradually. Take Androgen Balance every day, with food. [TIMELINE]
- The label advises checking in with your healthcare practitioner for use beyond 3 months. `[CLAIM CHECK: this needs to fit whatever [TIMELINE] says, and the subscription messaging]`

*(Hide this section on the pre-launch page.)*

### Section 6: H2: Reviews
- **Before reviews exist:** "**H3:** Be one of the first. Androgen Balance is new, so there are no reviews yet. Tried it? Tell us how it's going. **[Write a review]**" `[NEED FROM RACHEL: whether to run an early-reviewer program; any incentive must be disclosed in the review]`
- Optional while new: "See what Balance customers say" → `/pages/results` (clearly labelled as Balance reviews).

### Section 7: H2: Safety questions

**Who shouldn't take Androgen Balance?**
Don't use it if you're pregnant or breastfeeding, or if you're taking antibiotics or nitroglycerin. It's for adults only.

**Can I take it with birth control or spironolactone?**
Talk to your healthcare practitioner before starting if you take any medication or other supplements. Take Androgen Balance a few hours before or after other medication or supplements. `[CLAIM CHECK]` `[NEED FROM RACHEL: naturopath's guidance on hormonal birth control and spironolactone]`

**Can I take it with Balance?**
`[CLAIM CHECK: naturopath to confirm.]` Draft: Yes, they can be taken together if your quiz results show both high androgens and high estrogen. Space them a few hours apart. `[NEED FROM RACHEL: a simple daily schedule. Androgen Balance is taken 3 times a day with food and a few hours apart from other supplements, so we need to say when Balance fits.]`

**Are there side effects?**
`[NEED FROM RACHEL: naturopath's list of possible side effects]` Take it with food. If you have kidney stones, talk to your practitioner before use. Long-term zinc use may contribute to copper deficiency, so check in with your practitioner if you plan to take it for more than 3 months. If anything doesn't feel right, stop and talk to your practitioner.

**Can I take it long term?**
Check with your healthcare practitioner for use beyond 3 months.

**Can men take it?**
`[NEED FROM RACHEL: confirm. The brief describes women; the label includes a prostate warning ("consult a healthcare practitioner… to rule out prostate cancer"), which implies men may use it.]`

### Section 8: H2: Pairs well with
- **Liver Support:** a booster for the liver side of the formula.* **[Add Liver Support]** `[CLAIM CHECK]` (from Apr 2027; before then, **[Join the waitlist]**)
- **Balance:** if your quiz shows high estrogen as well.* **[See Balance]** `[CLAIM CHECK]`

### Section 9: H2: Risk-free, and flexible
Same copy as Balance, Section 9. `[NEED FROM RACHEL: confirm the 30-day guarantee covers the new products, and whether it's once per customer or once per product]`

### Section 10: Disclaimer
Full sitewide disclaimer.

---

## 5. Liver Support

- **URL:** `/products/liver-support` (new)
- **Page goal:** Sell Liver Support as the add-on to Balance or Androgen Balance (and capture waitlist sign-ups before Apr 2027).
- **Primary keyword:** liver support supplement (US 18,100/mo, CA 1,900)
- **Secondary:** liver health supplement (US 33,100, CA 2,400); liver support with milk thistle (1,900); milk thistle supplement (14,800); liver detox supplement (US 9,900, CA 880) `[CLAIM CHECK]`
- **SEO title:** Liver Support Supplement with Milk Thistle | Cocoon
- **Meta description:** The booster for your formula. Milk thistle, schisandra, dandelion, burdock and R-ALA support every phase of your liver's natural detox process.

### Section 1: Buy box
- `[IMAGE gallery: (1) Liver Support bottle, US packaging, on white; (2) Liver Support next to Balance and next to Androgen Balance, US packaging ("the stack"); (3) capsule close-up; (4) Supplement Facts panel, US label; (5) "activate → process → eliminate" graphic. NEED FROM RACHEL: Yuliia's packaging design.]`
- **H1:** Liver Support: the booster for clearer-looking skin `[CLAIM CHECK]`
- One-liner: A naturopath-formulated liver supplement that supports every phase of your liver's natural detox process, and pairs with Balance or Androgen Balance.* `[CLAIM CHECK]`
- Badge: New
- *(No star rating until reviews exist.)*
- Short description: Your liver processes hormones along with everything else you eat, drink and use. Liver Support gives it backup.* 2 capsules a day.
- **Purchase options** (same as Balance): Subscribe & save 10% · One-time 1-month (1 bottle, 60 capsules) or 3-month. `[NEED FROM RACHEL: 3-month format; bundle price with Balance or Androgen Balance]`
- **[Add to cart]**
- Under the button: Free shipping on subscriptions and orders $70+ · 30-day money-back guarantee · Ships to Canada from our US warehouse `[NEED FROM RACHEL]` · Not sure? **Take the quiz →**
- Short disclaimer.

**Pre-launch version (about 4 to 6 weeks before Apr 2027):** eyebrow "Coming April 2027", **[Join the waitlist]** in place of the price. Keep Sections 2, 3, 4 and 7.

### Section 2: H2: Is Liver Support for you?
Body: Liver Support is a booster. It's designed to pair with Balance or Androgen Balance rather than to work on one hormone imbalance by itself. It may be a good fit if your breakouts are hormonal and your routine includes:
- Coffee or other caffeine most days
- Alcohol
- Regular medication, including hormonal birth control
- Packaged foods or added sugar
- Plastics, or non-natural personal care and cleaning products
- Non-organic meat, dairy or produce
- Meals low in protein

`[CLAIM CHECK: brief asks to confirm these are all processed by the liver.]`
- **[Find your main formula with the quiz]**

### Section 3: H2: How Liver Support works
Body: Your liver clears used hormones in three phases. If one phase gets backed up, hormones can circulate longer than they should. Liver Support covers all three.*
1. **Strengthen: Milk thistle.** Supports liver resilience and helps recycle glutathione.* `[CLAIM CHECK]`
2. **Balance: Schisandra.** Helps keep phase 1 from getting ahead of phase 2.* `[CLAIM CHECK]`
3. **Move it out: Dandelion + burdock.** Support bile flow and digestion, the routes your body uses to clear what the liver has processed.* `[CLAIM CHECK: the brief also lists lymph and kidneys]`
4. **Protect: R-alpha lipoic acid.** An antioxidant that supports cellular protection.* `[CLAIM CHECK]`
5. **Skin: Burdock.** Traditionally used for congested skin.* `[CLAIM CHECK]`

`[IMAGE: liver pathway diagram, activate → process → eliminate]`
- **[Read: your liver and your skin]** → liver hub

### Section 4: H2: What's inside
Per serving (2 capsules), from the US label:

| Ingredient | Amount | What it does |
|---|---|---|
| **Milk thistle extract** (seed), standardized to 80% silymarin (160 mg) | 200 mg | Supports liver resilience and glutathione recycling.* |
| **Dandelion** (root) | 120 mg | Supports bile flow and digestion.* |
| **Burdock** (root) | 100 mg | Supports elimination and congested skin.* |
| **R-alpha lipoic acid** (from 125 mg sodium R-alpha-lipoate) | 100 mg | Antioxidant support for cells.* |
| **Schisandra** (*Schisandra chinensis*, fruit) | 80 mg | Helps balance phase 1 and phase 2 liver detox.* |

All descriptions `[CLAIM CHECK]`.
- Other ingredients: vegetable shell (hypromellose).
- Only 5 active ingredients. No fillers or additives. Plastic-free glass bottle.
- Made in Canada from imported ingredients.
- Free-from and testing claims: `[CLAIM CHECK: same note as Androgen Balance, including the facility allergen line]`
- **[View Supplement Facts]**

### Section 5: H2: What to expect
Body: Take 1 capsule twice a day, alongside your main formula. [TIMELINE] `[CLAIM CHECK: the US label says "Use for at least 3 weeks to see beneficial effects". The final timeline must agree with the label.]`

### Section 6: H2: Reviews
Same "Be one of the first" block as Androgen Balance.

### Section 7: H2: Safety questions

**Who shouldn't take Liver Support?**
Don't use it if you're pregnant or breastfeeding. Talk to your healthcare practitioner first if you have diabetes, a liver or biliary disorder, or an intestinal obstruction.

**Are there side effects?**
You may notice a diuretic effect (needing to pee more). Stop and talk to your practitioner if you notice sweating, paleness, chills, headache, dizziness or confusion, as these may be signs of low blood sugar. Stop if you have an allergic reaction.

**Can I take it with Balance or Androgen Balance?**
`[CLAIM CHECK: naturopath to confirm.]` Draft: Yes, that's what it's made for. Liver Support pairs with either formula. `[NEED FROM RACHEL: naturopath to check Liver Support + Androgen Balance together, since berberine supports blood sugar balance and the Liver Support label warns about low blood sugar.]`

**Can I take it with medication?**
Talk to your healthcare practitioner before combining it with any medication.

**Can men take it?**
`[NEED FROM RACHEL: confirm]`

### Section 8: H2: Pairs well with
- **Balance:** for estrogen-linked breakouts.* **[Add Balance]**
- **Androgen Balance:** for androgen-linked breakouts.* **[Add Androgen Balance]**
- Bundle: `[NEED FROM RACHEL: stack price]`

### Section 9: H2: Risk-free, and flexible
Same as Balance, Section 9.

### Section 10: Disclaimer
Full sitewide disclaimer.

---

## 6. Quiz

- **URL:** `/pages/quiz` (keep). The quiz itself stays on `/pages/typeform` (Typeform `WqZpjXT7`). Set `/pages/typeform` to `noindex`.
- **Page goal:** Match her to the right formula and capture her email.
- **Primary keyword:** acne quiz (GSC 851 impressions at position 32, 81% of quiz-cluster impressions from the US)
- **Secondary:** what type of acne do I have quiz (572); what is causing my acne quiz (344, position 12); hormonal acne quiz (265, position 2.4); hormone imbalance quiz
- **SEO title:** Acne Quiz: What Type of Acne Do I Have? | Cocoon
- **Meta description:** Take our free 2-minute acne quiz to find out which hormones may be behind your breakouts, and which Cocoon formula fits your skin.

### Landing page copy (indexable, about 300 words)
- `[IMAGE: woman on phone, natural light, Balance bottle (US packaging) on the table]`
- **H1:** Acne quiz: what's behind your breakouts?
- Body: Two minutes, a few questions about your skin, your cycle and your routine. We'll show which hormone imbalance your answers point to, and match you with a formula.
- **[Start the quiz]** → `/pages/typeform`
- Small print: Free. Results by email, plus 10% off your first order.

**H2:** What type of acne do I have?
Body: Breakouts that started in your teens are often driven by puberty. Adult breakouts that keep coming back are more often hormonal. Hormonal breakouts tend to:
- Appear around your chin, jawline and mouth
- Flare at the same point in your cycle
- Hang on despite topicals or prescriptions

**H2:** What the quiz looks at
- **Where and when you break out.** Location and timing are clues to which hormone is involved.
- **Symptoms beyond your skin.** Your cycle, mood, hair and cravings help tell estrogen from androgens.
- **Your routine.** Food, products, medication and caffeine all affect how hard your liver works.

**H2:** What you'll get
- The hormone pattern your answers point to: high estrogen, high androgens, or both
- The Cocoon formula that matches it, and whether Liver Support could help
- Your results by email, with 10% off

Reassurance line: Nothing to buy to see your result.

Small print: This quiz is a simplified guide, not a diagnosis or medical advice. The best way to check your hormones is with your healthcare practitioner.

- **[Start the quiz]** (repeat at the bottom)

### Recommended outcome → product mapping
Keep the existing Typeform branching and scoring. Change what each result screen recommends, and add a link to the product on every screen (today the end screens link nowhere).

| Quiz outcome (existing) | Now to Jan 2027 | Jan to Apr 2027 | From Apr 2027 |
|---|---|---|---|
| Estrogen dominance ("may be" or "likely") | Balance | Balance | Balance, + Liver Support module if 2+ liver factors |
| High androgens | Waitlist for Androgen Balance (email capture) | Androgen Balance | Androgen Balance, + Liver Support module if 2+ liver factors |
| High androgens + high estrogen | Balance now, plus Androgen Balance waitlist `[CLAIM CHECK]` | Androgen Balance + Balance `[CLAIM CHECK]` | Same, + Liver Support module if 2+ liver factors |
| No clear imbalance | Practitioner referral + learning (no product) | Same | Same. Optional: show Liver Support if 3+ liver factors `[NEED FROM RACHEL: decide; it fits the "booster" positioning less well]` |
| Under 18 (puberty) / menopause | Practitioner referral (no product) | Same | Same |

**Suggested quiz additions** (needs your OK to edit the Typeform)
1. Add to the androgen symptom question: "Oily skin" · "Cycles longer than 35 days" · "Blood sugar swings or insulin resistance". (From the Androgen Balance brief.)
2. New question, so the Liver Support module has something to score: "Which of these are part of your usual week? (pick all that apply)" Coffee or other caffeine most days · Alcohol a few times a week or more · Regular medication, including birth control · Packaged foods or added sugar · Meals low in protein · None of these. The existing "use/consume regularly" question (plastics, non-organic food, non-natural products) also counts. `[CLAIM CHECK]`
3. Rename "Which of the following treatments have you tried?" to "What have you already tried for your skin?"
4. Delete the default Typeform end screen ("Now create your own typeform").

### Result screens (Typeform)
Every result screen: heading · explanation · piped symptoms · match · email capture · product button. The disclaimer goes at the bottom of each screen.

**Result A1: "Likely" estrogen dominance**
- **Heading:** Your answers point to high estrogen.
- Body: Estrogen dominance means estrogen is high compared with progesterone. That shift can set off a chain reaction that ends in extra oil, clogged pores and breakouts, often around your chin and jawline, and often before your period.
- Your top signs: {{primary symptoms}} · Also noticed: {{secondary symptoms}}
- **Your match: Balance.** DIM, glutathione and calcium D-glucarate to support healthy estrogen metabolism.* One capsule a day. 4.6★ from 92 reviews.
- Email capture: Enter your email for your full results and 10% off your first order.
- **[Get my results + 10% off]** then **[Shop Balance]** → `/products/balance`

**Result A2: "May be" estrogen dominance**
- **Heading:** Estrogen may be part of your picture.
- Body and match: as A1, with the first line "You have more than one sign of high estrogen."

**Result B: High androgens**
- **Heading:** Your answers point to high androgens.
- Body: Androgens like testosterone are hormones everyone makes. When they run high, more testosterone can turn into DHT, which tells your skin to make more oil. That can mean oily skin and breakouts on your jawline or body, sometimes with unwanted hair.
- Your top signs: {{primary}} · Also noticed: {{secondary}}
- High androgens are common with PCOS. If you haven't already, talk to your healthcare practitioner, who can test your levels. `[CLAIM CHECK]`
- **From Jan 2027: Your match: Androgen Balance.** Berberine, saw palmetto, zinc, sarsaparilla and NAC to support healthy androgen balance from four angles.* **[Get my results + 10% off]** then **[Shop Androgen Balance]**
- **Before Jan 2027 (waitlist version):** We're launching a formula made for this: **Androgen Balance, coming January 2027.** Enter your email for your full results, and we'll tell you the moment it's ready. **[Get my results + join the waitlist]** `[NEED FROM RACHEL: launch offer for these sign-ups]`
- *(The old line "DIM has anti-androgenic properties" is removed: it's a drug-like claim and it oversells Balance for this outcome.)*

**Result C: High androgens and high estrogen**
- **Heading:** Your answers point to both high androgens and high estrogen.
- Body: These two often travel together. When testosterone is high, the body can make more estrogen to compensate, and the two imbalances feed each other. Both can raise oil and clog pores.
- Your top signs: {{primary}} · Also noticed: {{secondary}}
- PCOS line (as B).
- **From Jan 2027: Your match: Androgen Balance + Balance.** One formula for each side.* `[CLAIM CHECK: combination and timing]` **[Get my results + 10% off]** then **[Shop both]** (bundle link if offered) `[NEED FROM RACHEL: bundle]`
- **Before Jan 2027:** Start with **Balance** for the estrogen side today, and we'll let you know when **Androgen Balance** launches in January. `[CLAIM CHECK]` **[Get my results + 10% off]** then **[Shop Balance]**

**Module L: Liver Support add-on (from Apr 2027; shown on A, B and C when 2+ liver factors are ticked)**
- **H3:** Give your formula a boost
- Body: You told us {{liver factors}} are part of your week. Your liver processes all of those, along with your hormones. Liver Support pairs with your formula to support every phase of your liver's natural detox process.* `[CLAIM CHECK]`
- **[Add Liver Support]**

**Result D: No clear imbalance**
- **Heading:** Your answers don't point to one hormone imbalance.
- Body: That's useful to know. Breakouts can still be hormonal without other symptoms, so your healthcare practitioner is the best next step for a closer look. Meanwhile, our Learn hub covers the other common triggers, from stress to diet.
- Email capture: Want to keep learning? Enter your email for skin and hormone tips, plus 10% off if you decide to try a formula.
- **[Visit the Learn hub]**

**End screen E1: Under 18**
- **Heading:** Your breakouts may be part of puberty.
- Body: Teen breakouts are driven by the hormone surge that's a normal part of growing up. Our formulas are for adults over 18, so please talk to your healthcare practitioner about next steps.

**End screen E2: Menopause**
- **Heading:** You may be approaching or in menopause.
- Body: Hormones shift a lot around menopause, so it's worth checking your levels with your healthcare practitioner before adding a supplement. They can help you decide what fits.

**End screen E3: Thank you**
- **Heading:** Thanks for taking the quiz.
- Body: Check your inbox for your results. Your 10% code is in there too.
- **[Shop all formulas]** → `/collections/skin-supplements`

Disclaimer on every screen: \*These statements have not been evaluated by the FDA. This product is not intended to diagnose, treat, cure, or prevent any disease. This quiz is not medical advice.

*(Removed from the old screens: "almost 80% of the population" and "Balance is a safe and effective way… improving acne", both unsourced or disease claims.)*

---

## 7. Results

- **URL:** `/pages/results` (keep). 301 `/pages/results-1` and `/pages/reviews` here.
- **Page goal:** Prove it works for people like her, then send her to the product.
- **Primary keyword:** Cocoon reviews
- **Secondary:** Cocoon Skincare reviews (365 impressions on this page); Cocoon Balance reviews; Cocoon supplement reviews; Balance before and after
- **SEO title:** Cocoon Reviews: Before & After Customer Results
- **Meta description:** Real reviews and before-and-after photos from Cocoon customers (formerly Cocoon Skincare). 4.6 stars from 92 reviews. See what to expect.

### Header
- **H1:** Cocoon reviews and real results
- Body: Photos and words from real customers, unfiltered. Every skin is different, so these show a range of experiences.
- Rating line: ★ 4.6 from 92 reviews · 93% would recommend *(Okendo, live)*

### H2: Before and after
Before/after gallery, one card per customer: photo pair, name, timeframe label ("After 1 month", "After 2 months"), short quote. Keep Hanna, Hailee, Karley, Alexis, Paloma, Paulina, Kim and Taylor. Caption on every card: "Individual results vary."

Suggested quotes (trimmed from the existing page; keep the full quote in an expander):
- **Hanna, after 2 months:** "Two months in, and my skin is basically clear!"
- **Hailee, after 1 month:** "After about 30 days I noticed a difference, but after 90 days my skin is literally glowing!"
- **Karley, after 1 month:** "I have noticed I am experiencing less new breakouts forming."
- **Alexis, after 1 month:** "My skin is much less inflamed… I still get breakouts here and there, but nowhere near the level of severity as before."
- **Paloma, after 1 month:** "Within a few weeks, my skin started clearing up, and my confidence grew."

`[CLAIM CHECK: FTC requires these to reflect typical results or carry a clear disclosure. The disclosure is there; typical-results data would make it stronger. "Michelle" (period regularity) and "Krista Z." (95% clearer) are dropped as menstrual/strong outcome claims.]`

### H2: All reviews
Okendo all-reviews widget (moved here from `/pages/reviews`), filterable by product once the new products have reviews.

Note above the widget, from Jan 2027: Androgen Balance and Liver Support are new. Their reviews will appear here as customers share them.

### H2: Ready to start?
- **[Find my formula]** → quiz
- **[Shop Balance]** → `/products/balance`

Reviews disclosure + disclaimer.

---

## 8. Learn hub

- **URL:** `/pages/learn` (keep). Fix the broken links: the "period pimples" link (404) → menstrual-cycle section of the hub or the acne-types post; the Genetics "Learn more" button (no link) → remove; `/products/dim` links → `/products/balance`.
- **Page goal:** Explain the root causes, then route her to the matching concern hub, the quiz or a product.
- **Primary keyword:** hormonal acne (GSC 470 impressions, position 47)
- **Secondary:** how to balance hormones for acne (948); hormonal acne causes; hormonal acne types; fungal acne vs hormonal acne (~280 at 16 to 21); hormonal chin acne
- **SEO title:** Hormonal Acne: Causes, Types & What Helps | Cocoon
- **Meta description:** What causes hormonal acne? Learn the signs, the three root causes (estrogen, androgens and your liver) and what can help, from diet to supplements.

### Header
- `[IMAGE: calm editorial shot, woman's jawline in natural light, no product]`
- **H1:** Hormonal acne: causes, types and what helps
- Body: If your breakouts outlasted your teens and shrug off every cream, hormones are probably involved. Here's how to tell, and what's going on underneath.

### H2: How do I know if my acne is hormonal?
Hormonal acne usually:
- Continues past your teens, or starts in your 20s or 30s
- Shows up around your chin, jawline and mouth
- Flares at the same point in your cycle
- Resists topicals or medication

**H3:** Hormonal acne or fungal acne?
Fungal acne looks like small, uniform, itchy bumps, often on the forehead, chest or back. Hormonal breakouts tend to be deeper and tender, around the lower face, and tied to your cycle. If you're not sure, a dermatologist can tell you.

**H3:** Why the chin and jawline?
The skin on your lower face is especially sensitive to androgens, the hormones that drive oil production. That's why hormonal breakouts cluster there.

### H2: The three root causes we focus on
Body: Every breakout involves hormones. These three are the ones we see most often in adult women.

**Card 1: High estrogen**
- When estrogen runs high compared with progesterone, the balance tips toward more oil and clogged pores. Often comes with breakouts before your period, breast tenderness and bloating.
- **[Estrogen dominance & acne]** → estrogen hub · **[Meet Balance]**

**Card 2: High androgens**
- Testosterone and DHT tell your skin to make oil. When they run high, you may notice oily skin, jawline or body breakouts and unwanted hair.
- **[High androgens in women]** → androgen hub · **[Meet Androgen Balance]** (from Jan 2027)

**Card 3: An overloaded liver**
- Your liver clears used hormones, plus caffeine, alcohol, medication and more. When it's busy, hormones can circulate longer.
- **[Your liver and your skin]** → liver hub · **[Meet Liver Support]** (from Apr 2027)

- **[Which one is mine? Take the quiz]**

### H2: Other triggers that make it worse
Short tiles, each linking to a post:
- **Your cycle:** hormone shifts in the second half of your cycle can bring breakouts on schedule. → acne-types post
- **Stress:** cortisol can tip your hormone balance. → stress post
- **Diet:** what you eat affects how hormones are made and cleared. → diet post (merged)
- **Coffee:** does caffeine make it worse? → coffee post
- **Chemicals:** xenoestrogens in plastics and products can act like estrogen. → xenoestrogens post
- **Medication:** how prescriptions work, and what happens when you stop. → acne medications post
- **Genetics:** your genes shape how you make and clear hormones. *(no link)*

### H2: What helps
- **Topicals** calm the surface. → AM & PM routine post
- **Food and lifestyle** support your hormones day to day. → diet post
- **Targeted supplements** work on the root cause from inside.* → **[Compare formulas]** `[CLAIM CHECK]`

Disclaimer.

---

## 9. Concern hubs

### 9a. Estrogen dominance & acne (existing post, retitle only)
- **URL:** `/blogs/learn/estrogen-dominance-acne` (renamed from estrogen-dominance-in-women-symptoms-causes-and-natural-treatment, with a 301)
- **Page goal:** Rank for estrogen dominance + acne and feed Balance.
- **Primary keyword:** estrogen dominance acne (GSC 371 impressions at 11.0)
- **Secondary:** estrogen dominance (US 8,100); low progesterone acne (~450 at ~20); female too much estrogen (720); supplements for estrogen dominance (320)
- **SEO title:** Estrogen Dominance & Acne: Signs and Natural Support
- **Meta description:** What estrogen dominance is, how it shows up on your skin, and natural ways to support healthy estrogen balance, from diet to DIM. Take the quiz.
- **H1:** Estrogen dominance and acne: signs, causes and natural support
- Add a product module after the "causes" section: "**H3:** Made for estrogen-linked breakouts. Balance pairs DIM, glutathione and calcium D-glucarate to support healthy estrogen metabolism.* **[Meet Balance]**" + disclaimer. Body copy stays; remove "treatment" from the headings.

### 9b. High androgens in women (new)
- **URL (proposed):** `/blogs/learn/high-androgens-in-women` (a blog post, like the estrogen hub, so both hubs sit together in the Learn hub) `[NEED FROM RACHEL: OK on URL]`
- **Page goal:** Rank for androgen symptoms and feed Androgen Balance.
- **Primary keyword:** high androgens (US 1,000/mo, CA 110)
- **Secondary:** high androgen levels (US 1,300); elevated androgen levels (1,300); signs of high testosterone in a woman (2,400); excess androgen symptoms (170); supplements to lower androgens (50)
- **SEO title:** High Androgens in Women: Signs, Acne & Support | Cocoon
- **Meta description:** Oily skin, jawline breakouts, unwanted hair? Learn the signs of high androgens in women, what drives them, and how to support healthy levels.
- `[IMAGE: editorial, woman touching jawline, natural light; product module uses the Androgen Balance bottle, US packaging]`

**H1:** High androgens in women: signs, causes and support

Intro: Androgens, like testosterone and DHT, aren't only "male" hormones. Every woman makes them, and they help with energy, mood and libido. When levels run high, your skin is often the first place you notice.

**H2:** What are androgens?
Androgens are a group of hormones that includes testosterone, DHT and DHEA. Your ovaries and adrenal glands make them. In the skin, an enzyme turns testosterone into DHT, the more potent form, which tells oil glands to produce more oil.

**H2:** Signs of high androgens
- Oily skin and breakouts on the jawline, chin or body
- Unwanted hair on the face, chin, chest or stomach
- Thinning hair on the head
- Long or irregular cycles
- Blood sugar swings and strong cravings

Having one sign doesn't mean your androgens are high. A blood test with your healthcare practitioner is the only way to know.

**H2:** What drives androgens up?
- **Blood sugar and insulin.** High insulin can prompt the ovaries to make more testosterone. `[CLAIM CHECK]`
- **DHT conversion.** Some skin converts more testosterone into DHT than others.
- **Stress.** Cortisol and adrenal androgens come from the same glands, so chronic stress can push androgens higher. `[CLAIM CHECK]`
- **Liver processing.** Your liver helps clear hormones once they've done their job.

**H2:** High androgens and PCOS
High androgens are one of the main features of PCOS (polycystic ovary syndrome). If you have several of the signs above, especially irregular cycles, ask your healthcare practitioner about testing. Supplements aren't a substitute for diagnosis or care. `[CLAIM CHECK]`

**H2:** How to support healthy androgen levels
- **Balance your plate.** Protein, fibre and healthy fats with each meal help keep blood sugar steady.
- **Move most days.** Regular movement supports healthy insulin sensitivity.
- **Manage stress.** Sleep and downtime matter for cortisol.
- **Consider targeted support.** Ingredients like berberine, saw palmetto, zinc and NAC are studied for their roles in blood sugar, DHT and hormone balance. `[CLAIM CHECK]` `[NEED FROM RACHEL: ingredient studies to cite]`

**Product module:**
- **H3:** Made for androgen-linked breakouts
- Body: Androgen Balance supports healthy androgen balance from four angles: blood sugar, DHT, stress and liver.* 
- **[Meet Androgen Balance]** (before Jan 2027: **[Join the waitlist]**)
- **[Not sure? Take the quiz]**

Disclaimer.

### 9c. Your liver and your skin (new)
- **URL (proposed):** `/blogs/learn/liver-and-skin-health` `[NEED FROM RACHEL: OK on URL]`
- **Page goal:** Explain the liver–hormone–skin link and feed Liver Support as the add-on.
- **Primary keyword:** liver and skin health *(best-practice assumption: Keyword Planner shows only ~10 searches a month each for "liver detox for skin", "liver detox for hormone balance" and "detox estrogen from liver", and acne terms are suppressed. This page's job is education and internal linking, not volume. The product page takes the big liver terms.)*
- **Secondary:** liver detox for skin; liver detox for hormone balance; detox estrogen from liver; milk thistle for liver health (US 8,100)
- **SEO title:** Your Liver and Your Skin: The Hormone Link | Cocoon
- **Meta description:** Your liver clears used hormones. When it's busy, your skin can show it. Learn how the liver affects breakouts and simple ways to support it.
- `[IMAGE: editorial: green juice, cruciferous vegetables, glass water bottle; product module uses the Liver Support bottle, US packaging]`

**H1:** Your liver and your skin: how they're connected

Intro: Your liver is your body's processing centre. Along with food, drink and medication, it clears the hormones your body has finished using. When it's working hard, hormones can hang around, and your skin can show it.

**H2:** How your liver handles hormones
Your liver works in three phases:
1. **Phase 1 (activation):** enzymes start breaking hormones and other compounds down.
2. **Phase 2 (processing):** the liver attaches them to other molecules so they dissolve in water.
3. **Elimination:** they leave through bile, the gut and the kidneys.
If phase 1 runs faster than phase 2 can keep up, or elimination slows, the system backs up. `[CLAIM CHECK]`

**H2:** What keeps your liver busy
- Caffeine and alcohol
- Medication, including hormonal birth control
- Packaged foods and added sugar
- Plastics and non-natural personal care and cleaning products
- Non-organic animal products and produce
- Low-protein meals (your liver needs protein to do phase 2)
`[CLAIM CHECK: brief asks to confirm this list]`

**H2:** Why it matters for breakouts
When your liver can't clear estrogen and other hormones efficiently, they can recirculate, which keeps the hormone imbalances behind breakouts going. That's why liver support pairs well with formulas that target estrogen or androgens. `[CLAIM CHECK]`

**H2:** Simple ways to support your liver
- Eat cruciferous vegetables (broccoli, cauliflower, kale) and plenty of fibre
- Get enough protein at each meal
- Drink water through the day
- Cut back on alcohol and added sugar
- Swap plastic food containers for glass

**Product module:**
- **H3:** The booster for your formula
- Body: Liver Support pairs milk thistle, schisandra, dandelion, burdock and R-alpha lipoic acid to support every phase of your liver's natural detox process.* Take it with Balance or Androgen Balance. `[CLAIM CHECK]`
- **[Meet Liver Support]** (before Apr 2027: **[Join the waitlist]**)

Disclaimer.

---

## 10. Blog: new SEO titles and meta descriptions

Only the posts flagged in the SEO audit (section 8e). Keep every URL. Add a quiz or product CTA module to each post that matches its topic.

| # | Post (URL) | Primary keyword | New SEO title (≤60) | New meta description (≤155) | Notes |
|---|---|---|---|---|---|
| 1 | `/blogs/learn/best-teas-for-hormone-balance` (refresh) | tea for hormonal acne | 7 Best Teas for Hormonal Acne & Hormone Balance | Spearmint, green tea, dandelion and more: the best teas for hormonal acne and hormone balance, what each one does and how much to drink. | Biggest SEO asset (156,535 impressions). Add spearmint and an estrogen-tea section. CTA: quiz. |
| 2 | `/blogs/learn/can-coffee-make-hormonal-acne-worse` | does coffee cause acne | Does Coffee Cause Acne? Caffeine and Hormonal Skin | Does coffee cause acne? How caffeine affects cortisol, blood sugar and your liver, and how to enjoy coffee without the breakouts. | 48,320 impressions at 0.1% CTR. CTA: Liver Support (from Apr 2027), quiz before then. |
| 3 | Merge `/blogs/learn/balancing-hormones-with-food` into `/blogs/learn/hormonal-acne-diet-building-hormone-balancing-meals` | hormonal acne diet | Hormonal Acne Diet: Foods That Support Clearer Skin | What to eat for hormonal acne: the foods that support hormone balance and clearer-looking skin, plus easy hormone-balancing meal ideas. | Recommend keeping the slug with "hormonal-acne-diet" in it and 301-ing the other `[NEED FROM RACHEL: OK]`. |
| 4 | New post (proposed `/blogs/learn/hormonal-acne-pills-vs-supplements`) | hormonal acne pills | Hormonal Acne Pills vs Supplements: How They Differ | Spironolactone, the pill or a supplement? How prescription pills and supplements for hormonal acne differ, and questions to ask your doctor. | Product mentions stay structure/function `[CLAIM CHECK]`. |
| 5 | New post (proposed `/blogs/learn/dim-for-hormonal-acne`) | DIM for hormonal acne | DIM for Hormonal Acne: What It Does & Who It Suits | What DIM is, how it supports healthy estrogen metabolism, who it may suit, and what to know before you try a DIM supplement. | `[CLAIM CHECK]`. CTA: Balance. |
| 6 | New post (proposed `/blogs/learn/calcium-d-glucarate-benefits`) | calcium d glucarate benefits | Calcium D-Glucarate Benefits for Estrogen Balance | What calcium D-glucarate is, how it supports estrogen elimination through the gut, and why it pairs with DIM. | CTA: Balance. |
| 7 | `/blogs/learn/can-hormonal-acne-be-caused-by-stress` (refresh) | cortisol acne | Cortisol Acne: How Stress Triggers Hormonal Breakouts | Can stress cause hormonal acne? How cortisol affects your hormones and skin, the signs of stress breakouts, and what helps. | CTA: Androgen Balance (stress angle) from Jan 2027. |
| 8 | `/blogs/learn/hormone-safe-sunscreens` (refresh) | hormone safe sunscreen | Hormone-Safe Sunscreen: How to Choose One | How to choose a sunscreen that doesn't mess with your hormones: which filters to avoid, which to look for, and what the labels mean. | |
| 9 | `/blogs/learn/how-to-know-what-type-of-hormonal-acne-you-have` (refresh) | hormonal acne types | Hormonal Acne Types: Which One Do You Have? | Estrogen, androgen, stress or post-pill? Learn the main types of hormonal acne, how to spot yours, and take our free 2-minute quiz. | Replaces "How To Identify and Treat…". CTA: quiz. |
| 10 | `/blogs/learn/how-to-clear-hormonal-acne` (target of the 2025 → 2026 301) | how to clear hormonal acne | Hormonal Acne in 2026: 7 Habits for Clearer Skin | Seven realistic habits for clearer skin in 2026, from blood sugar to your liver, plus how to find the root cause of your breakouts. | Renamed to an evergreen slug without "treat", with 301s from the 2025 and 2026 URLs. |

Other live post titles that still use "treat", "treatment" or "heal" (not in 8e, but they break your rule): "The Best Natural Topical Acne Treatments" → **Natural Topical Ingredients for Acne-Prone Skin**; "Does Endometriosis Cause Adult Acne?" (blurb: "treat both at the root") → reword the blurb; "Can You Balance Hormones Through Diet?" (blurb: "heal your hormonal acne") → merged in row 3.

---

## 11. About

- **URL:** `/pages/about` (keep)
- **Page goal:** Build trust in the brand behind the range, and catch "Cocoon Skincare" brand searches.
- **Primary keyword:** Cocoon Supplements
- **Secondary:** formerly Cocoon Skincare; Cocoon Skincare (top brand query: 6,114 impressions); Cocoon acne supplement
- **SEO title:** About Cocoon Supplements (formerly Cocoon Skincare)
- **Meta description:** Cocoon Supplements, formerly Cocoon Skincare, makes naturopath-formulated supplements for hormonal acne-prone skin. Meet the founder and our story.

### Header
- `[IMAGE: Rachel portrait, natural light; or the three bottles, US packaging, if no portrait]`
- **H1:** About Cocoon Supplements
- Sub: Formerly Cocoon Skincare. Same people, same formulas, a clearer name.

### H2: We exist to help you feel confident in your skin
Hormonal breakouts aren't just a skin problem. They can wear on your confidence and your mood, especially when nothing seems to work. Cocoon exists to change that from the inside, with supplements that go deeper than the surface. Internal skincare, made simple.

### H2: How Cocoon started
Founder quote:
> "Like so many adult women, I struggled with persistent hormonal acne. Topicals and prescriptions left me with continued breakouts, side effects and a painful feeling of helplessness. It took a real toll on my mental health.
>
> Eventually, a naturopath helped me discover that my breakouts were linked to high estrogen. Within months of taking estrogen-balancing supplements, my skin changed completely. I wanted every woman going through what I went through to have that option.
>
> So I worked with a naturopath to create Cocoon's first formula, Balance."
>
> **Rachel Kirby, Founder**

`[CLAIM CHECK: founder's personal experience; add "individual results vary" under the quote]`

### H2: From one formula to a range
Body: Balance was made for one root cause: high estrogen. But as thousands of you took our quiz, a pattern showed up. Many of your answers pointed to high androgens instead, or to both, and you asked what you could take. `[NEED FROM RACHEL: OK to say "thousands"? The quiz is 26% of landing sessions; I haven't counted completions.]`

So we built a range, one formula per root cause:
- **Balance** for estrogen-linked breakouts
- **Androgen Balance** for androgen-linked breakouts (January 2027)
- **Liver Support**, the booster that pairs with either (April 2027)

Same approach as Balance: naturopath-formulated, a handful of ingredients in meaningful doses, and nothing extra.

### H2: Why "formerly Cocoon Skincare"?
We started as Cocoon Skincare, but we've always made supplements, not creams. Our new name says what we do. Your account, orders and subscriptions carry over, and our formulas haven't changed.

### H2: What we stand for
- **Integrity.** Quality ingredients, honest claims, and no promises we can't keep.
- **Simplicity.** The fewest ingredients that do the job, in doses that matter.
- **Empowerment.** Education that helps you understand your body and make your own choices, and a community centred on skin positivity.

### H2: Start with your root cause
- **[Take the quiz]** · **[Learn about hormonal acne]**

Disclaimer.

---

## 12. FAQ

- **URL:** `/pages/faq` (keep)
- **Page goal:** Answer pre-purchase and account questions in one place, for all three products. Add FAQ schema.
- **Primary keyword:** none (support page)
- **SEO title:** FAQ: Balance, Androgen Balance & Liver Support | Cocoon
- **Meta description:** Answers about our supplements: which formula fits, how to take them, safety, results, subscriptions, shipping to the US and Canada, and returns.

**H1:** Frequently asked questions
Intro: Can't find your answer? **[Contact us]** and we'll reply within 24 to 48 hours.

Jump links: Our formulas · Choosing · Taking them · Safety · Results · Subscriptions · Shipping · Returns

### H2: Our formulas

**What is Cocoon?**
Cocoon Supplements (formerly Cocoon Skincare) makes naturopath-formulated supplements for hormonal acne-prone skin. Each formula targets one root cause of hormonal breakouts.* `[CLAIM CHECK]`

**What's the difference between the three formulas?**
Balance supports healthy estrogen metabolism. Androgen Balance supports healthy androgen balance. Liver Support is a booster that supports your liver and pairs with either.* **[Compare formulas]**

**Where are they made?**
All three are made in Canada under GMP standards, with third-party testing for purity. `[CLAIM CHECK: confirm GMP and third-party testing for the new products]`

**Are they vegan and gluten-free?**
Balance is vegan and gluten-free, and free from GMOs, sugar, soy, nuts and dyes. `[CLAIM CHECK: confirm for Androgen Balance and Liver Support; their labels say they're made in a facility that handles milk, gluten, shellfish, soy, peanuts and tree nuts]`

**Why glass bottles?**
Amber glass protects the capsules from light and keeps plastics, which can contain hormone-disrupting chemicals, away from your supplements.

**How should I store them?**
In the original container, closed, away from heat, light and moisture. Androgen Balance and Liver Support are best used within 3 months of opening.

### H2: Choosing a formula

**Which formula is right for me?**
It depends on your root cause. Breakouts before your period with breast tenderness or bloating point to estrogen (Balance). Oily skin, jawline or body breakouts and unwanted hair point to androgens (Androgen Balance). The 2-minute quiz matches you. **[Take the quiz]**

**Can I take more than one?**
`[CLAIM CHECK: naturopath to confirm]` Yes. If your quiz shows both high estrogen and high androgens, take Balance and Androgen Balance. Liver Support pairs with either. Take Androgen Balance a few hours apart from other supplements. `[NEED FROM RACHEL: daily schedule for each combination]`

**Do I need a blood test first?**
No, but it can help. Your healthcare practitioner can test your hormones and give you a clearer picture.

**Do the formulas help with PCOS?**
`[CLAIM CHECK]` We can't make claims about PCOS, which is a medical condition. High androgens are common with PCOS, and Androgen Balance supports healthy androgen balance.* If you have PCOS, talk to your practitioner before starting.

**Can I take Balance after coming off the pill?**
Many women come to us after stopping the pill. Talk to your practitioner first, especially if your period hasn't come back, as that's worth checking out.

### H2: Taking them

**How do I take each formula?**
- Balance: 1 capsule a day, with or without food (food can help absorption and settle your stomach).
- Androgen Balance: 1 capsule, 3 times a day, with food, a few hours before or after other medication or supplements.
- Liver Support: 1 capsule, twice a day.

**What if I miss a dose?**
Just take your next dose as usual. Don't double up.

**Can I take a lower dose once my skin is clear?**
For Balance, many customers move to a maintenance dose of 1 capsule every other day. If breakouts come back, return to 1 a day. `[CLAIM CHECK]` `[NEED FROM RACHEL: maintenance guidance for the new products]`

### H2: Safety

**Can I take them if I'm pregnant or breastfeeding?**
No. Don't use any Cocoon formula if you're pregnant or breastfeeding.

**Can I take them under 18?**
No. Our formulas are for adults.

**Can I take them with birth control or other medication?**
Talk to your healthcare practitioner before combining any supplement with medication. Don't take Androgen Balance if you're taking antibiotics or nitroglycerin. `[NEED FROM RACHEL: naturopath's guidance on hormonal birth control and spironolactone, the most common questions in site search]`

**Are there side effects?**
- **Balance:** most people have none. Some notice mild, short-lived changes in the first weeks (darker urine, gas, headaches, tiredness or changes in stool). Taking it with food and water helps.
- **Androgen Balance:** take with food. Check with your practitioner if you have kidney stones, or for use beyond 3 months (long-term zinc can affect copper levels). `[NEED FROM RACHEL: side effects list]`
- **Liver Support:** may have a diuretic effect. Stop and talk to your practitioner if you notice sweating, paleness, chills, headache, dizziness or confusion (possible low blood sugar). Check with your practitioner first if you have diabetes, a liver or biliary disorder or an intestinal obstruction.
`[CLAIM CHECK]`

**Could my skin get worse before it gets better?**
Some Balance customers notice a short flare in the first few weeks as their body adjusts. If it continues, talk to your practitioner. `[CLAIM CHECK]`

**Can men take them?**
Balance: yes. Androgen Balance and Liver Support: `[NEED FROM RACHEL]`

**Do your formulas affect weight?**
`[NEED FROM RACHEL: naturopath's answer; "weight gain" is a recurring site search]` `[CLAIM CHECK]`

### H2: Results

**How long until I see results?**
[TIMELINE] Hormones shift gradually, so take your formula every day. Everyone is different.

**How long should I take it for?**
[TIMELINE] For Androgen Balance, check in with your practitioner for use beyond 3 months.

### H2: Subscriptions

**How does Subscribe & Save work?**
Choose delivery every 1 or 3 months and save 10% on every order. Subscriptions ship free.

**Can I skip, change or cancel?**
Yes, anytime. Log in and go to **Manage subscription** (in the Account menu). Changes need to be made before your next billing date. `[NEED FROM RACHEL: confirm cut-off]`

**Can I add Liver Support to my Balance subscription?**
`[NEED FROM RACHEL: confirm Appstle lets customers add products to an existing subscription]`

### H2: Shipping

**Do you ship to Canada and the US?**
Yes. `[NEED FROM RACHEL: where Balance ships from for each country]` Androgen Balance and Liver Support ship from our US warehouse, including to Canada.

**Is there a limit on Canadian orders?**
For Androgen Balance and Liver Support, Canadian orders can include up to a 3-month supply of each per order. `[CLAIM CHECK: regulatory advisor to confirm how to word the 90-day personal-use limit without mentioning licensing]`

**Will I pay duties or taxes in Canada?**
`[NEED FROM RACHEL]`

**How much is shipping and how long does it take?**
Free on subscriptions and orders $70+. `[NEED FROM RACHEL: flat rate under $70; the old meta description said $12]` Orders are processed within 24 to 48 hours (weekdays), and delivery usually takes 4 to 10 business days. `[NEED FROM RACHEL: confirm times for US-to-Canada shipping]`

**Can I order Balance and a new formula together?**
`[NEED FROM RACHEL: one shipment or two?]`

**What currency are prices in?**
`[NEED FROM RACHEL: USD for everyone, or CAD for Canadian shoppers via Shopify Markets?]`

### H2: Returns and the guarantee

**What's the money-back guarantee?**
Try any formula for 30 days. If it isn't the right fit, contact us within 30 days of your carrier-confirmed delivery date and we'll refund you. No need to send it back. **[Full terms]**

**Can I return an unopened product?**
Yes. We'll send a return label, and refund you minus the label cost once it arrives.

**My order arrived damaged or wrong.**
Contact us within 14 days of delivery with a photo and your order number, and we'll make it right.

Contact block: **H2:** Still have a question? · Contact form (Name, Email, Message) · **[Send]**

Disclaimer.

---

## 13. Money-back guarantee

- **URL:** `/pages/money-back-guarantee` (keep). Footer label: "Money-back guarantee" (was "Returns").
- **Page goal:** Remove purchase risk, with clear terms, for all products.
- **Primary keyword:** none (support page)
- **SEO title:** 30-Day Money-Back Guarantee | Cocoon Supplements
- **Meta description:** Try any Cocoon formula risk-free. If it's not the right fit, request a refund within 30 days of delivery. No need to send it back.

**H1:** Our 30-day money-back guarantee
Body: We want you to feel confident trying a new formula. If Balance, Androgen Balance or Liver Support isn't the right fit for your body, request a refund within 30 days of your carrier-confirmed delivery date. No need to send it back. We'll just ask for some quick feedback.
- **[Request a refund]** → contact form (with your order number)

**H2:** What's covered
- One bottle or refill per customer `[NEED FROM RACHEL: per customer, or per customer per product, now that there are three?]`
- Orders placed directly on cocoonsupplements.com
- Original shipping costs aren't refunded
- Not covered if the product was used against the directions, for example above the recommended dose

**H2:** Unopened products
If anything in your order is unopened and in sellable condition, you can return it. We'll send a return label, and refund you minus the label cost when it arrives. `[NEED FROM RACHEL: return address for products shipped from the US warehouse]`

**H2:** Damaged or wrong items
Contact us within 14 days of delivery with a photo and your order number, and we'll make it right. `[NEED FROM RACHEL: publish a support email, now that the guarantee mentions emailing us]`

**H2:** A note on results
Hormones shift gradually, and every body is different. [TIMELINE] The guarantee isn't a promise of results by a certain date. It's there so you can try something new with confidence.

**H2:** The legal bit
- **Health and safety:** Cocoon isn't responsible for adverse effects from misuse or pre-existing conditions. Please talk to your healthcare practitioner before starting, especially if you have a medical condition or take medication.
- **Limitation of liability:** By requesting a refund, you agree that Cocoon isn't responsible for health concerns or damages beyond what this policy covers.
- **Your rights:** This guarantee is in addition to your statutory consumer rights.
- **Governing law:** Ontario, Canada, unless the law where you live says otherwise. `[NEED FROM RACHEL: confirm, now that the store is US-facing]`

---

## Appendix A: How competitors word their claims

Scanned 21 Oct 2026 from each brand's own product page. **These are observed phrases, not legally safe ones.** Several are stronger than I'd recommend for Cocoon. I'm not a lawyer; use this to brief your reviewer.

| Brand · product | Phrase (verbatim) | Pattern |
|---|---|---|
| **Milamend** · [Hormone Balance](https://milamend.com/products/hormone-balance) | "Helps with promoting clearer skin, healthy hair and nails, as well as excessive hair growth management for overall physical well-being.\*" | "Clearer skin" with an asterisk |
| | "supports the signaling pathways that regulate androgen levels" (D-chiro-inositol) · "Promotes… healthy androgen levels" (alpha lipoic acid) | "Healthy androgen levels" |
| | Timeline: "2 WEEKS… 4 WEEKS… 6 WEEKS… 10 WEEKS… Clearer skin\*" · "We recommend 3–6 months of consistent use to see results." | One clear timeline |
| | Before/after chips: "Breakouts → Clearer Skin" | Skin outcome as a visual |
| **Nourished Natural Health** · [AndroEase Plus](https://nourishednaturalhealth.com/products/androease) | "Clearer Skin. Less Unwanted Hair. Hormonal Confidence." | Outcome headline |
| | "Helps with hormonal acne - supports clearer skin by helping your body handle hormone swings better" | "Acne" + "supports clearer skin" |
| | "designed to support healthy hormone balance and androgen wellness in women" | "Androgen wellness" |
| | "Hormonal skin concerns, particularly around the jaw, chin, or cheeks" (in "Designed for you if…") | Signs, not claims |
| | "Citations refer to published research on individual ingredients, not this specific product." | Ingredient-research footnote |
| **Arrae** · [Inositol](https://arrae.com/products/inositol) | "Healthier looking skin & hair\*" | Cosmetic "-looking" hedge |
| | "Inositol has been shown to support clearer skin & hair health over time.\*†" with "†Based on individual ingredient research." | Ingredient-level evidence, footnoted |
| | "Monthly breakouts or skin changes" (listed as a sign your hormones need support) | Signs, not claims |
| **Bird&Be** · [Inositol Cycle Support](https://birdandbe.com/collections/cycle-support/products/pcos-support) | No skin or acne claims on the page. | Avoids skin entirely |
| | "helps to reduce androgens, like testosterone." · "Supports hormone balance." | Stronger androgen verb |
| | "These statements have not been evaluated by the Food and Drug Administration and Health Canada." | Dual US + Canada disclaimer |
| **Clearstem** · [MINDBODYSKIN®](https://clearstemskincare.com/products/mindbodyskin-csb) | Product name: "MINDBODYSKIN® Hormonal Acne Supplement" | "Acne" in the product name |
| | "#1 bestselling daily capsule to proactively address and fight hormonal acne at its root.\*" | Aggressive ("fight") |
| | "→ Supports clearer-looking skin over time\*" · "→ Promote liver and lymph detoxification\*" | "-looking" hedge; liver detox |
| | "Many report results in as little as 7-10 days… Stay consistent for a minimum 3 months" | Fast + minimum timeline |

**What this tells us (my read, not legal advice)**
1. **"Supports clearer(-looking) skin\*" is the industry's default skin claim.** Adding "-looking" (Arrae, Clearstem) makes it a cosmetic appearance claim. I've used "clearer-looking skin" on our product pages.
2. **"Acne" mostly appears in names, headlines, "is this for you?" lists and reviews, not as a verb claim.** Our use ("support for androgen-linked breakouts", "for hormonal acne-prone skin") is in line with that, and tagged `[CLAIM CHECK]`.
3. **Androgens: "supports healthy androgen balance/levels" is common** (AndroEase, Milamend). Bird&Be's "helps to reduce androgens" is a step further. I used the softer version, plus the brief's "helps reduce the conversion of testosterone into DHT" for saw palmetto, flagged.
4. **Brands without product studies footnote ingredient research** (Arrae, AndroEase). Worth copying once you send ingredient studies.
5. **Everyone shows one timeline.** That's the case for settling [TIMELINE].
6. **Bird&Be (a Canadian brand) names Health Canada in its disclaimer.** You've ruled out mentioning Health Canada, so I haven't. Ask your reviewer whether Canadian buyers need anything beyond the FDA disclaimer.

---

## Appendix B: Product names

**Recommendation: keep "Androgen Balance" and "Liver Support".** Use "booster" in the Liver Support positioning, not the name.

**Data:** Google Keyword Planner via the Windsor `google_ads` connector, average monthly searches over the past 12 months, English, pulled 21 Oct 2026. Rounded by Google. Acne terms are suppressed for this account, so these are name-level signals only.

| Term | US | Canada | What the searches are about |
|---|---:|---:|---|
| androgen balance | 20 | 10 | Generic, ours to own |
| metabolic balance | 320 | 260 | Mostly **Metabolic Balance®, an existing diet program** (related ideas: "metabolic balance program" 110 US / 140 CA, "metabolic balance diet" 50 / 70, "wolf funfack metabolic balance") |
| metabolic support supplement | 880 | 40 | Weight and metabolism |
| high androgens / high androgen levels | 1,000 / 1,300 | 110 / 110 | The concern our hub targets |
| liver support | 6,600 | 390 | Exactly our category |
| liver support supplement | 18,100 | 1,900 | Exactly our category |
| liver booster | 590 | 70 | Small, mixed intent |

**Why Androgen Balance**
- **It says what it does.** It matches the quiz result she just got ("high androgens") and the concern people search for (1,000 to 1,300 a month in the US). "Metabolic" doesn't tell her it's for her skin.
- **"Metabolic Balance" is already a brand.** Its search demand belongs to an established diet program, so we'd compete for our own name, and there's a trademark risk. `[CLAIM CHECK: trademark search before final naming]`
- **"Metabolic" points to weight loss.** With berberine in the formula, that invites weight-loss expectations and the extra FTC scrutiny that comes with them.
- **The case for "Metabolic":** it's softer and less clinical, and it covers the blood sugar angle. If you prefer it, I'd use a different second word to avoid the existing brand.

**Why Liver Support**
- **About 30 times the searches:** "liver support supplement" gets 18,100 a month in the US and 1,900 in Canada, against 590 and 70 for "liver booster". With the keyword in the product name, the product page's title, H1 and URL all work for search.
- **"Booster" still fits the positioning.** The copy calls it "the booster for your formula", so you keep the idea without the weaker name.
- **The trade-off:** "Liver Support" is generic, so brand searches for it will compete with other liver products. Titles use "Cocoon Liver Support" where space allows.

---

## Open items

**Needs a decision from you**
1. **One results timeline** for every product. It's needed in 7 places in the page copy, marked [TIMELINE]. The site currently says "1 week to 3 months", "3 to 6 months" and "60 to 90 days". For Liver Support it must agree with the label ("Use for at least 3 weeks to see beneficial effects").
2. **Final names:** Androgen Balance vs Metabolic Balance; Liver Support vs Liver Booster (Appendix B recommends Androgen Balance and Liver Support). Run a trademark search either way.
3. **Bundles / stack pricing**, or confirm there are none at launch.
4. **Guarantee scope:** one bottle per customer, or one per customer per product? Does it cover the new products? Where do returns of US-shipped products go?
5. **Launch offers** for waitlist members and quiz sign-ups, if any.
6. **Diet post merge:** keep `hormonal-acne-diet-building-hormone-balancing-meals`, 301 `balancing-hormones-with-food` to it (adds one row to the redirect map).
7. **Concern hub URLs:** `/blogs/learn/high-androgens-in-women` and `/blogs/learn/liver-and-skin-health`.
8. **Quiz changes:** new liver-load question, extra androgen options, outcome D with or without Liver Support, Typeform end-screen buttons. Nothing has been edited.
9. **Pre-launch product pages:** OK to publish waitlist versions 4 to 6 weeks before each launch? Klaviyo waitlist lists need setting up.

**Facts I need**
10. **Label contact email:** both US label files still say "Questions? Email info@cocoonskincare.ca", and "Manufactured for: Cocoon Skincare Inc." Update before print.
11. **3-month format** for the new products: 3 bottles, or 1 bottle + 2 refills like Balance? Are there refill pouches?
12. **Shipping:** does free shipping over $70 apply to Canada? Where does Balance ship from? US-to-Canada transit times, duties and taxes, the flat rate under $70, and whether mixed orders ship together.
13. **Currency:** USD for everyone, or CAD for Canadian shoppers?
14. **Legal entity name** for the footer, Terms and Privacy (they currently say "Cocoon Skincare Inc." and "Cocoon Inc."). Governing law for the guarantee.
15. **Support email** to publish (the guarantee says "email us", but the site shows no address).
16. **Packaging designs and photography** from Yuliia for Androgen Balance and Liver Support (US packaging).
17. **Ingredient studies** to footnote (both briefs say "will dig and get these").
18. **Typical-results data** (for example, a short customer survey) so testimonials can carry a typical-results statement.
19. **"Thousands" of quiz takers** on the About page: OK to say?

**For your naturopath** `[CLAIM CHECK]`
20. **Combinations:** Balance + Androgen Balance, and either + Liver Support. Plus a daily schedule: Androgen Balance is taken 3 times a day with food and "a few hours before or after… other medication or dietary supplements", which leaves little room for Balance.
21. **Blood sugar:** Androgen Balance (berberine) with Liver Support, whose label warns about low blood sugar.
22. **Androgen Balance beyond 3 months:** the label says to consult a practitioner. This needs to fit the timeline and the subscription messaging.
23. **Men:** can they take Androgen Balance (its label has a prostate warning) and Liver Support?
24. **Birth control, IUDs and spironolactone** with each formula. These are the most common safety searches on the site.
25. **Side effects** for the new products, and maintenance dosing.
26. **The liver-load list** (caffeine, alcohol, medication, plastics and so on): confirm each is processed by the liver.

**For your regulatory reviewer** `[CLAIM CHECK]` *(I'm not a lawyer)*
27. Every product + acne pairing: the home H1 "Internal skincare for hormonal acne", the product H1s, "for hormonal acne-prone skin" in titles, and "acne supplements" as a keyword.
28. "Anti-androgen supplement" in the Androgen Balance title (it names a drug class).
29. Mechanism claims for the new products (DHT conversion, insulin sensitivity, cortisol, phase 1/phase 2 detox, burdock for congested skin).
30. "Detox" wording on Liver Support.
31. Free-from, GMP and third-party-testing claims for the new products, given the label's facility allergen statement.
32. Canada: how to describe the 3-month-per-order limit for the new products, and whether Canadian pages need anything beyond the FDA disclaimer. The site never mentions an NPN or Health Canada licensing.
33. Testimonials: confirm the selection and the "individual results vary" disclosure meet FTC typical-results rules.

**Removed from the current site** (for your awareness)
- Unsourced stats: "72% of adult women", "almost 80% of the population", "20-30% of adults".
- Disease states in symptom lists (ovarian cysts, fibroids, anxiety, depression, migraines, insomnia, erectile dysfunction).
- "Health Canada licensed facility", "scientifically proven", "the only supplement that contains…", "acne-healing", "once and for all", and DIM's "anti-androgenic properties".
