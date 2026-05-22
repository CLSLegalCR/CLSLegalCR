# CLS Discovery & Content Meeting — Open Questions

Prepared: 2026-05-21
For the content review + onboarding meeting (next week)

Everything below comes from comparing the three documents CLS sent (`Law Firm_CLS Legal CR.pdf`, `Manual de Uso Correcto del Logo.pdf`, `Presentación Logotipo CLS.pdf`) against each other and against the demo site. Bring this list to the meeting — most items require their direct confirmation.

---

## 🚨 Inconsistencies in CLS's Own Materials

These are conflicts *between* their own provided documents. Only CLS can tell us which is correct.

### 1. Main phone number — two different numbers

| Source | Phone |
|---|---|
| Law Firm overview deck | `+506 5056 5736` |
| Business card (brand manual) | `+506 6056 5736` |
| Current demo site | `+506 6056 5736` *(matches business card)* |

**Ask:** Which is the correct main number? The other one — typo somewhere?

### 2. Office address — two different addresses, two different postal codes

| Source | Address |
|---|---|
| Law Firm overview deck | Century 21 Caribe Real Estate Puerto Viejo · Frente Restaurante El Rincon Portello · Limón, **Puerto Viejo de Talamanca, 70402** |
| Business card (brand manual) | **Talamanca, Punta Cocles**, en C21 Segundo Piso Oficina CLS · **70403** |

**Ask:** What's the actual office address as it should appear on the website / Google Maps / Schema markup? Both versions reference C21 (Century 21) but the location and postal code differ.

### 3. Services list — three different lists across their own materials

| Source | Services listed |
|---|---|
| **Logo tagline** (brand manual) | REAL ESTATE · CORPORATE · TAX *(3 items)* |
| **Law Firm overview deck — Areas of Practice** | Real Estate · Corporate · Tax · **Labor** *(4 items)* |
| **Instagram bio** (shown in brand manual mockup) | Corporate · Tax Advisory · **Environmental** · Labor *(4 items, includes Environmental but not Real Estate)* |

**Ask:** What is the canonical, complete list of legal services CLS offers? This needs to be locked down for:
- Site structure (which services get pages, which get summary mentions)
- Schema markup
- llms.txt
- AI visibility queries we target

### 4. Immigration — listed nowhere in their official docs

Their Law Firm overview deck's "Areas of Practice" lists only Real Estate / Corporate / Tax / Labor. Immigration does not appear in any of their docs.

The demo site I built (as a sales tool) leads with Immigration because of the strategic expat-market angle in our audit. That positioning landed CLS as a client, so it's not wrong — but we need to confirm with them:

**Ask:** Do you actually handle immigration cases (residency, work permits, pensionado/rentista visas)? If yes, why isn't it in your official Areas of Practice doc? If no, we need to reposition the homepage strategy.

---

## 📂 Missing Assets We Need From CLS / Rebeca Escalante

### 5. Original logo files

The brand manual is a presentation deck — it shows the logo as rendered vector paths, but doesn't ship the logo as a separate file. For now I've cropped a screenshot from the manual (50 KB PNG, decent quality), but this is a temporary substitute.

**Request from CLS (who can pass it to Rebeca Escalante, the designer):**
- Vector source: `.svg` or `.ai` or `.eps`
- High-res PNG with **transparent background** (for use on dark/light backgrounds)
- All approved variations: gold-on-dark, white-on-dark, black-on-white, monogram-only (just the CLS mark, no text)
- Favicon-friendly version (just the monogram, square)

### 6. Real photographs

The Law Firm overview deck has beautiful photos — office in nature, attorney portraits, supporting business imagery. We need:
- The actual office exterior/interior photos (high-res)
- Both attorney portraits (high-res)
- Permission to use them on the website
- Photo credits if needed

### 7. Attorney bios

We have names, titles, emails, phones — but no bio paragraphs:
- **Mario Andrés Hernández Bertarioni** — Lawyer & Notary — Andres@clslegalcr.com
- **Javier Antonio Guerrero Alvarez** — Lawyer & Notary — Javier@clslegalcr.com

**Ask:** Each attorney's:
- Education (where, when)
- Years of experience
- Specialty areas
- Bar admission / notary credentials
- Languages spoken
- 2-3 sentence "about me" paragraph for their page

