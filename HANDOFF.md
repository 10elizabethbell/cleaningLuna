# Cleaning Luna LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/cleaningLuna/ · **Repo:** https://github.com/10elizabethbell/cleaningLuna · **Built:** 2026-10-17 from Muse brief (run 2026-10-17, NJ Small Business Network flyer post)

## What's built
- One page, phone first: header (CL moon mark + "Cleaning Luna", number top-right) → hero → What we clean → Booking starts with one message (night) → Tell us about your place (form) → Book your cleaning today (night, moon) → footer with the full logo.
- **World:** the room they clean. Cream wall, honey hardwood floor in perspective, brass threshold; navy night sections with gold stars and moon from the logo. Desktop adds a moonlit window on the wall that the clean floor reflects.
- **Signature element:** the hero floor is dusty (grey haze, pale shoe prints, scuffs, crumbs, sawdust, grit). A navy microfiber mop works it in figure-eights by itself; touch or mouse takes over (drag works up, down and sideways on phones). Clean wood shows the varnish and the window reflection, just-mopped wood stays a shade darker until it dries, gold four-point sparkles (the logo's) pop behind the mop, debris gets pushed and swept off the edges, and dust creeps back over a few seconds. Night-section stars spring away from a finger and keep clear of text. Day/night seams are moving gold lines.
- **Contact:** everything goes to WhatsApp (wa.me/19732462624) with pre-written messages: the hero button, each of the 11 service rows ("I'd like to book: Deep Cleaning."), the form (name, services, where, when, notes → one composed message, with a copy fallback), the close button. The number in the header and footer is a `tel:` link.
- Tunables are in `TUNE` at the top of the script (mop size, dust regrow, wet fade, debris count, sparkles, stars, seam speed).
- Verified in Chromium and WebKit at 360/390/430/1440: no sideways scroll, tap targets ≥44px, inputs ≥16px, the first phone screen shows headline + WhatsApp button + number + ~200px of floor, touch drags mop without scrolling the page, every WhatsApp text decodes, and form validation works.

## Assumptions I made
- **Colors** are sampled from the logo: navy `#072752` → `#0a2a58`, gold `#d6a035`. The cream wall is my choice, to match the logo's white ground.
- **Serif headings** use the system serif stack (Iowan Old Style/Palatino/Georgia) to echo the logo's "CL" monogram. This is still system fonts only, but not the usual sans display. On Android it falls back to Noto Serif.
- **"We" voice,** going by "Professional Team" in their post.
- **The service groups** (Homes / Rentals & businesses / Job sites) are mine. Row labels are shortened ("Concrete & wood haul-away"); the WhatsApp messages use their exact service names.
- **Copy that's mine, not theirs:**
  - the hero promise ("We look after your home, your rental or your office like it's our own…")
  - the three booking steps
  - "We'll read it on WhatsApp and get back to you with a quote."
  - "Get a quote" (I didn't say "free": the brief doesn't say quotes are free)
- **The phone number is a `tel:` link** in the header and footer. The brief only shows it as a WhatsApp number, so voice calls are unconfirmed.
- **Service area** is exactly "Elizabeth, NJ and the surrounding areas". I listed no towns.

## Placeholders and gaps
- **No work photos, before/afters or reviews,** so there's no proof section. This is the biggest gap.
- **Facebook** goes to Rosa's personal profile, and only from the footer. The rules want the Facebook link under the work photos; there are none yet, and a personal profile isn't a business page.
- **No email, hours, prices, years in business or insurance;** none appear on the page.
- **The logo** is the AI-style render from the flyer post (1254px JPG on white). The header uses a crop of the mark. The script wordmark couldn't be cut out cleanly because it touches the moon swoosh, so the header name is typed lettering. Favicon and home-screen icon are from the mark.

## Questions for the owner
1. Does 973-246-2624 take regular calls and texts, or WhatsApp only?
2. Can you send 6–10 photos of real jobs, especially before/afters (deep clean, move-out, post-construction)?
3. Do you have a business Facebook or Instagram page we can link instead of your personal profile?
4. Is the quote free? Do you want any starting prices shown?
5. Which towns do you cover besides Elizabeth (Union, Linden, Hillside, Roselle, Newark…)?
6. Hours, and do you work weekends?
7. A business email for the footer?
8. Should the site also be in Spanish? (Elizabeth has a large Spanish-speaking population.)

## Ideas not built (yours to pick)
- **Runner-up world:** a moonlit window you wipe clean with a squeegee, with fog and suds on the glass over a night sky and moon. It's the most literal "Luna" idea and would pair well with the logo.
- **Proof section** with before/after sliders (plain gold divider) as soon as photos exist, with "Click to see more of our work." linking to a business page directly under them.
- **Spanish toggle** (EN/ES) with the WhatsApp messages translated too.
- **Holiday / party-season cleaning promo** line or banner (Muse flagged the timing). Only if the owner confirms an offer.
- **Airbnb host turnover checklist** module for rental hosts.
- **A self-hosted serif** (e.g. Cormorant or Playfair subset, ~20KB) to match the logo's monogram on every phone.
- **Floor tuning:** `TUNE.regrow` (dust return speed), mop size, sparkle rate, and how dark the wet streak is (`globalAlpha .35` in `draw()`).
- Desktop "What we clean": the 5/3/3 rows leave a little air under the 2nd and 3rd columns.

## Not verified
- A real-device touch feel and frame rate on older Android phones (the floor redraws several full-canvas layers a frame; DPR is capped at 1.5).
- The WhatsApp handoff inside Facebook's in-app browser on iOS and Android (`wa.me` should open the app).
- Android serif fallback appearance.
- The link preview in Facebook's own debugger (og image is at `/assets/og.jpg`, 1200×630).
