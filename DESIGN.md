---
name: Cleaning Luna LLC
description: We clean. You relax. A local Elizabeth, NJ cleaning crew, booked by one WhatsApp message.
colors:
  navy: "#0a2a58"
  navy-2: "#13386f"
  navy-ink: "#0b2246"
  night: "#0c2550"
  gold: "#d6a035"
  gold-hi: "#f2cf74"
  gold-deep: "#8f6416"
  accent: "#2a6fdb"
  wall: "#f8f3ea"
  paper: "#fffdf8"
  line: "rgba(10,42,88,.14)"
  muted: "#4a5a78"
  night-text: "#dfe6f3"
  night-muted: "#b4c1da"
  error: "#b3261e"
typography:
  display:
    fontFamily: "\"Iowan Old Style\", \"Palatino Linotype\", Palatino, \"Book Antiqua\", Georgia, serif"
    fontSize: "clamp(2.9rem, 13.2vw, 6rem)"
    fontWeight: 700
    lineHeight: 0.98
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "\"Iowan Old Style\", \"Palatino Linotype\", Palatino, \"Book Antiqua\", Georgia, serif"
    fontSize: "clamp(2rem, 7.4vw, 3.25rem)"
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.01em"
  title:
    fontFamily: "\"Iowan Old Style\", \"Palatino Linotype\", Palatino, \"Book Antiqua\", Georgia, serif"
    fontSize: "24px"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "-0.01em"
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, \"Segoe UI\", Roboto, \"Helvetica Neue\", Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 700
    lineHeight: 1.3
rounded:
  field: "14px"
  panel: "16px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter-phone: "16px"
  gutter-wide: "32px"
  max: "1180px"
  section-phone: "64px"
  section-wide: "96px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.navy-ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.gold-hi}"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.navy}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-secondary-hover:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.wall}"
  button-secondary-night:
    backgroundColor: "transparent"
    textColor: "{colors.night-text}"
    rounded: "{rounded.pill}"
    height: "56px"
  service-row:
    textColor: "{colors.navy-ink}"
    padding: "8px 0"
    height: "60px"
  service-arrow:
    backgroundColor: "transparent"
    textColor: "{colors.navy}"
    rounded: "{rounded.circle}"
    size: "40px"
  service-arrow-hover:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.navy-ink}"
  chip:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.pill}"
    padding: "8px 16px"
    height: "44px"
  chip-selected:
    backgroundColor: "{colors.navy}"
    textColor: "#ffffff"
  input:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.navy-ink}"
    rounded: "{rounded.field}"
    padding: "13px 16px"
    height: "54px"
  step-ring:
    textColor: "{colors.gold-hi}"
    rounded: "{rounded.circle}"
    size: "52px"
---

# Design System: Cleaning Luna LLC

## Overview

**Creative North Star: "The Room After We Leave"**

The page is the room the crew cleans. Day sections are a cream painted wall; the hero floor is honey hardwood seen from the doorway, dusty until it is mopped; night sections are the sky outside the window ("Luna"), full of stars. Deep navy and warm metallic gold come straight from the logo's CL monogram and crescent moon, and gold is spent only where something is clean or active. The visitor does the cleaning: the hero floor responds to a finger before anything else on the page asks for one.

Density is calm and phone-first: one column, generous section padding, lists as rows rather than cards, and every interactive element at least 44px tall. Type is system-only by house rule (no web fonts): a bookish serif stack echoing the monogram for display, the platform sans for everything read. Depth is mostly tonal (wall vs. paper vs. night) with a few physical cues taken from the room: a baseboard shadow, a brass threshold, a soft drop under the gold button.

**Key Characteristics:**
- Two grounds, day (cream wall) and night (deep navy sky), joined by animated gold wave seams.
- Gold means clean or active: buttons, sparkles, hovered arrows, the threshold. Never decoration on resting text.
- Serif display with an italic gold second half; system sans body.
- Rows, not cards. Pills for actions and choices, circles for markers.
- A living hero floor and pointer-shy night stars; reduced motion gets a still frame.

