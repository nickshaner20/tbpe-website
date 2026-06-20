# Tampa Bay Property Experts — Website, SEO & Tech Strategy

*Prepared June 2026. This is the blueprint behind the new website. It covers the keyword plan, the local/geo SEO strategy for your neighborhoods, blog cadence, the recommended software stack, and how to handle the secure SS# and ACH-rent problems the right way.*

---

## 0. Decisions locked & recommended stack (June 2026)

**Build:** new custom-coded site (delivered — see file list below). **Hosting:** use **Netlify** or **Cloudflare Pages** — both are free, and you deploy by literally dragging the website folder onto their dashboard. You can update content anytime and it's trivial to hand off later. Point your existing domain at it when ready.

**Service area:** corrected to the *entire* greater Tampa Bay area — **Hillsborough, Pinellas, and Pasco** counties (St. Petersburg, Clearwater, etc. now included).

**Management fee:** messaged as **"from 7.5%"** across the site, with the 7.5%–10% range explained on the Owners page (scaled to property complexity).

**Leases:** positioned around your standard **12-month** lease.

### The big recommendation: replace Rentec Direct with an all-in-one platform

Your current workflow is the real problem — applicant fills your form, pays via Zelle/PayPal, you email yourself the app, manually re-key it into Rentec's screening portal, *phone the renter for their SSN*, key that in, pay Rentec's fee yourself, then wait for reports. That's slow, error-prone, and it's why you're stuck handling SSNs by phone.

A modern platform collapses all of that into one automated flow: **apply → pay app fee → applicant enters their own SSN directly with the bureau → screening reports (credit, criminal, eviction) come back to you automatically.** The same platform also runs ACH rent with tenant-paid fees, maintenance, owner portals, and accounting — so it replaces Rentec entirely and powers the Apply / Pay-Rent pages on the new site.

| Platform | Why / fit | Notes |
|---|---|---|
| **DoorLoop** *(top pick)* | Highest ease-of-use rating in 2026; all-in-one (applications, built-in TransUnion screening, ACH rent, maintenance, accounting, QuickBooks sync). Applicant-paid screening (≈$49.90) with **no merchant account required** on the Comprehensive plan. | Best balance of modern UX + full feature set for a company your size replacing Rentec. |
| **AppFolio** | Most powerful; great if you're scaling a larger portfolio fast. | Higher cost, minimum monthly spend; more than you likely need today. |
| **Buildium** | Solid, owner-friendly mid-market option. | Good, but less modern than DoorLoop. |
| **Rentvine** | Modern, open API, loved by pro SFR operators. | Great if deep customization matters later. |

**My recommendation: DoorLoop.** It directly solves the SSN problem (applicant enters it with the bureau — you never touch it), eliminates the manual re-keying, handles the app fee, and runs your ACH rent with tenant-paid fees. The new site's **Apply** and **Pay Rent** pages are built as the polished front door that hands off to it.

> This supersedes the earlier "build fully custom forms + custom ACH/SSN vault" plan — DoorLoop does all of it natively, compliantly, and far cheaper than building and maintaining your own.

---

## 1. Where you are today

Your current site is a 3-page Wix site from 2015 (Home / Tenants / Contact). It has almost no indexable text, no service pages, no neighborhood pages, no blog, and no schema markup. For Google, there is very little to rank. That's actually good news: nearly everything we add is upside.

The new site is built around three goals:

1. **Rank locally** for "property management" + your neighborhoods.
2. **Convert** owners (free rental analysis) and tenants (apply / pay / maintenance).
3. **Handle the two hard problems** — secure SS# collection and ACH rent — properly and compliantly.

---

## 2. Keyword strategy

The single most important SEO principle for you: **separate owner keywords from tenant keywords, and give each its own page.** People searching to *hire* a manager and people searching to *rent* are different audiences with different intent.

### Primary keywords (owner intent — highest commercial value)

