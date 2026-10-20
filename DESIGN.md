---
name: Cleaning Luna LLC
description: A calm, banded one-pager in the logo's night colours; book a cleaning in Elizabeth, NJ with one WhatsApp message.
colors:
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  ink: "#0a2350"
  body: "#26364d"
  soft: "#4a5870"
  navy: "#173d7a"
  deep: "#0a2350"
  on-dark: "#f4f7fb"
  on-dark-soft: "#c9d6ea"
  gold: "#d6a035"
  gold-2: "#e2b452"
  gold-ink: "#7f5a12"
  line: "rgba(10,35,80,.12)"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, min(12.4vw, 15vh), 84px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(19px, 5.2vw, 24px)"
    fontWeight: 400
    lineHeight: 1.2
  action:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.1em"
  caption:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.7
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter: "20px"
  gutter-desktop: "40px"
  stack: "16px"
  block: "36px"
  band: "64px"
  band-desktop: "96px"
  column: "64px"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    typography: "{typography.action}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.gold-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    typography: "{typography.action}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-soft:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 20px"
    height: "48px"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "6px 12px"
    height: "52px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  card-form:
    backgroundColor: "{colors.card}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  service-row:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    padding: "8px 0"
    height: "64px"
  row-arrow:
    backgroundColor: "rgba(255,255,255,.1)"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.circle}"
    size: "44px"
  row-arrow-hover:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
  step-number:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "48px"
  whatsapp-float:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "60px"
---

# Design System: Cleaning Luna LLC

## Overview

**Creative North Star: "The Moonlit Night Shift"**

The whole system is the logo's night: an off-white paper ground, two navies for the bands (a moonlit navy and a midnight with faint diagonal lines), and the crescent moon's gold as the one warm accent. Full-bleed bands alternate light and dark so each section is obvious on a phone, and inside them everything is soft and borderless: pill buttons, a 24px form card, tinted fields. It is the calm band house style, built without photos because the client supplied none.

Density is low and mobile-first. One display face (Cal Sans, always at 400) carries hierarchy by size alone; the system stack sets running text at 16/1.7. Motion is rationed: the hero headline bounces in letter by letter, everything else below the first screen rises 12px once, and nothing is ever hidden at rest, without JS, or under reduced motion.

Gold is precious. It fills the primary button, the step numbers, the service-row arrow on hover and the floating WhatsApp circle, and it colours the last phrase of a dark-band heading. Everywhere else the page is navy on paper or pale blue on navy.

**Key Characteristics:**
- Paper, navy and midnight bands, full-bleed, alternating light and dark.
- Gold as a fill with navy text on it; a darker gold-ink when gold must be text on light.
- Cal Sans at one weight for headings, rows, buttons and labels; system stack for body.
- Soft geometry: 24px card, 10px fields, full pills, circles for icons and counters.
- Flat surfaces; the floating WhatsApp circle is the only thing that casts a shadow.
- One letter bounce-in (hero H1 only) and one 12px fade-up.

## Colors

A cool, low-saturation night palette with a single warm metallic accent taken from the logo's moon.

### Primary
- **Moon Gold** (gold): the one accent, used as a fill only: primary buttons, numbered step discs, the hovered or focused service-row arrow, the floating WhatsApp circle, text selection, focus rings on dark bands, and the accent phrase in dark-band headings (heading sizes only; it sits at 4.5:1 on navy).
- **Lit Gold** (gold-2): the primary button's hover fill. Nothing else.
- **Old Brass** (gold-ink): gold as text or icon on light grounds (5.8:1 on paper): the header phone icon and its hover, the care-claim icons.

### Secondary
- **Moonlit Navy** (navy): the hero and the content bands for services and the close; also the input caret and the focus/hover outline on light grounds.
- **Midnight** (deep): the How-it-works band and the footer, always with the diagonal line texture.

### Neutral
- **Night Paper** (paper): the page ground, header and light bands. Never replaced by black or pure white.
- **Card White** (card): the quote form card only.
- **Frost Field** (field): input, chip and soft-button fill on the white card, and the composed-message panel.
- **Midnight Ink** (ink): headings and labels on light, and all text on gold. Same value as Midnight, different role.
- **Slate Body** (body): running text on light.
- **Slate Soft** (soft): ledes, secondary text, placeholders, small print.
- **Moonlight** (on-dark): headings, rows and links on navy and midnight.
- **Moonlight Soft** (on-dark-soft): running text and ledes on dark bands.
- **Hairline** (line): 1px dividers between list items on paper; on dark bands the divider is `rgba(255,255,255,.12)`.
- **Signal Red** (error): inline error sentences and the error border on a field.

### Named Rules
**The Fill-Only Gold Rule.** Gold is a fill, and text on a gold fill is Midnight Ink. Gold never sets text on paper or white; use Old Brass there. Gold text on a dark band is limited to heading-size accent phrases.

