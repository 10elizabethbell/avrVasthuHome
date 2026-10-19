---
name: AVR Vasthu Home 2D Plan
description: The drafting table. A Vastu house plan drafted live on blueprint, with paper-cream sections for reading.
colors:
  ink: "#11304f"
  ink-line: "#cfe2f6"
  ink-soft: "#a9c6e4"
  wall: "#e4efff"
  marigold: "#f2a516"
  marigold-hi: "#ffb72e"
  marigold-deep: "#c77f00"
  numeral: "#a86a00"
  focus: "#2f78d0"
  paper: "#f6f1e6"
  paper-2: "#ede5d4"
  field: "#fffdf8"
  field-line: "#8f846e"
  rule: "#d6ccb8"
  text: "#1a2a3b"
  muted: "#4b5a6a"
  placeholder: "#756e60"
  error: "#a3261b"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "clamp(40px, 12.4vw, 84px)"
    fontWeight: 850
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "clamp(30px, 8vw, 52px)"
    fontWeight: 850
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "20px"
    fontWeight: 850
    lineHeight: 1.15
  lead:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "clamp(19px, 5vw, 24px)"
    fontWeight: 500
    lineHeight: 1.45
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "17px"
    fontWeight: 750
    lineHeight: 1.25
  price:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "22px"
    fontWeight: 850
    lineHeight: 1.1
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, Noto Sans Tamil, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1.5
rounded:
  field: "10px"
  button: "12px"
  panel: "14px"
  full: "50%"
spacing:
  pad-phone: "20px"
  pad-desktop: "32px"
  section-phone: "56px"
  section-desktop: "88px"
  stack: "26px"
  gap: "10px"
components:
  button-primary:
    backgroundColor: "{colors.marigold}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.button}"
    padding: "0 18px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.marigold-hi}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "#ffffff"
    typography: "{typography.label}"
    rounded: "{rounded.button}"
    padding: "0 18px"
    height: "56px"
  input-text:
    backgroundColor: "{colors.field}"
    textColor: "{colors.text}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "0 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.text}"
    rounded: "{rounded.field}"
    padding: "0 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "#ffffff"
  price-row-arrow:
    backgroundColor: "transparent"
    textColor: "{colors.text}"
    rounded: "{rounded.full}"
    size: "34px"
  price-row-arrow-hover:
    backgroundColor: "{colors.marigold}"
  plot-preview:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.ink-line}"
    rounded: "{rounded.panel}"
---

# Design System: AVR Vasthu Home 2D Plan

## Overview

**The drafting table.** The site is a sheet of drawing work: blueprint navy at the top and bottom (header, hero, footer), drafting paper in between for reading the prices, the process and the form. On the blueprint a Vastu house plan drafts itself wall by wall with a marigold pen tip; the visitor can take the pen and draw grid-snapped walls with live feet-and-inches dimensions, and a compass needle swings toward the finger and springs back to north. Dimension lines (end ticks plus a run) divide the paper sections and draw in on scroll. The form ends in a live SVG plot preview drawn to scale on a small blueprint panel.

Everything visual is drawn in line, not filled in: walls, ticks, rules, arrows, compass. Type is the system font stack at heavy weight and uppercase for display, which is the owner's deliberate house style, not a gap to fill with a webfont. One page, phone first.

**The Drawn Not Decorated Rule.** Every ornament on the page is a drafting device the world owns (grid, wall, dimension line, compass, door swing, scale preview). Anything that is not something a draftsman would put on a sheet does not belong.

**The North Returns Rule.** Motion is physical and settles home: the compass is a damped spring back to north, the pen moves at a constant drafting speed, dividers draw in once and stay. Nothing loops for attention except the self-drafting plan, which holds its finished state before redrawing.

## Colors

Two grounds, one pen, one form signal.