## Colors

Logo navy and logo gold on a warm cream wall, with a night navy for the sky and one cool blue kept off the brand entirely, reserved for form outlines.

### Primary
- **Monogram Navy** (navy): headline color, outline button stroke and text, brand wordmark, selected chips, arrow glyphs. The brand's voice on light grounds.
- **Ink Navy** (navy-ink): body text on the wall and paper, label text, text on gold buttons.
- **Group Navy** (navy-2): the italic service-group titles ("Homes", "Job sites"); a half-step lighter than the headline so the groups sit beneath it.

### Secondary
- **Crescent Gold** (gold): primary button fill, hovered service arrow fill, sparkle base, the center line of the wave seam, the threshold's mid-stop.
- **Moonlight Gold** (gold-hi): primary button hover/active, step-ring numerals and rings on night, sparkle highlights.
- **Brass Gold** (gold-deep): the italic "You relax." half of the hero headline, the phone glyph, phone hover, the text caret. The only gold dark enough to carry text on cream.

### Tertiary
- **Form Blue** (accent): focus-visible outline sitewide (3px, offset 3px), and the hover/focus border plus 3px halo (`rgba(42,111,219,.18)`) on inputs and chips. Deliberately outside the brand so it never competes with the gold buttons.

### Neutral
- **Painted Wall** (wall): page ground, header, hero wall, day sections; also `theme-color`.
- **Fresh Paper** (paper): input and chip fills, the sent-message panel, footer ground, baseboard highlight.
- **Night Sky** (night): ground of the night sections (booking steps, closing call to book).
- **Hairline** (line): service-row dividers, resting arrow ring, footer top border, panel border.
- **Quiet Slate** (muted): section intro paragraphs, the hero promise, optional markers, copyright.
- **Starlight** (night-text) and **Dim Starlight** (night-muted): text and secondary text on night; night headlines go pure white.
- **Error Red** (error): field error messages and the invalid input border.

### Named Rules
**The Gold Is Clean Rule.** Gold appears only where something is clean or active: the primary button, sparkles, a hovered arrow, the threshold, the seams' light line, the step rings. Resting text and decoration stay navy.

**The Blue Belongs To The Form Rule.** Form Blue is used only for focus rings and form-control hover/focus outlines. It never fills anything and never appears as brand color.

## Typography

**Display Font:** Iowan Old Style (with Palatino Linotype, Palatino, Book Antiqua, Georgia, serif)
**Body Font:** System sans (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial)

**Character:** A warm book serif that echoes the logo's serif monogram, set bold and tight, against the platform's own sans for everything people actually read and tap. System-only stacks are the owner-pipeline house style; there are no web fonts and none should be added.

### Hierarchy
- **Display** (700, clamp(2.9rem, 13.2vw, 6rem), 0.98): the hero headline only. Its second half is italic Brass Gold on its own line ("We clean. / *You relax.*").
- **Headline** (700, clamp(2rem, 7.4vw, 3.25rem), 1.05): section h2s; the closing h2 scales up to clamp(2.3rem, 9vw, 4rem). Balanced wrapping.
- **Title** (700, 24px): italic serif for service-group names; upright serif for step titles on night.
- **Body** (400, 17px, 1.55): all reading text; intros capped near 44ch, the hero promise at 34ch and clamp(17px, 4.6vw, 20px).
- **Label** (700, 16px, 1.3): field labels and legends; button text is the same family at 700/17px; service rows 600/17px.
- **Serif italic aside** (400 italic, clamp(21px, 5vw, 24px)): the service-area line in the close section.

### Named Rules
**The Relaxed Half Rule.** Display lines that pair work and rest set the rest half in italic Brass Gold on its own line. One per page, in the hero.

**The System Stack Rule.** Display uses the serif stack, everything else the sans stack, both from the operating system. No font files.

## Layout

