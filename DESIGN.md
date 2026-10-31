---
name: CARDROOM
description: Compact Korean TCG storefront with vivid manga campaigns
colors:
  primary: "#ed3234"
  manga-red: "#ec3034"
  manga-deep: "#aa1726"
  campaign-yellow: "#ffe344"
  pokemon-yellow: "#ffdf39"
  pokemon-blue: "#214e9c"
  series-blue: "#0e55c0"
  series-dark: "#232434"
  ink: "#17191e"
  white: "#fff"
  secondary-text: "#777"
  border: "#ddd"
  product-surface: "#f5f5f7"
  section-surface: "#f5f6f8"
  focus: "#2367dc"
typography:
  display:
    fontFamily: "Pretendard, sans-serif"
    fontSize: "43px"
    fontWeight: 900
    lineHeight: 1.18
    letterSpacing: "-.035em"
  headline:
    fontFamily: "Pretendard, sans-serif"
    fontSize: "25px"
    fontWeight: 800
    letterSpacing: "-.03em"
  product-title:
    fontFamily: "Pretendard, sans-serif"
    fontSize: "13px"
    fontWeight: 650
    lineHeight: 1.4
  body:
    fontFamily: "Pretendard, sans-serif"
    fontSize: "14px"
  price:
    fontFamily: "Pretendard, sans-serif"
    fontSize: "16px"
    fontWeight: 800
    letterSpacing: "-.02em"
rounded:
  square: "0px"
  campaign-button: "2px"
  quick-add: "3px"
  search: "5px"
  circle: "50%"
spacing:
  icon-gap: "8px"
  promo-gap: "16px"
  grid-gap: "20px"
  section-pad: "36px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.white}"
    rounded: "{rounded.square}"
    padding: "15px 18px"
    width: "100%"
  button-campaign:
    backgroundColor: "{colors.white}"
    textColor: "#191b24"
    rounded: "{rounded.campaign-button}"
    padding: "10px 13px"
  search:
    rounded: "{rounded.search}"
    padding: "0 13px"
  product-image:
    backgroundColor: "{colors.product-surface}"
    height: "224px"
---

# Design System: CARDROOM

## Overview

CARDROOM is a compact Korean card shop: familiar commerce structure, crisp white surfaces, bold Korean typography, and collectible artwork. Its visual energy comes from a red manga campaign and a bright yellow Pokémon promotion, followed by an efficient product grid.

The user rejected muted, generic AI-looking styling and requested graphics and flashy elements. Preserve that expressive campaign direction while keeping product information easy to scan.

## Colors

Red marks the logo, search outline, selected filters, basket counts, and primary action. Campaign red and yellow carry the strongest graphic emphasis. Pokémon blue and the darker series panel provide franchise-specific contrast. White, pale product wells, subtle gray dividers, and dark ink keep the shopping area clear.

## Typography

Use the bundled variable Pretendard font throughout. Hero text is 43px/900 on desktop, 36px below 1100px, and 31px below 760px. Section headings are 25px/800; product names 13px/650; prices 16px/800. Metadata and utility copy intentionally stay compact at 8–12px. Avoid turning every element into display typography.

## Layout

The centered wrapper is at most 1240px wide, with 40px desktop side gutters. At 1100px gutters become 24px, and at 760px become 16px. The desktop campaign uses a flexible main banner plus a 300px side column with a 16px gap. Product grids use six columns, then three below 1100px, and two below 760px. Series panels use two columns and stack on mobile. The header wraps the search onto its own mobile row; the main campaign stacks above the yellow promotion. Section spacing is compact, generally 25–50px vertically.

## Elevation & Depth

Commerce surfaces are flat and separated with thin borders or background tone. The hero uses artwork overlaps, oversized rotated OP09 lettering, a conic speed-line background, and a tilted outlined yellow label. Hero text alone has a hard `0 2px 0 #aa1621` shadow. The basket drawer uses a translucent `#171b2566` backdrop; the toast floats above it. Do not add diffuse card shadows.

## Shapes

Promotional panels, product wells, and series tiles have square corners. Search and toast use 5px radii; small campaign actions use 2px, quick-add 3px. Circular shapes belong to quick categories, saved counts, heart controls, and the Pokémon arrow. Preserve the tilted comic sticker and large cropped franchise graphics.

## Components

- **Campaign:** Official Luffy art overlaps the red manga background; the yellow Pokémon panel uses official Pikachu art and a darker yellow ring. Copy sits above artwork and stays legible.
- **Search:** A 2px red outline surrounds a 43px-high input; mobile input height is 38px. Popular search terms sit immediately below.
- **Product:** A flat pale image well, condition badge, circular heart, and small quick-add control precede tight metadata, title, code, and bold price. Artwork scales to 1.035 on hover over 0.2 seconds; quick-add turns yellow, and saved hearts turn red.
- **Tabs and navigation:** Selected state uses red text; tabs add a 2px red underline. Desktop navigation is 14px/700 and mobile 11px.
- **Actions:** The drawer primary action is full-width red with white copy. The hero action is a compact white rectangle with a trailing arrow.
- **Guide:** Fine dividers separate disclosure rows; opening a row rotates its plus icon 45 degrees.
- **Focus and motion:** Interactive elements have a 3px blue focus outline with 4px offset. Respect the existing reduced-motion rule, which disables transitions and smooth scrolling.

## Do's and Don'ts

- **Do** make campaign art vivid, recognizable, and deliberately cropped.
- **Do** preserve the white, dense Korean storefront and six/three/two-column product rhythm.
- **Do** use red for shopping emphasis and selection, with franchise colors in promotional areas.
- **Don't** replace the campaign with muted gradients, abstract blobs, or generic decorative cards.
- **Don't** round every panel or add floating shadows to the product grid.
- **Don't** let oversized art obscure campaign text or shopping controls.