### Primary
- **Blueprint Ink** (ink): the ground of header, hero, footer, the plot preview and selected chips. Also the knockout behind dimension labels on canvas, so labels sit on clean ground over grid lines.
- **Drafted Line** (ink-line): grid lines (at 5.5% and 13% alpha for minor and major), dimension label text, compass ring and N.
- **Blueprint Secondary** (ink-soft): secondary text on blueprint (promise line, brand subtitle, hint, footer tag and fine print), dashed dimension leaders, room sub-labels.
- **Wall White** (wall): the drafted walls and fittings on the canvas and the plot outline in the preview. Brighter than ink-line so built walls read above their annotations.

### Secondary
- **Marigold** (marigold): the pen. The pen tip and its halo, walls the visitor draws and their live dimensions, the compass north needle, the POOJA room label, the hero emphasis word, the primary button fill and ghost button border, the brand mark outline, the phone icon, the price-row arrow on hover, selection highlight, and focus rings on blueprint.
- **Marigold Bright** (marigold-hi): primary button hover only.
- **Marigold Deep** (marigold-deep): marigold on paper where the bright tone would be too weak, e.g. the north needle of the form compass hub.
- **Step Numeral** (numeral): the large step counters in "how we work". Marigold darkened enough to stand as text on paper.

### Tertiary
- **Form Blue** (focus): the form's interaction signal on paper: input and chip hover borders, focus border with a 3px translucent ring, focus-visible outlines, and the send button's hover border. Deliberately different from the marigold button fill, so "you are here in the form" never reads as "this is the action".

### Neutral
- **Drafting Paper** (paper): reading sections. **Paper Shade** (paper-2): the form section, one step darker to mark it as the working sheet.
- **Field** (field) with **Field Line** (field-line): inputs, chips, the composed-message panel.
- **Paper Rule** (rule): dimension-line dividers, price-row rules, the arrow ring, the service-area rule.
- **Text** (text), **Muted** (muted), **Placeholder** (placeholder), **Error** (error).

**The One Pen Rule.** Marigold is the only warm accent and it always means the pen or the primary action. Never use it for decoration or as a section background.

**The Blue Belongs To The Form Rule.** Form Blue appears only on paper, only on form interaction states. On blueprint, focus rings switch to marigold.

## Typography

**Display / Headline / Title:** the system font stack (with Noto Sans Tamil in the chain), 850 weight, uppercase, tight -0.01em tracking, 1.02 leading, balanced wrapping. The hero headline caps at roughly 9 characters per line; the footer name repeats the display treatment at a smaller clamp (28-48px).

**Body:** the same stack at 17px / 1.55, regular. Lead paragraphs (the care statement) step up to 19-24px at weight 500.

**Labels and names:** 750 weight, sentence case, for buttons, form legends and service names. Uppercase is reserved for headings, the brand name and the service-area label.

**Numerals:** every price, phone number and step counter uses tabular figures. Prices sit at 850 weight with a smaller "Rs" (0.68em, 600 weight) before them.

**The One Family Rule.** One system stack carries everything; hierarchy comes from weight (400, 500, 600, 750, 850) and case, never from a second typeface.

**The Heavy Caps Rule.** Display is always uppercase at 850. Never set a heading in light or regular weight, and never set body copy in caps.

## Layout

Single column on phones with a 20px side margin (32px from 720px). Content max width 1160px. Sections breathe at 56px vertical padding on phones and 88px on desktop; each paper section opens with a full-width dimension-line divider.

- **Phone (base):** hero copy, then two equal buttons side by side, then the plan canvas bleeding to the screen edges directly under the buttons. The canvas fades in from the top edge with a 26px mask.
- **720px:** steps go to three columns; the numeral moves above its heading.
- **1024px:** hero splits into copy (bottom-aligned) and plan (about 1 : 1.05); the canvas is masked on both sides as well as the top so it dissolves into the ground. Prices and the form use a 1 : 1.6 two-column split with the heading (and plot preview) sticky on the left. The footer splits into name and numbers.

Forms stack at 26px between fields and cap at 640px. Interactive targets are at least 44px tall; buttons 56px, inputs 52px, chips 46px.