**The Night Bands Rule.** Sections are full-bleed bands in paper, navy or midnight, alternating light and dark. The ground is never black. The diagonal line texture belongs to the hero and to midnight bands, never to a plain navy content band.

**The Faint Lines Rule.** The texture is `repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`. Never stronger than about 4% white, so it never reads as lines through text.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui, sans-serif)
**Body Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif)

**Character:** A friendly geometric display face with tight leading over a plain, roomy system body. Cal Sans speaks for the brand (headings, service names, buttons, field labels, phone numbers); the system stack just reads.

### Hierarchy
- **Display** (400, clamp 40-84px tied to viewport width and height, 1.02): the hero H1 only, max 11-12ch, white with the gold accent phrase.
- **Headline** (400, clamp 30-48px, 1.08): section H2s, balanced wrapping.
- **Title** (400, 19-24px fluid, 1.15-1.2): service rows, care claims, step titles (21-22px), field labels and legends (18px).
- **Action** (400, 18px, 1): buttons and the header phone number (20px on desktop).
- **Lede** (400, clamp 17-19px, 1.7): the paragraph under an H2, max 38ch. The hero promise is a variant at 17-20px / 1.5, max 30-36ch.
- **Body** (400, 16px, 1.7): running text; inputs are also 16px so iOS does not zoom.
- **Label** (600, 14px, 0.1em, uppercase): service group headings on navy (Homes, Rentals & businesses, Job sites). The wordmark's "LLC · Elizabeth, NJ" line is the same treatment at 12px.
- **Caption** (400, 14px): the "(optional)" field hint and the note under the submit button.

### Named Rules
**The One Weight Rule.** Cal Sans is set at 400 everywhere. Hierarchy comes from size and colour, never from a heavier weight.

**The Display Voice Rule.** Anything the visitor taps or reads as a name (buttons, service rows, phone numbers, field labels) is in Cal Sans; sentences are in the system stack.

## Layout

A single 1160px max-width column with a 20px phone gutter that becomes 40px at 760px. Bands are padded 64px top and bottom on phones and 96px from 760px. Inside a band, a heading block stacks with 16px gaps (max 640px), and lists sit 28-36px below it.

Phones are one column throughout. At 760px the hero buttons sit side by side (min 240px each). At 1024px: the care section splits into two equal columns with a 64px gap, service groups go two-up (the first group spans two rows), the three steps sit in a row with 40px gaps, the form section goes 1 : 1.3 with a sticky heading, and the close band puts the big phone number at the bottom right. The hero's gold crescent is a 72px mark in the top corner on phones and grows to 300-380px at the right on desktop, always clear of the text.

Short landscape screens (max-height 500px) shrink the hero padding and size the H1 at 12vh. Safe-area insets pad the header top, the footer bottom and the floating circle. Tap targets are 44px or larger everywhere.

## Elevation & Depth

Flat. Depth comes from band colour (paper, navy, midnight) and from the white form card sitting on paper, not from shadows. The single exception is the floating WhatsApp circle, which genuinely floats over content.

### Shadow Vocabulary
- **Float** (`box-shadow: 0 10px 28px rgba(6,20,46,.3)`): the floating WhatsApp circle only.

### Named Rules
**The One Shadow Rule.** Only the element that floats over the page casts a shadow. Cards, buttons, rows and fields stay flat; their states change fill, border or outline instead.

## Shapes

Soft and borderless. Containers round at 24px (the form card), fields at 10px, and every button and chip is a full pill. Small icon carriers are circles: the 44px service-row arrow, the 48px step discs, the 60px floating circle. Fields and chips carry a 2px transparent border so a state colour can appear without shifting layout. Lists are divided by 1px hairlines rather than boxed. Icons are inline stroked SVG (about 2.2-2.6 stroke), drawn in currentColor.

## Components

### Buttons
Round, warm and unmistakable.
- **Shape:** full pill (999px), 56px tall, 26px side padding, 2px border, Cal Sans 18px, optional 22px leading icon.
- **Primary:** Moon Gold fill and border, Midnight Ink text. Hover (pointer devices only) shifts to Lit Gold. On the form card, hover and focus add a 2px navy outline offset 2px.
- **Ghost:** transparent with a 70% Moonlight border and Moonlight text, used only beside a primary on a dark band. Hover makes the border solid white over a 10% white wash.
- **Soft:** Frost Field fill, Midnight Ink text, 48px tall, 16px text; the fallback actions after the form sends.
- **Press:** every button scales to 0.98 on press.