Single centered container (max 1180px) with a 16px gutter on phones and 32px from 760px, padded out to safe-area insets. Sections breathe at 64px top / 72px bottom on phones and 96px / 104px from 760px. Breakpoints in use: 380px (narrow-phone header shrink), 760px (gutters, side-by-side hero buttons, taller floor), 900px (three-up steps), 1024px (three-up service groups, hero wall gains the moonlit window in a 1fr / 340px grid).

The page alternates day and night: header and hero (wall) → services (wall) → steps (night) → quote form (wall) → book today (night) → footer (paper). The hero floor is full-bleed, clamp(250px, 40svh, 340px) tall on phones and clamp(300px, 44svh, 460px) wider, 180px in short landscape. The quote form column caps at 800px on desktop. Scroll padding is 72px.

**The Phone Screen Rule.** On a phone the first screen holds the header (mark left, phone number right), the two-line headline, one promise line, at most two buttons, and the start of the floor. Nothing else is added above the floor.

## Elevation & Depth

Flat and tonal by default: depth comes from the three grounds (wall, paper, night) and from the room's own physical edges rather than from floating surfaces. The few shadows are all part of the room or tied to the primary action.

### Shadow Vocabulary
- **Gold lift** (`box-shadow: 0 8px 18px -10px rgba(10,34,70,.45)`): under the gold button on day grounds only; removed on night.
- **Baseboard** (`box-shadow: 0 4px 8px rgba(60,35,10,.28)`): the 16px painted baseboard across the top of the floor.
- **Threshold** (`box-shadow: 0 3px 6px rgba(80,50,10,.25)`): under the brass strip that ends the hero.
- **Halo** (`box-shadow: 0 0 0 3px rgba(42,111,219,.18)`): inputs and chips on hover/focus.

### Named Rules
**The Room Has Edges Rule.** Shadows describe the room (baseboard, threshold) or the one action you should take (gold lift). Content blocks never float; there are no card shadows.

## Shapes