**The Plan Under The Buttons Rule.** On phones the drawing sits directly below the calls to action in the first viewport, never pushed below the fold by extra copy.

## Elevation & Depth

Flat. Depth comes from ground change (blueprint against paper, paper against paper-shade) and from line weight, not shadows. The only box-shadows are the 3px Form Blue focus rings. On the canvas, a dimension label sits on a rectangle of blueprint ink so it reads above the grid, the way a draftsman breaks a line for a figure.

**The Flat Sheet Rule.** Nothing floats. No drop shadows on cards, buttons or panels; separation is a rule line or a change of ground.

## Shapes

Gently rounded rectangles: 10px on inputs, chips and the copy button; 12px on buttons; 14px on the plot preview and message panel. The only circle is the price-row arrow ring. Lines are 1.5px throughout on paper (rules, field borders, dividers, arrow ring); canvas walls scale with the grid (minimum 3px) and annotations stay at 1.2px.

**The Line Weight Rule.** Paper uses one line weight (1.5px). Blueprint uses two: heavy walls and hairline annotations.

## Components

**Buttons.** Primary is a marigold fill with ink text, 2px marigold border, 56px tall, 750 weight; hover brightens to marigold-hi, press nudges down 1px. Ghost (on blueprint only) keeps the marigold border with white text and a 12% marigold wash on hover. The form's send button is the primary button full-width (max 360px) with a Form Blue border on hover.

**Price rows.** The whole row is one link: service name (750, with an optional muted note under it), price on the right, and a circled arrow. Rows are separated by paper rules. Only the arrow reacts: it fills marigold on hover and carries the focus ring on keyboard focus. The row itself does not change background.

**Dimension-line divider.** A full-width SVG: two end ticks and a run between them in paper-rule color. When it enters view the run draws from left to right (1.4s, ease-out-expo) and the ticks fade in after 0.9s. With reduced motion it is simply drawn.

**Drafting canvas (hero).** A 1-ft grid on blueprint; a Vastu plan (pooja north-east, kitchen south-east, master bedroom south-west) drafted wall by wall by a marigold pen tip with a soft halo, then rooms labeled, then overall dimensions. Touch takes the pen: drags snap to the 1-ft grid along the dominant axis and show live feet-and-inches in marigold; user walls fade after a few seconds and the pen resumes. A compass sits top-right of the plan; its needle swings toward a nearby finger and springs back to north. A one-line hint sits centered at the bottom and fades after first touch.

**Inputs.** Field-cream fill, 1.5px field-line border, 10px radius, 52px tall. Hover and focus switch the border to Form Blue; focus adds a 3px translucent blue ring. Plot size is two inputs with a muted × and "ft" between.

**Chips.** Radio and checkbox choices as 46px field-cream chips; selected fills with blueprint ink and white text. The facing-direction choice is a 3 × 3 compass grid (N, E, S, W around a small compass hub).

**Plot preview.** A small blueprint panel that redraws the plot to scale as the visitor types: faint grid, the plot outline in wall white (dashed and faint until both sizes are entered), a marigold road band on the chosen facing side with ink lettering, and a marigold north arrow.

**Errors.** Inline text under the field, error red at 15px / 600, shown only after a send attempt.

## Do's and Don'ts

- Do draw with the world's own devices: grid, walls, dimension lines with end ticks, compass, door swings, scale drawings.
- Do keep marigold for the pen and the primary action, and Form Blue for form interaction on paper.
- Do keep prices verbatim with a small "Rs" and tabular figures.
- Do keep every touch target at 44px or more and every animated drawing readable as a finished drawing under reduced motion.
- Don't introduce a webfont or a second typeface; the system stack at heavy caps is the house style.
- Don't add shadows, gradients-as-fills or glass panels; the sheet is flat.
- Don't add small uppercase labels above headings, or decorative icons beside headings and list items.
- Don't use marigold as a large fill area or put Form Blue on blueprint.
