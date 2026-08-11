---
name: Feel Great — Lina Oueis
description: Independent-distributor site for Unicity's Feel Great System, built on personal trust and calm clarity.
colors:
  deep-trust-navy: "#153862"
  navy-hover: "#1f4879"
  clinical-sky: "#e8f1f9"
  sky-divider: "#c2d4e8"
  neutral-white: "#ffffff"
  muted-label: "#6b7c93"
  muted-disclaimer: "rgb(143, 143, 143)"
typography:
  display:
    fontFamily: "'Segoe UI', Tahoma, Geneva, Verdana, sans-serif"
    fontSize: "3rem"
    fontWeight: 700
    lineHeight: 1.1
  title:
    fontFamily: "'Segoe UI', Tahoma, Geneva, Verdana, sans-serif"
    fontSize: "2rem"
    fontWeight: 700
    lineHeight: 1.2
  subhead:
    fontFamily: "'Segoe UI', Tahoma, Geneva, Verdana, sans-serif"
    fontSize: "1.4rem"
    fontWeight: 400
    lineHeight: 1.3
  body:
    fontFamily: "'Segoe UI', Tahoma, Geneva, Verdana, sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: "25px"
  cta:
    fontFamily: "'Segoe UI', Tahoma, Geneva, Verdana, sans-serif"
    fontSize: "1.2rem"
    fontWeight: 600
    lineHeight: 1
  value:
    fontFamily: "'Segoe UI', Tahoma, Geneva, Verdana, sans-serif"
    fontSize: "1.15rem"
    fontWeight: 500
    lineHeight: 1.2
  label:
    fontFamily: "'Segoe UI', Tahoma, Geneva, Verdana, sans-serif"
    fontSize: "0.8rem"
    fontWeight: 700
    letterSpacing: "0.07em"
rounded:
  pill: "50px"
  card: "22px"
components:
  button-primary:
    backgroundColor: "{colors.deep-trust-navy}"
    textColor: "{colors.neutral-white}"
    typography: "{typography.cta}"
    rounded: "{rounded.pill}"
    padding: "16px 40px"
  button-primary-hover:
    backgroundColor: "{colors.navy-hover}"
    textColor: "{colors.neutral-white}"
    typography: "{typography.cta}"
    rounded: "{rounded.pill}"
    padding: "16px 40px"
  card-contact:
    backgroundColor: "{colors.neutral-white}"
    rounded: "{rounded.card}"
    padding: "70px 80px"
---

# Design System: Feel Great — Lina Oueis

## Overview

**Creative North Star: "The Trusted Consult"**

This is one person's health story handed to a visitor across a table, not a funnel built to convert traffic. The page is long and genuinely information-dense — a personal journey, a two-product protocol, a video explainer, a step-by-step guide — but it stays legible because restraint does the organizing work: one accent color, one type family, alternating full-bleed bands instead of boxes and borders. The system is deliberately quiet where a typical affiliate/MLM landing page would be loud: no countdown timers, no stacked urgency banners, no gradient sales-page gloss. Trust is built through clarity and a real face (Lina's), not pressure.

Confirmed rejection: this must never read as a generic high-pressure landing page, even under the weight of a lot of content to convey. Clear heading hierarchy and color-banding are what keep a long page navigable without resorting to tabs, accordions, or a sidebar.

**Key Characteristics:**
- One accent color (Deep Trust Navy) carries every heading, link, and call to action — no competing hue exists anywhere in the UI.
- Pure system font stack — no webfont import, instant load, deliberately unbranded/clinical voice.
- Flat by default everywhere except one card, where a single soft shadow marks the one moment a visitor commits to personal contact.
- Long-form content is organized by alternating white / pale-sky-blue full-bleed bands rather than borders, cards, or dividers.
- Pill buttons and one circular portrait are the system's only curves in an otherwise rectilinear layout.

## Colors

A two-color system — one navy doing all the trust-and-action work, one pale sky-blue doing all the "breathing room" work — plus near-white neutrals. Restraint, not saturation, is the mechanism.

