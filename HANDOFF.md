# Cleaning Luna LLC — handoff at ~60% (calm-style revamp)

**Live:** https://10elizabethbell.github.io/cleaningLuna/ · **Repo:** https://github.com/10elizabethbell/cleaningLuna · **Built:** 2026-10-17 from Muse brief (run 2026-10-17, NJ Small Business Network flyer post) · **Revamped:** 2026-10-19 to the calm band style

## What changed in the revamp (2026-10-19)
The business hasn't been contacted yet, so the whole site was rebuilt under the new house default (`calm-photo-style.md`, learned from lpmr.co.uk), copied from the DPG reference build.
- **Removed:** the mopped-floor canvas hero, the moonlit-window illustration, the star canvases in the night sections, the moving gold seams, the serif headings, the cream wall, and the gold burst on chip ticks. All of it is in git history (last commit of that world: `81c63b2`).
- **Look:** paper / navy / midnight bands, coloured from the logo. Navy is `#173d7a`, midnight is `#0a2350` with the faint diagonal texture, and the logo's moon gold `#d6a035` is used only as a fill, with navy text on it. Gold as text on light uses `#7f5a12` (5.8:1). Headings are Cal Sans from Google Fonts, body text is the system stack at 16/1.7. Pill buttons, a 24px form card, and 10px fields on `#e6ecf5`.
- **Hero:** the plain textured navy band, because there are no work photos (the flyer post's only image is the logo). It has:
  - the eyebrow "Homes, businesses & job sites"
  - the H1 "In Elizabeth, we clean. You relax." (their tagline plus the place), which bounces in letter by letter
  - one promise line
  - "Book on WhatsApp" (gold) and "Get a quote" (outline)
  - the logo's gold crescent: 72px in the top corner on phones, about 300–380px at the right on desktop
- **Sections:** hero → "We treat your place like our own." with their own three words (Reliable service / Professional team / Quality work) → "What we clean." service rows on navy in three groups → "Booking takes one message." three steps on midnight → quote form → "Book your cleaning today." close → footer.
- **Contact wiring:**
  - Service rows no longer open WhatsApp directly. They jump to the form with that service already ticked (calm kit pattern), so a row and the floating circle never offer the same action.
  - The form composes one WhatsApp message (name, services, where, optional when and notes). If WhatsApp doesn't open, it shows "Thanks, {name}…", the message itself, "Open WhatsApp", "Copy message" and the number as plain text.
  - The closing band's big number is now a WhatsApp link, not `tel:`, because booking is WhatsApp-only per the brief.
  - The header number stays a `tel:` link (house rule: tap-to-call number top right).
- **Floating circle:** 60px, gold, opens WhatsApp with "Hi Cleaning Luna! I'd like to book a cleaning." It shows once the hero is gone and hides while the form or the closing WhatsApp link is on screen. It is `hidden` without JS.
- **Motion:** the H1 bounce-in and one 12px fade-up (`.rise`), nothing else. Reduced motion and no-JS show everything at once (checked).
- **Link preview:** a new `assets/og.jpg` (1200×630) of the calm hero.
- **Process:** Impeccable sweep (audit, critique, polish, clarify, distill, harden, adapt, optimize, animate, colorize, typeset, layout, delight, bolder, quieter) plus the finish reviewer. Their fixes are applied; the conflicts are listed below. The detector is clean apart from two recorded exceptions (the band texture, and a type-scale reading that ignores the clamped headings). DESIGN.md was regenerated from the new build.

## Verified
- **Live:** the Pages build of `6062528` is served at the link above, checked in WebKit at 390px (new hero, Cal Sans loaded, og image 200). The Call Sheet already had this URL (`call-sheet-site.sh` printed UNCHANGED).
- Chromium and WebKit at 320, 360, 390, 430, 844×390 (landscape) and 1440:
  - no sideways scroll
  - tap targets 44px or more
  - inputs at 16px or more
  - "Book on WhatsApp" is on the first screen at every size, landscape included
- H1: letters are offset early on, and the plain heading is restored once they settle. "You relax." stays on one line.
- Floating circle: hidden on the hero, shown over the services, hidden over the form and over the close.
- Form:
  - errors show and focus the first bad field, with the red border kept while focused
  - a service row pre-ticks its chip
  - the composed WhatsApp URL decodes correctly
- Contrast: lowest text pair is 4.5:1 (gold "You relax." on navy, large text); everything else is 5.8:1 or higher.
- No template leftovers (`123456789`, `domainname`, bare facebook.com, lorem, demo/sample, mailto).

## Assumptions I made
- **Colours** are taken by eye from the logo: navy, midnight and moon gold. The paper ground is the house default.
- **"We" voice,** going by "Professional Team" in their post.
- **Copy that's mine, not theirs:**
  - "You book with one message. We take it from there."
  - "We treat your place like our own." and its two-line lede
  - the three steps
  - "Not sure we cover your street? Ask us."
  - "Get a quote" (I didn't say "free": the brief doesn't say quotes are free)
- **The service groups** (Homes / Rentals & businesses / Job sites) are mine. Labels are shortened; the WhatsApp message uses their exact service names.
- **The header `tel:` link.** The brief only shows the number as WhatsApp, so voice calls are unconfirmed.

## Placeholders and gaps
- **No work photos, before/afters or reviews,** so there's no proof section and the hero is the plain navy band. This is the biggest gap. With 3+ real job photos, the hero should become a photo under navy (house rule) and a work-card section with a Facebook link under it.
- **Facebook is in the footer only.** It goes to Rosa's personal profile; there's no business page and no work section to put it under.
- **No email, hours, prices, years in business or insurance.** None of them are on the page.
- **The logo** is the AI-style render from the flyer. The header uses the CL moon mark (multiply-blended so its white square disappears on the paper header). The favicon and home-screen icon are from the same mark.

## Questions for the owner
1. Does 973-246-2624 take regular calls, or WhatsApp only? (If WhatsApp only, the header number should become a WhatsApp link too.)
2. Can you send 6–10 photos of real jobs, especially before/afters (deep clean, move-out, post-construction)?
3. Do you have a business Facebook or Instagram page to link instead of your personal profile?
4. Is the quote free? Do you want any starting prices shown?
5. Which towns do you cover besides Elizabeth?
6. Hours, and do you work weekends?
7. A business email for the footer?
8. Should the site also be in Spanish?

## Ideas not built (yours to pick)
- **Runner-up worlds (opt-in signature motion), from the trade:**
  1. A moonlit window you wipe clean with a squeegee, fog and suds on the glass over a night sky. The most literal "Luna" idea; this is the one I'd add.
  2. The old dusty floor you mop by finger (in history at `81c63b2`).
  3. Sparkles that pop where you touch a just-cleaned counter.
  4. A dust sheet pulled off the hero.
  5. Foam on a tile wall rinsing away.
- **Spanish toggle** (EN/ES), with the WhatsApp messages translated too.
- **Self-hosted Cal Sans subset** to save two round trips on cellular. The house rule says Google Fonts, so I left it.
- **Desktop form column:** about 900px of empty paper under the sticky heading. Proof photos or reviews would fill it once they exist.
- **Holiday/party-season promo line,** only if the owner confirms an offer.
- **Impeccable findings I didn't apply because they remove Ellie's chosen calm-style features:**
  - eyebrow pills (the craft floor bans them)
  - the H1 bounce-in (Impeccable says "no bounce or elastic", and the headline isn't readable for about 1.5s)
  - `.rise` on every section ("one focal sequence")
  - the band texture ("decorative stripes")
  - the floating circle
  - Google-hosted Cal Sans
  - the gold last phrase on dark-band headings (Impeccable: "gold stops meaning anything"; the house rule asks for it)
  - row focus shown on the arrow only (Impeccable wants a whole-row ring)
- **Not applied, for other reasons:**
  - The calm kit's header shadow on scroll: the header isn't sticky (same as DPG), so there's nothing for a shadow to separate.
  - The floating circle can sit over a service row's arrow as you scroll on phones. Tapping it still opens WhatsApp, and hiding it over the services would leave it hidden most of the page.
  - Without JS the form does nothing useful (same as DPG).

## Not verified
- Real-device touch, and the WhatsApp handoff (`wa.me`) inside Facebook's in-app browser on iOS and Android.
- The link preview in Facebook's own debugger.
- Cal Sans rendering on old Android.