| Keyword | Why it matters |
|---|---|
| tampa property management | Core money term |
| property management tampa fl | Core money term, geo-qualified |
| property management company near me | Highest-intent "ready to hire" search |
| rental property management tampa | Service-specific |
| property managers for landlords tampa | Owner-specific |
| residential property management tampa bay | Matches your service area |

### Neighborhood keywords (your competitive edge)

These are lower-volume but far easier to rank for and convert better. One page each:

`carrollwood property management` · `northdale property management` · `south tampa property management` · `downtown tampa property management` · `seminole heights property management` · `tampa heights property management` · `lutz property management` · `wesley chapel property management` · `new tampa property management` · `temple terrace property management` · `land o lakes property management`

### Tenant keywords (drive applications & rentals)

`homes for rent tampa`, `rentals in [neighborhood]`, `pet friendly rentals tampa`, `houses for rent wesley chapel`, plus support terms like `pay rent online`, `tenant maintenance request`.

### Long-tail / blog keywords (low competition, build authority)

`how much does a property manager cost in florida`, `florida landlord tenant law security deposit`, `should I hire a property manager tampa`, `average rent in carrollwood`, `tampa rental market trends 2026`.

> **Rule of thumb:** map every keyword to **one** page *before* writing the copy. Never target the same term with two pages — they'll compete with each other.

---

## 3. Site architecture (recommended sitemap)

```
/                         Home (built — draft delivered)
/property-management      Owner services hub  → "property management tampa"
/owners                   Why us, pricing, free rental analysis
/tenants                  Tenant hub (apply / pay / maintenance / FAQ)
/apply                    New secure rental application
/pay-rent                 ACH rent portal
/maintenance              Maintenance request form
/secure-upload            Secure SS#/document submission
/areas/                   Areas-we-serve index
   /areas/carrollwood
   /areas/northdale
   /areas/south-tampa
   ... (one per neighborhood)
/blog/                    Blog index
   /blog/[post-slug]
/about                    Company, broker, license
/contact                  NAP + form + map
```

Each owner/neighborhood page should have a single clear call-to-action: **Get a Free Rental Analysis**.

---

## 4. Local & geo SEO plan (the part that wins Tampa Bay)

Most of your competitors are national directories (Zillow, etc.) and big chains. You beat them on hyper-local relevance. Three pillars:

### A. Google Business Profile (free, do this first)

Your GBP is arguably your most important asset — it's what shows up in the map pack. Action list:

- Claim/verify the profile, category **"Property Management Company."**
- Exact, consistent **NAP** (Name, Address, Phone) matching the website footer.
- Add real photos, services, service-area cities (all your neighborhoods).
- Post updates regularly (even short ones) — active profiles rank better.
- **Reviews are a top-3 local ranking factor.** Build a simple habit: ask every happy owner/tenant for a Google review and respond to each one. Aim for a steady trickle, not a burst.

### B. Neighborhood landing pages (your highest-ROI SEO work)

This is the most powerful lever you have. **One genuinely unique page per neighborhood** — not a template with the name swapped. Each page should be **800–1,500 words** of real local content:

- Local rental market snapshot (typical rents, vacancy, property types).
- "Owner insights" for that area (what rents well, seasonal demand).
- Landmarks, school districts, commute notes — these tell Google exactly where you operate.
- Your services framed for that neighborhood + a free-rental-analysis CTA.
- Internal links to nearby neighborhood pages and the main services page.

The homepage already links to all 11 neighborhood pages — we just need to build them out. *(I can draft these for you; each needs a few real local facts to be credible — see "What I need from you.")*

### C. Citations & consistency

List the business in the same NAP format across Google, Bing Places, Yelp, Apartments.com, and the BBB. Inconsistent addresses/phones hurt local ranking — pick one canonical format and use it everywhere. **Note:** your current Wix footer has a typo in the mailing ZIP ("336624"). Fix that everywhere.

---

## 5. Blog strategy & cadence