### 8. Testimonials

The site currently has **fabricated placeholder testimonials** (Michael Thompson / Sarah & David Miller / Hans Weber — none of these are real CLS clients).

**Ask:** 3-4 real client testimonials. Options:
- Existing written reviews from clients (with permission to reuse)
- Pull quotes from existing Google Reviews (their GBP shows 4.5★ with 16 reviews)
- Write together at the meeting based on past cases they remember
- First name + country/category is enough, full names optional

---

## ✅ What We Have Confirmed (Just Need Their Sign-Off)

### 9. Brand palette (already locked from their manual)

| Color | Name | Hex |
|---|---|---|
| 🟡 Primary gold | Mustard Yellow | `#DEAA09` |
| ⬛ Dark | Charleston Green | `#282C2D` |
| 🔘 Mid grey | Davy's Grey | `#4E5354` |
| 🟦 Slate | Stormcloud | `#4E6365` |
| ⬜ White | Ghost White | `#FAFDFE` |

### 10. Typography (already locked)
- **Arial** in Regular / Bold / Italic / Bold Italic

### 11. Firm culture pillars (from Law Firm deck)
- Collaborative Teams · High-Pressure · Client-Focused · Ethical Standards

### 12. About-us copy (from Law Firm deck — ready to use)
> *"Caribe Legal Services is a law firm with solid legal experience and a clear strategic vision, focused on providing comprehensive, secure, and tailored legal solutions in Costa Rica's Caribbean region. We advise companies, national and international investors, and individuals, supporting them at every stage of the legal decision-making process through preventive legal counsel, sound legal structuring, and reliable representation..."*

**Ask:** Sign-off — are you comfortable with this copy as written, or do you want to revise before it goes on the public site?

---

## 📋 Site Configuration Questions

### 13. Languages
The demo has bilingual ES/EN with full mirror pages. Confirm:
- Both languages confirmed as service offerings?
- Which is the primary (default landing language)?

### 14. Hours of operation
Demo currently shows "Monday–Friday, 9:00 AM – 5:00 PM."
- Confirm exact hours
- Lunch break / closed periods?
- Holiday/seasonal variations?

### 15. WhatsApp number
The current site has a WhatsApp link to `+50660565736`.
- Confirm this is monitored
- Should it be the same as the main phone (once that's resolved per Q1)?

### 16. Social media accounts
The brand manual shows an Instagram account: `cls_legal_cr` (with 42.6K followers and 2000 posts visible in the mockup).
- Confirm Instagram URL: instagram.com/cls_legal_cr
- Confirm Facebook URL (currently demo points to facebook.com/clslegalcr)
- Any other social accounts (LinkedIn, X/Twitter, YouTube)?

### 17. Google Business Profile
- Confirm the existing listing (Law Firm deck shows 4.5★ / 16 reviews at "Century 21 Caribe Real Estate Puerto Viejo")
- Will CLS add `hello@vizacat.com` as Manager during the setup walkthrough?

### 18. Stripe / online payments
- Does CLS want to take consultation payments online via the new site?
- If yes, we set up Stripe during the onboarding session.

### 19. Business email
- Currently the law firm uses `Andres@clslegalcr.com`, `Javier@clslegalcr.com`, `Info@clslegalcr.com`
- Is the `Info@` mailbox actively monitored, or is it a forward?
- Do they want a `contacto@clslegalcr.com` Spanish version added?

---

## 🗓️ Meeting Agenda Checklist

Bring this list. Suggested order:

1. **Quick site walkthrough** — review every page together (~20 min)
2. **Lock the inconsistencies** — items 1–3 above (phone, address, services list) (~10 min)
3. **The Immigration question** — item 4 (~5 min strategic conversation)
4. **Gather missing assets** — items 5–8 (logo files, photos, bios, testimonials) (~15 min, may require follow-up email)
5. **Configuration confirmations** — items 13–19 (~15 min)
6. **Account setup walkthrough** — Vercel, GoDaddy DNS, GBP (~60 min from the onboarding doc)

**Total estimated:** ~2 hours. Block the time accordingly.

---

*This document is the source of truth for the discovery phase. Update with answers as they come in.*
