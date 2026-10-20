---
version: alpha
name: "Mother Knows Best — Retail & Styling Edition"
description: "Bright, warm, retail-editorial styling and conscious capsule OS for mothers aged 25-45. Built on the official Mother Knows Best Wicklow (motherknowsbest.ie) colour system."
colors:
  primary: "#C82D08"
  secondary: "#1F2022"
  tertiary: "#006948"
  neutral: "#F9F8F4"
  surface: "#FFFFFF"
  surface-warm: "#F2EFE9"
  ink: "#1E1E20"
  ink-muted: "#575559"
  mkb-pink: "#FBCFFA"
  mkb-light-pink: "#FEEAFD"
  sage-tint: "#E6F4EE"
typography:
  h1:
    fontFamily: Newsreader
    fontSize: 2.75rem
    fontWeight: 500
    lineHeight: 1.08
    letterSpacing: "-0.02em"
  h2:
    fontFamily: Newsreader
    fontSize: 1.85rem
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.015em"
  h3:
    fontFamily: Plus Jakarta Sans
    fontSize: 1.12rem
    fontWeight: 600
    lineHeight: 1.28
  body-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 0.95rem
    fontWeight: 400
    lineHeight: 1.55
  label-mono:
    fontFamily: JetBrains Mono
    fontSize: 0.72rem
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "0.06em"
rounded:
  sm: 10px
  md: 16px
  lg: 24px
  xl: 9999px
spacing:
  sm: 8px
  md: 16px
  lg: 24px
  xl: 36px
components:
  page-canvas:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.ink}"
    padding: "{spacing.lg}"
  button-primary:
    backgroundColor: "{colors.secondary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.xl}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
  button-accent:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.xl}"
    padding: "{spacing.md}"
  button-secondary:
    backgroundColor: "{colors.surface-warm}"
    textColor: "{colors.ink}"
    rounded: "{rounded.xl}"
    padding: "{spacing.sm}"
  card-retail:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
  badge-mkb-pink:
    backgroundColor: "{colors.mkb-light-pink}"
    textColor: "{colors.ink}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  badge-mkb-pill:
    backgroundColor: "{colors.mkb-pink}"
    textColor: "{colors.ink}"
    rounded: "{rounded.xl}"
    padding: "{spacing.sm}"
  badge-jev-verified:
    backgroundColor: "{colors.sage-tint}"
    textColor: "{colors.tertiary}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  caption-muted:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink-muted}"
    typography: "{typography.body-md}"
---

## Overview

**Mother Knows Best — The Conscious Style Edit (`motherknowsbest.ie`)** is a bright, high-trust retail-editorial styling experience for mothers aged 25–45. It adopts the exact visual identity of the **Mother Knows Best Wicklow** community (`motherknowsbest.ie`):
- **Warm Alabaster Linen (`#F9F8F4`)** and **Pure Editorial White (`#FFFFFF`)** canvases
- **MKB Vermilion Red-Orange (`#C82D08` / `#E83A0F`)** for italic serif emphasis and high-energy retail callouts
- **MKB Soft Orchid Pink (`#FBCFFA` & `#FEEAFD`)** for supportive community badges, interview highlights, and ampersand flourishes
- **Deep Charcoal Pill CTAs (`#1F2022`)** and **Coastal Greystones Sage (`#006948`)** for verified TypeSafe AI `Jev` (`typesafe/jev-latest`) confidence scores and Cost-Per-Wear savings.

## Colors

- **Primary (`#C82D08` - MKB Vermilion Red-Orange):** Signature Mother Knows Best editorial accent (WCAG-AA verified `5.51:1` on white) used for italic headline highlights (*"warmer"*, *"flattering"*), active step indicators, and priority retail gap tags.
- **Secondary (`#1F2022` - MKB Deep Charcoal):** Used for signature pill-shaped primary CTAs (`Join the community`, `Unlock My Smart Edit →`), giving a crisp Sézane / Arket retail polish.
- **Tertiary (`#006948` - Greystones Coastal Sage):** Used for TypeSafe AI `Jev` calibrated confidence scores, Cost-Per-Wear badges, and verified silhouette match scores.
- **MKB Pink (`#FBCFFA` & `#FEEAFD`):** Signature Mother Knows Best pastel pink wash used for interview chat bubbles, supportive postpartum comfort callouts, and community tags.
- **Neutral (`#F9F8F4` - Warm Alabaster):** Bright, sunlit paper background that lets retail fashion photography shine.

## Typography

- **Display & Retail Lookbook Headlines (`Newsreader`):** High-contrast editorial serif with expressive italic alternates (`font-style: italic; color: #E83A0F`) matching the `"Mothering, made a little warmer together"` hero on `motherknowsbest.ie`.
- **UI & Retail Product Cards (`Plus Jakarta Sans`):** Clean, modern retail sans-serif for effortless scanning.
- **Jev Decision Telemetry & Cost-Per-Wear (`JetBrains Mono`):** Reserved strictly for calibrated `Jev` probabilities, Cost-Per-Wear (`€0.54/wear`), and hex swatches.

## Layout

- **Retail-Editorial Lookbook Layout:** High-resolution fashion photography throughout every section, paired with a clean 4-step user journey that accelerates directly from **1. Personal Circumstances** → **2. Interactive Stylist + Jev Interview** → **3. Computer Vision Wardrobe Snap** → **4. Hero Feature: The Conscious Capsule & Smart Shop**.
- Demo persona switcher is tucked cleanly into a discrete `"Demo Mode"` pill in the utility bar so real users always start by self-identifying their own motherhood stage.

## Elevation & Depth

- **Level 0 (`#F9F8F4`):** Warm Alabaster page canvas.
- **Level 1 (`#FFFFFF`):** Crisp white retail product cards with `1px solid #EAE5DD` border and soft editorial lift shadow.
- **Level 2 (`#FEEAFD` & `#E6F4EE`):** MKB Orchid Pink and Coastal Sage callout surfaces.

## Shapes

- Signature Mother Knows Best **full-pill buttons (`9999px`)**, `24px` retail lookbook image cards, and `10px` telemetry tags.

## Components

- `button-primary` (`#1F2022` pill) and `button-accent` (`#C82D08` pill) drive the accelerated funnel into the Conscious Shop Hero.
- `badge-jev-verified` displays the calibrated TypeSafe AI `Jev` (`typesafe/jev-latest`) decision output (Silhouette Flatter Score `1–5`, Regret Risk `%`, and Calibrated Purchase Confidence `%`).

## Do's and Don'ts

- **Do** start by letting the user self-identify her current life stage (On Maternity Leave, Working Mum Office/Hybrid, Stay-at-Home / Full-Time Mum, Return-to-Work Transition, or Expecting / 4th Trimester).
- **Do** use real, bright editorial photography across every card and accelerate the user straight to the **Conscious Capsule & Smart Shop Hero**.
- **Do** weave in `motherknowsbest.ie` community touchpoints (Greystones/Wicklow Mum Style Swap, Book Club outfit picks, and WhatsApp community styling tips).
- **Don't** clutter the UI with dark developer telemetry or show demo personas as the primary user identity.
