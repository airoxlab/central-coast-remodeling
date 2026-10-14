# Central Coast Remodeling — Santa Maria, CA

Single-page sample site for a licensed B-2 residential remodeling contractor in
the Santa Maria Valley. Built as a free sample for a warm SMS lead with no
online presence at all.

## Business details

| | |
|---|---|
| Business | Central Coast Remodeling |
| Owner | **Not public** — ask him |
| Phone | (805) 448-9462 (mobile — call and text both offered) |
| Location shown | **Santa Maria, CA** (see below) |
| Website | None |
| Google Maps | **Not listed** |

## Licence — verified

Checked against the CSLB database on **2026-10-14**, licence **#1153899**:

- **CENTRAL COAST REMODELING**, 395 Crescent Ave
- Business phone (805) 448-9462 — matches the number he was texted on
- Issued **04/21/2026**, expires **04/30/2028**
- **This licence is current and active.**
- Classification **B-2 — Residential Remodeling**
- Contractor's bond with **Merchants Bonding Company (Mutual)**, **$25,000**
- **Workers' compensation: exempt** — certified no employees

He is comp-exempt, so the site says **"licensed & bonded"** and **never
"insured"** — a grep for "insured" returns zero. The licensing section frames it
as "owner-operated", and the services section turns it into a selling point:
*"No sales rep, no subcontracted crew turning up unannounced."*

## ⚠️ CSLB has his city wrong — and directories are repeating it

**CSLB lists him as "SANTA MONICA, CA 93455".** That is a data error:

- **ZIP 93455 is Santa Maria / Orcutt.** Santa Monica is 90401–90405.
- **395 Crescent Ave geocodes to Santa Maria, CA 93455** (Mission Highlands,
  Orcutt), confirmed independently.
- A **Nextdoor listing** for Central Coast Remodeling gives **4614 Harmony Lane,
  Santa Maria**, same phone number — a second, independent Santa Maria address.

**This is costing him real money.** Licence-scraper directories have copied the
error, so he currently appears on sites like truelocalpros.com and
localcontractorslist.com under **"Bathroom Remodeling in Santa Monica"** and
**"Renovation Contractors in Santa Monica"** — 150 miles from where he works.
Anyone finding him there will not call, and anyone in Santa Maria will not find
him at all.

**Tell him to correct the address with CSLB.** It is a free change through their
licensee portal, and the directories refresh from CSLB. That is worth more to him
than the website in the short term.

The site shows **Santa Maria** throughout, and no street address at all.

## A near-miss worth recording

A Google result appeared to show an Instagram post reading *"CENTRAL COAST
REMODELING · QUALITY CRAFTSMANSHIP. TIMELESS RESULTS. · 805-448-9462 · LICENSE
#1153899 · KITCHENS • BATHROOMS • ADDITIONS"*.

Opening that post showed it belongs to **forgeconstructionllc**, a different
company in **Naples, Florida** (the post is about a job on Lagos Way in
Mediterra). Google had merged two unrelated results on one page.

**Four images scraped from it were discarded**, and no Instagram account is
claimed on the site. The tagline is not used either, since it cannot be shown to
be his.

**Worth asking him directly** whether he has an Instagram — if that strapline
really is his it is good copy, but it could not be verified.

## What was deliberately not built

- **No reviews or testimonials.** Nothing exists anywhere.
- **No years-in-business claim.** Licensed April 2026 (~6 months).
- **No owner name.** Not published anywhere.
- **No "insured" claim** — comp-exempt.
- **No street address** — 395 Crescent Ave is residential.
- **No Instagram link or tagline** (see above).

## Images

`img/` — six stock photos (Unsplash): kitchens, bathrooms, flooring and living
spaces. He has no photos of his own. Disclosed under the gallery and in the
footer.

Two candidates were discarded for showing the wrong subject (a welder labelled
"carpenter", plus the four Florida images above).

**Before/after project photos are the biggest upgrade available** — remodeling
sells on them more than almost any other trade.

## The estimate form

Builds a pre-filled **text** to (805) 448-9462 with name, phone, city, project
type and details, and prompts the visitor to attach photos of the room.

SMS rather than email because it is a mobile number, he has no published business
email, and remodel enquiries start with photos.

**Tested functionally in a browser:**

| Test | Result |
|---|---|
| Submit with empty fields | Rejected |
| Honeypot filled (bot) | Silently accepted, nothing sent |
| Valid submission | Correct `sms:` URI with all fields |
| JS errors | None |

## Design

- Charcoal `#1A1714` navbar and bands, coastal teal `#2F6F7E`, clay `#C2704A`
  and sun `#D7A74B` on warm sand — Central Coast rather than generic.
- Archivo (display) + Inter (body).
- Inline SVG roofline-over-waves mark, tying the name to the coast.
- Nine sections: hero, credential strip, services, owner-operated band, process,
  licensing, work gallery, service areas, estimate form, contact.
- Full dark mode, sticky header, `scroll-margin-top` anchors, reduced-motion
  respected, inline CSS, no build step.
- Sendra visit-tracking script before `</body>`.

## Open questions for the client

1. **His first name.**
2. **Confirm the city** — Santa Maria, and whether he will fix it at CSLB.
3. **Does he have an Instagram?** (See the near-miss above.)
4. **Project photos**, especially before and after.
5. **Which remodels** he wants more of — kitchens, bathrooms, whole-house?

## The name problem

"Central Coast" is the most generic possible name for the region, and **five
other building companies hold it on Google Maps around Santa Maria**:

- Central Coast Construction (Santa Maria)
- Central Coast Builder (Orcutt, 5.0★)
- Central Coast Renovations (Atascadero, 5.0★, has a website)
- Central Coast Marble and Granite (4.8★)
- Central Coast Maintenance

He has **no listing at all**, so every one of those captures searches meant for
him. Combined with the Santa Monica address error, he is effectively invisible in
his own market.

**Two fixes, in order: correct the CSLB address, then create a Google Business
Profile for Santa Maria.** The website gives both somewhere to point.

Not to be confused with **Central Coast Renovations** (Atascadero,
(805) 400-9584, centralcoastrenovations.com).