Three shapes only: the pill (999px) for every action and choice, the circle for markers (service arrows, step numerals), and a softly rounded field (14px inputs, 16px panel). Dividers are 1px hairlines; strokes on controls are 1.5px, on buttons and step rings 2px. Sections meet through wave seams: an SVG wave filled with the upper ground over the lower, crossed by a 2.5px gold line and two fainter gold lines that drift slowly (TUNE.seamSpeed). The hero ends on a 12px brass threshold gradient (#f4d98c → gold → #9c6d1b).

## Components

### Buttons
Confident pills, one gold and one quiet.
- **Shape:** full pill (999px), 56px tall, 26px side padding, icon 22px with 10px gap.
- **Primary (gold):** Crescent Gold fill, Ink Navy text, 2px navy border, gold lift shadow on day. Hover and press go to Moonlight Gold; press nudges down 1px.
- **Secondary (outline):** transparent with a 2px Monogram Navy stroke and navy text; hover fills navy with wall-colored text. On night the stroke and text become Starlight and hover inverts to Starlight fill with night text.
- **Form context:** the submit button and the copy button take a 3px Form Blue outline (offset 3px) on hover as well as focus.
- **Count:** at most two buttons together (hero: gold "Book on WhatsApp" + outline "Get a quote"); elsewhere a single gold button. Phones stack them full width; 760px+ sits them side by side.

### Service Rows
The services list is rows, not cards.
- **Row:** full-width link, 60px min height, 600/17px sans in Ink Navy, 1px hairline beneath. The row itself never changes on hover.
- **Arrow circle:** 40px circle with a 1.5px hairline ring and a navy 18px arrow. On row hover or focus only the circle fills Crescent Gold (ring gold, glyph Ink Navy); on keyboard focus it also takes the Form Blue ring.
- **Groups:** italic serif title in Group Navy above each list; one column on phones, three from 1024px.

### Chips
- **Style:** pill, 44px min height, Fresh Paper fill, 1.5px stroke `rgba(10,42,88,.28)`, 600/16px sans.
- **State:** hover or keyboard focus shows the Form Blue border plus halo; selected fills Monogram Navy with white text (hover keeps the blue border). Ticking a chip releases a 600ms burst of four gold sparkles (skipped under reduced motion).

### Inputs / Fields
- **Style:** Fresh Paper fill, 1.5px stroke `rgba(10,42,88,.28)`, 14px radius, 54px min height (textarea 110px, vertical resize), 17px text, Brass Gold caret.
- **Focus / Hover:** Form Blue border plus 3px halo; no default outline.
- **Error:** Error Red border on the input and a 600/16px Error Red message below; optional fields marked with a muted "(optional)".
- **Sent panel:** Fresh Paper, 16px radius, hairline border, holding the composed message and a small 44px outline pill to copy it.

### Navigation
A plain header, not a nav bar: CL moon mark (44px, 52px wide) with the italic serif "Cleaning Luna" wordmark on the left, the tap-to-call number top-right in 700 sans with tabular figures and a Brass Gold phone glyph (hover turns the number Brass Gold). The header scrolls away; there is no sticky element.

### Step Rings
On night, booking steps are a 52px circle with a 2px `rgba(242,207,116,.7)` ring and a Moonlight Gold 24px serif numeral, beside a white serif title and Dim Starlight text. Stacked on phones, three-up from 900px.

### Hero Floor (signature)
A canvas drawn as dusty honey planks in perspective under a painted baseboard, ending at the brass threshold. A navy microfiber mop (pad #1b3d78 with lighter navy loops, silver handle, gold joint) runs figure-eights on autopilot until the visitor touches or hovers the floor, then follows the pointer; it returns to autopilot after TUNE.idleMs (2600ms) of stillness. Mopping wipes the dust layer, leaves a drying wet streak (TUNE.wetFade), pushes crumbs, sawdust and grit ahead of the pad until they pile at the baseboard or sweep off, and drops gold four-point sparkles (the logo's star, TUNE.sparkleChance). Clean wood shows the moonlit window's reflection. Dust creeps back at TUNE.regrow (0.0035 per frame) so a clean patch lasts a few seconds. A white hint with a hand glyph sits bottom-left on a dark scrim and fades after the first mop. All tunables live in the `TUNE` object (planks, pad size, debris counts, stars, seam speed). Under reduced motion the floor draws one still frame and allows vertical page panning.

### Night Stars (signature)
Each night section carries a full-bleed canvas of small white stars plus a few larger gold four-point sparkles (TUNE.starsPhone 34, starsDesktop 80) that twinkle and drift slightly. Stars are placed away from text boxes, spring aside from a pointer within about 110px, spring back home, and bounce off text instead of crossing it. Reduced motion draws them once, still.

## Do's and Don'ts

### Do:
- **Do** keep gold for clean or active things: the primary button, sparkles, the hovered arrow circle, step rings, seam lines, the threshold.
- **Do** use Form Blue only for focus rings and the hover/focus outline of inputs, chips and form buttons.
- **Do** set display type in the system serif stack and everything else in the system sans stack.
- **Do** list services and similar choices as hairline rows with an arrow circle, not as cards.
- **Do** join day and night sections with the gold-lined wave seam.
- **Do** keep every tap target at least 44px (buttons 56px, rows 60px).
- **Do** give every animated piece a still frame under `prefers-reduced-motion`, and change motion through `TUNE` rather than inline numbers.

### Don't:
- **Don't** add a sticky bottom bar or any sticky/fixed call-to-action.
- **Don't** show the phone number anywhere on the first screen except the header top-right.
- **Don't** add email links; there is no email address.
- **Don't** link Facebook anywhere but the footer (it is a personal profile).
- **Don't** add captions, eyebrows or kicker labels above headlines.
- **Don't** style anything that isn't clickable as a button or pill.
- **Don't** put more than two buttons together; the hero holds exactly gold + outline.
- **Don't** add web fonts, card shadows, or gold on resting body text.
