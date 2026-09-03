# Golf at X3 Fort Myers: concept proposal

A single page showing what a golf performance program would look like running inside
X3 Performance and Physical Therapy, 13050 Metro Parkway, Fort Myers. Prepared by
Ryan Hogan. Built by Cross Designs.

## This page is fenced, and the fences stay

It carries X3's real logo, real facility facts and real Google rating, so:

- `<meta name="robots" content="noindex, nofollow">` in the head
- No LocalBusiness or Organization JSON-LD. Structured data claiming to be X3 would be
  the one thing on this page that is not honest, so there is none
- A footer disclaimer stating the page is a concept proposal by Ryan Hogan, is not
  published, endorsed or operated by X3, that no partnership exists, and that the X3
  marks and facts are reproduced from x3ppt.com for the purpose of this proposal

Do not remove any of those three without a conversation with Ryan first. Nobody has
asked X3 whether they mind their marks being used this way. That conversation belongs
to Ryan and should happen before the link is shared beyond him.

## Two readers, one page

The surface is a golfer facing booking page. The last two sections before contact are
the pitch to X3 itself, deep linkable at `#partnership` so a decision maker can be sent
straight to the ask.

## Visual direction

Dark dominant, athletic, photography at full scale. Saira Condensed 800 for display,
Jost for body, IBM Plex Mono confined to actual data values. X3 red as a real accent
rather than a tint. Every colour traced to X3's own stylesheet.

Section grounds alternate deliberately: dark hero, full bleed facility band, light
method, dark hour, light coach, dark objections, light programs, darker roster,
dark partnership, light contact, dark footer.

## Measured, not assumed

Headless Chromium at 390x844 and 1440x900:

| Check | Mobile 390 | Desktop 1440 |
|---|---|---|
| Horizontal overflow | 0 | 0 |
| WCAG contrast failures | 0 | 0 |
| Pseudo-element rules beside text | 0 | 0 |
| Uppercase micro-labels | 4 | 4 |
| Non-pressable pills | 0 | 0 |
| Console errors | 0 | 0 |
| Swipes, hero to footer | 14.4 | 11.5 |

The 14.4 mobile swipe count is above the 8 to 10 target and is a known, accepted
overrun. Eleven sections carry load bearing argument and none is padding. Getting to 10
would mean deleting parts of the pitch. Flagged here rather than hidden.

Headless Chromium hides scrollbars, so zero overflow needs one confirmation in a
painting browser at 390 wide on the deployed URL.

## Open items

1. `[EMAIL ADDRESS NEEDED]` appears twice. Ryan's `ryan@redlinegolfacademy.com` address
   dies with the Redline brand, so a new one is needed.
2. No og:image. A designed 1200x630 share card does not exist, so the link previews
   badly over iMessage.
3. Zero golf testimonials. The Redline site's testimonials were fabricated and were
   deliberately not carried over. The only social proof here is X3's real Google rating.
   Real quotes from real students would be the single biggest improvement available.
4. The revenue split is deliberately left as the one open question on the page.
5. The contact form is not wired to anything. It validates and shows a success state
   that explicitly says nothing was transmitted.

## Repo contents

- `index.html` is the page. All CSS and JS inline. External dependencies are Google
  Fonts and Font Awesome 6 only.
- `assets/` holds the six referenced files: `x3-logo-alt.png`,
  `ryan-followthrough-monitor-hero.jpg`, `ryan-swing-launch-monitor.webp`,
  `ryan-backswing-portrait.webp`, `x3-fortmyers-facility.jpg`, `cross-designs.png`.
  All X3 images were downloaded rather than hotlinked.
- `.nojekyll` so GitHub Pages serves the tree as is.

Internal notes (design direction, QA scripts, credentials) stay local and are excluded
by `.gitignore`. They are never served from this domain.
