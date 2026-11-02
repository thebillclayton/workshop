# Move-Up Homebuyer Workshop: Attendee Worksheet

**Owner:** Bill Clayton, Rate, NMLS #151125 · 706-660-5245 · bill.clayton@rate.com
**Live site:** https://workshop.callbillclayton.com (GitHub Pages, repo `thebillclayton/workshop`, branch `main`, root folder)
**Last updated:** 11/2/2026 by Claude

This README is the handoff for any AI (Claude, ChatGPT, Gemini, Perplexity) picking up this project. Read it fully before changing anything.

## What this is

A one-page, phone-friendly worksheet for Bill's Move-Up Homebuyer Workshop (Zoom Webinar). Core message: compare the **whole monthly budget** (house payment + all other debt payments), not just old rate vs new rate. Home equity can pay off consumer debt and keep the total budget close to today's.

**How it's used (decided 11/2/2026, after the 10/30 dry run with Rick Mount):**
1. Bill presents the deck and **demos this worksheet himself** by screen share.
2. Attendees do NOT use it during the talk (it distracts them and adds tech risk).
3. At the end, Bill drops the link or QR code (`workshop-qr.png`) in chat as the reward.
4. The call to action is the big **Book 10 Minutes with Bill** button (Calendly Intro Call: https://calendly.com/billclayton-rate/intro-call). Calendly captures name and phone, so the page itself does not collect leads.

## Files

| File | What it is |
|---|---|
| `index.html` | The attendee worksheet. Everything (HTML, Tailwind CDN, JS) in one file. |
| `workshop-qr.png` | QR code to the live site, for the closing slide. |
| `move_up_presenter.html` | Old presenter console from the "share with room" idea. No longer used. Leave it alone unless Bill asks. |
| `CNAME` | Custom domain `workshop.callbillclayton.com`. **Never delete or edit.** Deleting it breaks the domain and the SSL certificate. |

## How the page works

- **Step 1, Your Home Today:** home value, mortgage payoff, today's house payment (with taxes and insurance), listing fees %, negotiations %. Shows gross equity, cost to sell, net equity.
- **Step 2, Your Other Debts:** editable rows. Checked rows get paid off in Paths 2 and 3.
- **Step 3, Your Next Home:** price, rate, taxes + insurance per month. 30-year fixed.
- **Today's Budget bar:** today's house payment + all debt payments.
- **Three paths, always three** (Bill's rule). Side by side on desktop, swipe cards on phones. Each shows: New house payment (P&I + taxes/ins) + other debt payments = whole monthly budget, then "$X more/less than today."
  - **Path 1, Down Payment Only:** net equity goes down, all debts stay.
  - **Path 2, Pay Off + Cushion (Recommended, highlighted):** checked debts paid, zero down (like VA), leftover kept as cushion.
  - **Path 3, Pay Off + Down:** checked debts paid, leftover goes down.
- **One limited slider per path, 0 to 25% only** (Bill wants attendees to adjust "to a limited extent" while the three options stay distinct):
  - Path 1: keep in savings (% of net equity).
  - Path 2: put down (% of what's left after payoffs).
  - Path 3: keep as cushion (% of what's left after payoffs).
- **Badges are automatic:** "Most cushion" goes to the path with the largest cushion; "Closest to today's budget" goes to the path whose total is nearest today's. At defaults: Path 2 and Path 3.

## Master example (defaults, must match the deck)

From `Prelim Est (Video 10-16-26).xlsx` in Drive > Move Up Homebuyer Workshop.

- Home value $415,832 · payoff $234,980 (at 2.25%) · today's house payment $1,376
- Selling costs 6% + 0.71% → net equity **$152,950** (deck says $152,959; Bill accepted the $9 difference for clean percentages)
- Debts $113,005, $2,094/mo: 2 car loans ($24,602 / $493), 2 credit cards ($6,735 / $191), 2 student loans ($19,528.50 / $215), 2 personal loans ($5,637 / $148)
- Next home $515,000, VA 30-yr fixed 6.75%, taxes + insurance $675/mo
- **Expected results:** Today $3,470 · Path 1 $5,117 (+$1,647) · Path 2 $4,015 (+$545, ~$39,945 cushion) · Path 3 $3,756 (+$286)

If you change the math, re-check these numbers before publishing.

## Bill's rules for this page

- Goals first, plan second, mortgage last. Encouraging tone ("life changes, it's okay if your home needs to too"). No fear language, no airplane or flight metaphors.
- KISS (Keep It Super Simple): 5th-grade-simple screens.
- Phone numbers are tap-to-call (`tel:`) with a Copy button. Emails are `mailto:` links.
- No em dashes in any text. No compliance disclaimers unless Bill asks.
- Never change the three-path structure.

## How to publish an update

Claude cannot push to GitHub directly (no GitHub connector on Bill's account). Working method:
1. Edit `index.html` (one file).
2. In Bill's Chrome, signed in as `thebillclayton`: go to https://github.com/thebillclayton/workshop/upload/main, upload the file(s), choose "Commit directly to the main branch," commit.
3. Wait 1 to 2 minutes, open https://workshop.callbillclayton.com, hard refresh, and check the Today and three path totals.

Never change the custom domain or Enforce HTTPS settings in repo Settings > Pages.

## Open items (as of 11/2/2026)

1. **Zoom Webinar setup:** Bill is finishing it with Zoom AI (registration, attendees hidden, recording). Use Zoom's built-in polls for audience questions; the old "share with room" feature was removed.
2. **Invites:** invite list and sends for the Tue 11/10 6:00 PM pilot (past clients). Drafts are in Drive > Move Up Homebuyer Workshop ("Pilot Invitations - Bill's Past Clients v1").
3. **Soft open:** treat 11/10 as the friendly test of tech and call to action, per Rick Mount.
4. **Deck:** add the QR code slide at the close; add real stories from Bill's PrePurchase Consults; recheck the 6.75% rate the week of.
5. **Megan Kennedy:** text inviting her to watch the pilot.
6. **Later:** recordings to YouTube and Opus Clip social posts; realtor-hosted versions; Rick Mount's discovery-call Claude skill (emailed to Bill) to review after the pilots.
