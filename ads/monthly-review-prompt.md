# Monthly Google Ads review: scheduled task instructions

Copy of the instructions the "Monthly Google Ads review" scheduled task runs (1st of each month, 9:07am Toronto, email only). Needs the Windsor.ai and Shopify connectors attached.

---

Run Cocoon's monthly Google Ads review for the month that just ended. This is ANALYSIS ONLY: do not make any changes to Google Ads (never call execute_action). Rachel approves changes afterwards by replying in this session.

Setup:
1. Get the cocoon repo (GitHub: rachelkirby55-rgb/cocoon). If it isn't already in your working directory, call the add_repo tool (claude-code-remote MCP server; load it with ToolSearch if needed) with owner "rachelkirby55-rgb", repo "cocoon" and access "push", then clone it using the command add_repo returns.
2. In the repo, run `git fetch origin claude/amazing-gates-1hqv0p` and check out that branch if it exists on origin; otherwise stay on the default branch. Do all your commits there and push to the same branch.
3. Read `.claude/agents/ads.md` and follow it as your role and rules. Then read `ads/google-ads-manual.md` in full, and the last 2–3 reviews in `ads/reviews/` if any exist.

Review (follow the manual's "Monthly review" steps exactly):
- Use the Windsor.ai connector `google_ads` (account 742-164-2243) with get_data. Pull last month, the month before, and a 3-month view. Ignore conversion data from before mid-Sept 2026 (double-counted).
- Results per campaign: cost per purchase, purchases, spend, conversion rate vs last month and vs target. Canada vs CA$84 target CPA. US vs the kill rule (~CA$500 spent with fewer than 2 sales) and graduation rule (~15 sales).
- Cross-check Google's purchase counts against real Shopify orders for the same period.
- Search terms: list irrelevant searches to add as negatives (never glutathione or DIM) and repeat converters to add as phrase keywords.
- Keywords, bidding and budget: only propose changes the manual's rules support. Max one or two big changes. Nothing from the "Rejected on purpose" list.
- Every 2–3 months: check for headlines rated "Low".
- Note progress on the manual's open items.

If the Windsor.ai or Shopify tools are not available in this session, or you still can't get the repo after trying add_repo, stop and say so plainly instead of guessing numbers.

Output:
1. Write the review to `ads/reviews/YYYY-MM-google.md` (YYYY-MM = the month reviewed). Start with a 3–5 line plain-language summary: is each campaign making or losing money, and the top things you want to change. Then a numbered list of proposed changes, each with: what exactly, why (with the numbers), and expected effect. Then the supporting tables.
2. Commit and push it.
3. End your reply with the same short summary and the numbered proposals, written very simply, and ask Rachel which numbers she approves. When she replies, make only the approved changes, then add them to the change log in `ads/google-ads-manual.md` with the date and reason, commit and push.