### Primary
- **Deep Trust Navy** (#153862): every heading, nav link, in-section body copy, button background, and the active-link underline. This single color is effectively the entire brand voice.
- **Navy Hover** (#1f4879): the hover state for navy buttons. Used nowhere else.

### Neutral
- **Neutral White** (#ffffff): navbar background, card backgrounds, button text.
- **Clinical Sky** (#e8f1f9): full-bleed section backgrounds (hero, journey, guide) that segment a long page without needing a border.
- **Sky Divider** (#c2d4e8): hairline borders — the contact card's outline, the footer's top rule.
- **Muted Label** (#6b7c93): the small uppercase field labels on the contact card, the one place the palette speaks below a whisper.
- **Muted Disclaimer** (rgb(143, 143, 143)): reserved for the single line of independent-distributor disclaimer text.

### Named Rules
**The One Voice Rule.** Every UI color is navy, its one hover tint, or a neutral. There is no secondary or tertiary accent. Product-packaging colors that appear inside photography (Unimate's yellow, Balance's orange) are content, not palette — never pull them into chrome, buttons, or UI accents.

## Typography

**Body Font:** 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif
**Display Font:** same family — there is no separate display face; hierarchy is carried entirely by size and weight.

**Character:** Deliberately native and unbranded. The typography doesn't announce itself — it reinforces the "consult, not campaign" feel and keeps the page loading instantly with zero webfont weight.

### Hierarchy
- **Display** (700, 3rem/48px, tightens to 2rem/32px ≤992px, line-height ~1.1): the single hero H1, "Feel Great, Live Better." Used once per page.
- **Title** (700, 2rem/32px, steps to 1.6rem ≤900px and 1.4rem ≤600px): section-level headings — homepage content headings ("About," "My Feel Great Journey," "Unicity Balance – How it Works," "Feel Great Quick Start Guide") and the contact card's "Contact Information."
- **Subhead** (400, 1.4rem/22.4px, drops to 1rem ≤992px): the hero paragraph directly under the Display headline — the only body-family text sized between Title and Body.
- **Body** (400, 1rem/16px, line-height 25px): all other paragraph copy.
- **CTA** (600, 1.2rem/19.2px, steps to 15px ≤992px): the label inside every primary pill button. Distinct from Body because it needs to hold its own against a solid navy background.
- **Value** (500, 1.15rem/18.4px): the contact card's phone/email values — one step down from CTA, paired with the Label role above each value.
- **Label** (700, 0.8rem/12.8px, letter-spacing 0.07em, uppercase): the contact card's field labels only.

### Named Rules
**The No-Pairing Rule.** One font family carries every weight and role on the site. A second typeface would be a decision this system deliberately doesn't make.

**Exception, not a role:** the 1.25rem on `.navbar-toggler` sizes Bootstrap's hamburger icon glyph, not text — it's UI-control sizing, not part of the type ramp, and shouldn't be reconciled against it.

## Layout

Built on Bootstrap 5's grid (`container-fluid`, `col-lg-6` splits), with hand-tuned breakpoints layered on top at 992px, 900–960px, 650px, and 450px — finer-grained than Bootstrap's own steps, because the long-form sections need their own padding choreography as they compress.

The hero splits 50/50 (text | product photo) above 992px and stacks below it. Content sections (journey, guide) run full-bleed edge-to-edge, with internal text padding that scales from 9–10rem on desktop down to 3rem on mobile — the page is designed to be read in wide horizontal bands, not a centered column. The `.about` block and the contact page are the exceptions: they cap width (750px, or a percentage-based center column) because those are single-column reading moments rather than paired story/photo bands.

## Elevation & Depth

Flat by default. Nav, hero, buttons, and every section band carry zero shadow. The one deliberate exception is the contact card (`box-shadow: 0 4px 30px rgba(21, 56, 98, 0.10)`, plus a 1.5px Sky Divider border), floating over a softened, whited-out background photograph.

### Shadow Vocabulary
- **Contact elevation** (`box-shadow: 0 4px 30px rgba(21, 56, 98, 0.10)`): reserved exclusively for the contact card — the one page where a visitor commits to a personal, non-outbound action.

### Named Rules
**The One Shadow Rule.** Exactly one shadow value exists in the system, and it's spent on the contact card. Don't add shadows to buttons, nav, or content bands to "lift" them — flatness is the resting state everywhere else.

## Shapes

Rectilinear by default (image containers, section bands, nav) with two deliberate organic exceptions: pill buttons (50px radius, fixed 270px width) for every call to action, and a circular-cropped portrait (Lina's headshot) floating on a sky-blue disc. The contact card softens the rectangle rather than fully rounding it (22px radius). No other radius scale exists in the system.

## Components

### Buttons
- **Shape:** pill (50px radius / `border-radius: 50px`), fixed 270px width, 16px/40px padding.
- **Primary:** Deep Trust Navy background, white text, 600 weight, 1.2rem (steps to 15px ≤992px). This is the only button variant on the site — every CTA uses it.
- **Hover / Active:** background shifts to Navy Hover (#1f4879) on hover; scales to 0.95 (0.97 on the contact card's variant) on press for tactile feedback.
- **Secondary / Ghost:** none exist. Introducing one would need a deliberate reason — the current system has exactly one visual verb for "take action."

### Cards (Contact)
- **Corner Style:** 22px radius.
- **Background:** Neutral White.
- **Shadow Strategy:** the system's one shadow (see Elevation & Depth).
- **Border:** 1.5px Sky Divider.
- **Internal Padding:** 70px/80px desktop, stepping down to 36px/28px at ≤600px.
- **Internal Rhythm:** centered, stacked label/value pairs, single CTA pill anchoring the bottom.

### Navigation
- White, fixed-top navbar, 80px tall, logo left-aligned.
- Links: Deep Trust Navy, 500 weight, with a centered underline that grows from 0 to full width on hover/active (desktop only, ≥960px).
- Mobile: Bootstrap offcanvas panel sliding from the right; same link styling, underline-grow effect dropped.

### Section Bands (signature component)
- Full-bleed, alternating White / Clinical Sky backgrounds with no borders or shadows between them.
- This is the page's primary wayfinding device: a single long scroll (story, product, video, guide, quote) stays organized through vertical rhythm and color-banding alone, without tabs, accordions, or a sidebar.

## Do's and Don'ts

### Do:
- **Do** keep every call to action the same Deep Trust Navy pill button — one visual verb for "take action," repeated everywhere.
- **Do** preserve the heading hierarchy (Display → Title → Body → Label) and section-band structure as the page's primary navigation aid; a visitor should be able to tell where they are on this long, information-dense page without reading everything.
- **Do** keep the independent-distributor disclaimer visible near the top of the homepage in its current small, muted-gray treatment — it's load-bearing trust language, not filler.
- **Do** reserve the system's one shadow for the contact card; it marks the single moment someone commits to a personal, non-outbound action.

### Don't:
- **Don't** introduce a second accent color, a gradient, a countdown timer, or an urgency banner — the site must not read as a typical high-pressure landing/MLM page, even where there's a lot to say.
- **Don't** pull colors from product-packaging photography (Unimate yellow, Balance orange) into UI chrome, buttons, or backgrounds — they're content, not palette.
- **Don't** add a display webfont or a second typeface; hierarchy is carried by size and weight alone.
- **Don't** add shadows to nav, buttons, or section bands to "lift" them — flat is the resting state everywhere outside the contact card.
