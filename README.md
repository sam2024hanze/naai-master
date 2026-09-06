# Naai Master

Landing page for **Naai Master** — kledingreparatie en stomerij aan de Hoofdstraat 46, 9601EH Hoogezand. Ook ophaalpunt van Wasserij & Stomerij Aïnda.

## Live site

Published with GitHub Pages from the `main` branch.

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | The complete page. No build step, no dependencies. |
| `ainda-logo.png` | Aïnda partner logo, used in the marquee and the hero badge. |
| `gmaps-pin.png` | Icon for the floating Google Maps directions button. |

Fonts (Inter and Great Vibes) load from Google Fonts. Everything else is self-contained: the styles are inline, the icons are inline SVG, and the map is a Google Maps embed.

## Sections

- Scrolling partner marquee and sticky navigation
- Hero with call-to-action buttons for WhatsApp and opening hours
- Six service cards covering repairs, zippers, dry cleaning, laundry, ironing, and pickup/delivery
- Opening hours table
- Contact details and an embedded map
- Floating WhatsApp and Google Maps buttons

## Editing

Open `index.html` and edit it directly. The layout uses inline styles, so a change to a section lives in that section's markup. Hover states are the `.hv1`–`.hv8` rules in the second `<style>` block in the head.

Details worth knowing before you edit:

- The marquee text is duplicated in two sibling rows. Change one and you must change the other, or the loop will visibly jump.
- The phone number appears in three places: the "Bellen" button, the contact card, and both WhatsApp links.
- The `<title>` and the description and Open Graph meta tags are in the head.

## Source

Designed in Claude Design and exported to static HTML.