### Chips
- **Style:** Frost Field pill, 52px tall, centred 16px system text in Midnight Ink, laid out in an auto-fill grid (min 136px) with 10px gaps. The checkbox is visually hidden; the label is the chip.
- **State:** hover draws a navy border; selected fills Midnight Ink with white text; focus adds a 3px navy outline offset 2px; selected-and-hovered uses an offset outline because a border would vanish on the ink fill. Error turns the border Signal Red.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** Card White on a paper band.
- **Shadow Strategy:** none (see The One Shadow Rule).
- **Border:** none.
- **Internal Padding:** fluid 20-32px, 22px between fields.

### Inputs / Fields
- **Style:** Frost Field fill, 10px radius, 2px transparent border, 16px text, 52px tall (textarea 110px, vertical resize), Slate Soft placeholder, navy caret. Labels sit above in Cal Sans 18px; optional hints follow in 14px Slate Soft.
- **Focus / Hover:** the border turns Moonlit Navy; no glow.
- **Error:** the border turns Signal Red and stays red even while focused; a plain-sentence error appears under the field in red.

### Navigation
A slim paper header: the moon mark (40px, 48px on desktop) and the Cal Sans wordmark with its small uppercase locality line on the left, the tap-to-call number in Cal Sans with an Old Brass phone icon on the right. Below 375px the locality line drops; below 340px the icon drops. The footer is a midnight band with the line texture, Moonlight links at 44px tap height that turn gold on hover.

### Service Rows
Each row on the navy band is a whole link: Cal Sans service name at 19-22px, 64px tall, hairline dividers, and a 44px translucent-white arrow circle at the right. On hover or focus only the arrow changes: it fills gold with ink arrow (focus adds a gold outline to the arrow). Tapping a row jumps to the form with that service's chip already selected.

### Numbered Steps
Three steps on midnight, each led by a 48px gold disc holding a Cal Sans counter in ink, a Moonlight title (21-22px) and a Moonlight Soft line. One column on phones, three across from 1024px.

### Eyebrow Pill
Ellie's house choice (calm band style, 2026-10-19), kept even though Impeccable's craft floor bans eyebrows. A quiet label above the hero H1 and at most one or two section headings (here: "Homes, businesses & job sites", "Big job or small"). It's a `<p>`, never a heading: 14px/500 system text, 9px 14px padding, pill radius, a 7px gold dot before the text. On light it's ink on rgba(10,35,80,.06); on navy it's Moonlight on rgba(255,255,255,.12). No arrow, no hover, no shadow, never a full gold fill, so it can't read as a button.

### Floating WhatsApp Circle
A 60px gold circle with a 28px ink WhatsApp glyph, fixed 16px from the bottom-right (plus safe area), carrying the Float shadow. It slides in from 120px below once the hero has scrolled away (0.35s, cubic-bezier(.2,.8,.2,1)) and steps aside while the form or the closing WhatsApp link is on screen; while hidden it is untabbable and aria-hidden. Its focus ring is a 3px ink outline with a white halo. Removed entirely without IntersectionObserver or in print.

### Hero Headline Bounce-in
The hero H1 is split into letters by JS; each slides in from 50px right with opacity, over 1s on cubic-bezier(.34,1.56,.64,1), staggered 20ms per letter, words kept unbreakable. When the last letter lands, the original heading markup is restored. Skipped under reduced motion and without JS.

### Fade-up
Elements that start below the first screen rise 12px and fade in over 0.4s ease-out as they enter. Everything above the fold, without JS, in print, and under reduced motion is simply visible.

## Do's and Don'ts

### Do:
- **Do** put Midnight Ink on every gold fill, and use Old Brass (#7f5a12) when gold has to be text or an icon on light.
- **Do** alternate full-bleed paper, navy and midnight bands, and put the 135deg line texture only on the hero and midnight bands, at about 4% white or fainter.
- **Do** set every Cal Sans element at weight 400 and carry hierarchy with the clamp()ed sizes.
- **Do** keep fields and chips on Frost Field (#e6ecf5) inside the white card, with a 2px border that turns navy on hover and focus and red on error.
- **Do** gate hover styles behind `(hover:hover)` so taps never leave a stuck state.
- **Do** keep every tap target at 44px or larger and every input at 16px or larger.
- **Do** keep content visible at rest; motion only ever reveals something that is already there for no-JS and reduced-motion visitors.

### Don't:
- **Don't** set text in gold on paper or white, or white text on gold.
- **Don't** use a black ground or a pure-white page ground; white is for the form card only.
- **Don't** give the bounce-in letter animation to any heading other than the hero H1, or add a second kind of scroll animation.
- **Don't** add shadows to cards, buttons or rows; the floating circle is the only shadow.
- **Don't** change anything but the arrow when a service row is hovered or focused.
- **Don't** turn the floating circle into a bottom bar, or show it while the form or the closing WhatsApp link is in view.
- **Don't** add a heavier Cal Sans weight or a second body font.