**How often should you publish?** The data-backed sweet spot for a service business is **one high-quality post per week (≈4/month)**. If that's too much, the *minimum* that still keeps Google crawling you as "active" is **2 posts/month**. More important than frequency: **quality, depth, and local usefulness.** Ten genuinely helpful local articles beat fifty thin ones.

**My recommendation for you:** start at **2 posts/month**, ramp to weekly once the engine is running. Alternate between *owner* topics (lead-gen) and *tenant/local* topics (traffic + authority).

### Starter topic calendar (first 12 posts)

1. How much does property management cost in Tampa? (owner, money keyword)
2. Carrollwood rental market report 2026 (local authority)
3. Florida security deposit law: what landlords must know
4. 7 signs it's time to hire a property manager
5. Best neighborhoods to own a rental in Tampa Bay
6. Tenant screening: how we find reliable renters
7. Wesley Chapel vs. New Tampa: where should you invest?
8. How to handle a maintenance emergency as a tenant
9. Average rent in South Tampa & what drives it
10. Landlord tax deductions in Florida
11. What to look for in a Tampa lease agreement
12. New Tampa rental market report 2026

### Auto-publishing the blog

Since you're on a custom code site, the clean way to "auto-publish" is a **headless CMS** (e.g., Sanity, Contentful, or Notion-as-CMS) feeding the site, with builds triggered automatically. Practical setup:

- You (or I, on a schedule) draft posts into the CMS.
- A scheduled job publishes them on cadence and the site rebuilds — no manual deploy.
- **I can run a recurring scheduled task** that drafts a new SEO-optimized post on your chosen cadence and queues it for your one-click approval. That gives you "set it and forget it" blogging with a human check before anything goes live (recommended — you don't want fully unattended publishing on a professional site).

---

## 6. The secure SS# form (do this carefully)

**Why Wix blocked it:** generic form builders refuse SSNs because storing them creates serious liability under the FCRA and data-privacy law. The fix is *not* a normal web form that emails you the number — that's the worst option.

**Best-practice options, in order of recommendation:**

### Option A (recommended): Tenant-initiated screening — you never touch the SSN
Use a screening service like **TransUnion SmartMove** (or similar). Flow: the applicant gets an email invite, enters their SSN **directly with the screening company**, and you receive the finished credit/background/eviction report — **without ever seeing or storing the SSN.** This eliminates almost all of your liability and is usually the cheapest path. The applicant typically pays the screening fee.

### Option B: Tokenized secure form (if you must collect it yourself)
If you need the raw SSN in your own workflow, never let it hit your own server in plain text. Use a **tokenization vault** — e.g., **Basis Theory, Very Good Security (VGS), or Skyflow**. The SSN goes straight from the applicant's browser into the vault, which returns a token; your system only ever stores the token. Requirements: TLS in transit, encryption at rest, strict access controls, an audit log, and a written data-retention/deletion policy.

**What this means for the build:** the secure form needs a small backend — it cannot be a static page. The page at `/secure-upload` in the new site is the front door; behind it we wire either SmartMove (Option A) or a tokenized vault (Option B).

> My strong recommendation: **Option A as primary** (solves your problem, minimal liability), with a tokenized upload as a fallback for documents.

---

## 7. The ACH-only rent portal

Your requirements: **ACH only (no credit/debit cards), renter pays the processing fee, keep it as cheap as possible.** Your instinct is right on two counts:

- **No cards = no chargebacks-after-move-out.** Card "chargebacks" don't exist on ACH. ACH does allow limited *returns/disputes* (a consumer can claim an unauthorized debit, generally within 60 days), but it's far less abused than card chargebacks, and a signed ACH authorization agreement protects you.
- **ACH fees are much lower than cards** (cards run 2.9%+; ACH is pennies-to-a-few-dollars).

### Cheapest options for the tenant

| Processor | Tenant cost on ~$1,500 rent | Notes |
|---|---|---|
| **Dwolla** (ACH-native) | ~$0.50 flat / txn | Cheapest per-transaction; built for ACH; needs dev integration |
| **Stripe ACH Direct Debit** | 0.8%, **capped at $5** (so ~$5 here) | Easiest to build; +bank-verification cost; great docs |
| RentRedi (PM app) | $1.00 flat | Cheapest *turnkey*, but it's full PM software (you opted out) |

**Recommendation:** for "cheapest for the renter" on a custom build, **Dwolla's flat ~$0.50/transaction** is hard to beat and passed straight to the tenant. **Stripe ACH** is the easier integration if you'd rather move fast — its $5 cap still beats any card option.

### Build notes & compliance
- Verify the tenant's bank account (Plaid instant verification or micro-deposits).
- Collect a **written ACH authorization** at signup (protects against "unauthorized" return claims).
- **Disclose the exact fee before they pay** — required, and just good practice.
- Florida allows passing a convenience fee to the payer; keep the fee tied to actual processing cost and disclose it clearly.
- Like the SS# form, this needs a **backend + a payments account** (Dwolla or Stripe). The `/pay-rent` page is the front end.

---

## 8. Fixing the application form

You mentioned the current application is weak and has a question out of order. The new `/apply` page should:

- Put fields in logical order: applicant info → current address & residence history → employment & income → references → vehicles/pets/occupants → consent & e-signature.
- **Move SS#/screening out of this form entirely** — route it to the secure SmartMove flow (Section 6). The application collects everything *except* the SSN; the SSN is handled in the secure step.
- Be mobile-friendly, save progress, and confirm submission by email.

*Send me your current application (or a screenshot) and I'll redo it field-by-field, including fixing the out-of-order question.*

---

## 9. What's resolved & what's still open

**Resolved this round:** build approach (custom code), hosting (Netlify/Cloudflare — easy + cheap), service area (3 counties incl. Pinellas), fee (from 7.5%), 12-month lease positioning, branding (new navy/teal/gold "Harbor" brand created — your logo didn't actually upload, only the two PDFs did), screening + payments (DoorLoop), and the application flow (apply → pay → self-entered SSN screening).

**Still useful from you, to take it from "demo" to "live":**

1. **Sign up for DoorLoop** (or your chosen platform) so we can wire the real Apply / Pay-Rent / Maintenance flows behind the buttons. This requires your business identity for setup.
2. **Real local data per neighborhood** — current rent ranges and any specifics you want emphasized. The area pages use clearly-flagged illustrative ranges right now.
3. **A logo file** (PNG/SVG) if you want your existing mark instead of the new one I designed — it didn't come through in the upload.
4. **A branded email** (e.g., info@tampabaypropertyexperts.com) to replace the personal Gmail/Live addresses currently public.
5. **Connect the forms** — at launch the demo forms need to post somewhere (your inbox, DoorLoop, or a form service). Quick to wire up.
6. **Photography** — I used licensed-style stock imagery as placeholders; real photos of your properties/team will lift it further.

---

## 11. Files delivered (this build)

A full multi-page site in your project folder: `index.html` (home), `owners.html`, `tenants.html`, `apply.html`, `pay-rent.html`, `maintenance.html`, `areas.html`, six neighborhood pages (`area-carrollwood`, `area-northdale`, `area-south-tampa`, `area-new-tampa`, `area-wesley-chapel`, `area-st-petersburg`), `about.html`, `contact.html`, `blog.html`, one full sample post, and a shared `styles.css`. Open `index.html` to explore — every nav link works.

---

## 10. Suggested order of operations

1. ✅ New homepage (draft delivered) → refine with your branding.
2. Build owner services page + about/contact.
3. Build all 11 neighborhood pages (biggest SEO win).
4. Set up & optimize Google Business Profile + reviews habit.
5. Stand up `/apply` + secure SmartMove screening (fixes the SS# problem).
6. Stand up `/pay-rent` ACH portal (Dwolla or Stripe).
7. Launch blog; I run a scheduled task drafting posts on your cadence.
8. Fix NAP citations everywhere (and that ZIP typo).
