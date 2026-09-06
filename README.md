# Naai Master

Landing page for **Naai Master** — kledingreparatie en stomerij aan de Hoofdstraat 46, 9601EH Hoogezand. Ook ophaalpunt van Wasserij & Stomerij Aïnda.

Hosted on Vercel. The page is plain static HTML with no build step and no JavaScript.

## Contents

| File | Purpose |
| --- | --- |
| `index.html` | The complete page. |
| `naai-logo.png` | Naai Master badge, used in the header, the footer, and as the favicon. |
| `ainda-logo.png` | Aïnda partner logo, used in the marquee and the hero badge. |
| `gmaps-pin.png` | Icon for the floating Google Maps directions button. |
| `svc-reparatie.webp` | Photo for the Kledingreparatie card. |
| `svc-stomerij.webp` | Photo for the Stomerij card. |
| `svc-haalbreng.webp` | Photo for the Haal- en breng service card. |
| `vercel.json` | Cache headers for the images plus two security headers. |

Fonts (Inter and Great Vibes) load from Google Fonts. Everything else is self-contained: the styles are inline, the icons are inline SVG, and the map is a Google Maps embed.

## Sections

- Scrolling partner marquee and sticky navigation
- Hero with call-to-action buttons for WhatsApp and opening hours
- Three photo cards: Kledingreparatie, Stomerij, Haal- en breng service
- Opening hours table
- Contact details and an embedded map
- Floating WhatsApp and Google Maps buttons

## Editing

Open `index.html` and edit it directly. The layout uses inline styles, so a change to a section lives in that section's markup. Hover states are the `.hv1`–`.hv7` rules in the second `<style>` block in the head.

Details worth knowing before you edit:

- The marquee text is duplicated in two sibling rows. Change one and you must change the other, or the loop will visibly jump.
- The phone number appears in three places: the "Bellen" button, the contact card, and both WhatsApp links.
- Each service photo fills its card with `object-fit: cover`, so the centre of the image is what stays visible as the card changes width.
- The `<title>` and the description and Open Graph meta tags are in the head.

## Known issues

- The email link points to `a.a@naaimaster.nl` but displays `info@naaimaster.nl`. Clicking it mails the first address. Both come from the design source; one of them is wrong.
- The three service photos are circular crops centred on white canvases, so each card shows a circle with white corners rather than a full-bleed photo. Replacing them with rectangular photos fixes it.

## Source

Designed in Claude Design and exported to static HTML. The exported canvas markup uses a `<helmet>` block, `style-hover` attributes, an `<sc-if>` guard, and `<image-slot>` elements, none of which work without the Claude Design runtime; all four were resolved into plain HTML and CSS for this deployment.
