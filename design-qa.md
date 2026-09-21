# HORK website design QA

## Evidence

- Source visual truth:
  - Final Home reference supplied by the user: `/var/folders/d3/0jmfz87d5fs7hk5q3mxt1yjc0000gn/T/codex-clipboard-b72440fa-fdd1-46ff-9b78-322fecd3c4bd.png`
  - Home: `/Users/uj/.codex/generated_images/01a061b7-9b2b-7db2-81d7-13996be5a9ea/exec-12cb268c-9e6d-426c-99e9-4014dd4d9741.png`
  - Our Brands: `/Users/uj/.codex/generated_images/01a061b7-9b2b-7db2-81d7-13996be5a9ea/exec-9a0d1570-a528-4c2b-8806-115dceb32dc8.png`
  - Our Customers: `/Users/uj/.codex/generated_images/01a061b7-9b2b-7db2-81d7-13996be5a9ea/exec-458f4ead-26f4-4355-8e54-536706569fb3.png`
  - Contact: `/Users/uj/.codex/generated_images/01a061b7-9b2b-7db2-81d7-13996be5a9ea/exec-da62a4ee-d887-41b5-b738-daba3384ac2b.png`
- Browser-rendered implementation screenshots:
  - `/Users/uj/Desktop/Projects/HORK/HORK Branding/qa-index.png`
  - `/Users/uj/Desktop/Projects/HORK/HORK Branding/qa-brands.png`
  - `/Users/uj/Desktop/Projects/HORK/HORK Branding/qa-customers.png`
  - `/Users/uj/Desktop/Projects/HORK/HORK Branding/qa-contact.png`
- Browser state: local production-static routes, light theme, unauthenticated.
- Viewport/evidence: visible in-app browser content within a 1512 × 982 CSS-pixel desktop; screenshots are 3024 × 1964 at 2× device density. Source mocks are 1536 × 1024. Comparisons accounted for browser chrome and the small aspect-ratio difference.

## Full-view comparison evidence

The rendered pages preserve the approved information hierarchy and visual direction: warm cream ground, rust display typography, compact navigation, shared H/lotus and Omira system, practical colourful textile imagery, equal wholesale/retail weight, an India-led customer map, and the split-brand contact flow. The implementation intentionally adapts the mockup's fixed canvas into responsive page sections.

## Focused region comparison evidence

Focused checks covered the shared header, H-lotus mark, dotless `omıra` wordmark with lotus above the word, equal brand columns, customer-region labels, state list, contact cards, and form alignment. The generated five-petal lotus replaced the earlier generic floral glyph after the first browser review.

## Required fidelity surfaces

- Fonts and typography: display serif/sans hierarchy, weights, wrapping and small uppercase tracking match the approved editorial direction.
- Spacing and layout rhythm: section spacing, paired columns, card padding, borders and radii are consistent; no clipped primary controls were observed.
- Colors and visual tokens: cream, rust, antique gold and charcoal tokens are consistent across all routes with readable contrast.
- Image quality and asset fidelity: the practical mid-market textile-shop photography is sharp and avoids the rejected luxury/bridal direction; the map and lotus are dedicated raster assets rather than placeholders.
- Copy and content: locked copy is present. Customer reach now includes Uttarakhand, Rajasthan, Bihar, Afghanistan and Africa while keeping India visibly primary.

## Findings

- No actionable P0, P1 or P2 mismatch remained after the final browser comparison.

## Comparison history

1. Initial browser pass found the shared lotus rendered as a generic gear-like flower (P2 asset mismatch).
2. Fix: generated and installed a dedicated five-petal antique-gold lotus asset for both the H crossbar and Omira crown.
3. The first published homepage then drifted from the approved composition: its hero headline was oversized and pushed both brand cards below the first screen (P1 hierarchy mismatch).
4. Fix: rebuilt the homepage as the approved three-column editorial composition—story at left, equal wholesale and retail cards at right—with the value strip and textile quote immediately below.
5. Post-fix evidence: `qa-index.png` now matches the final user-supplied homepage reference at a 1536 × 1024 viewport.
6. A live-browser review exposed font and pseudo-element drift in the H and Omira marks (P1 brand-fidelity mismatch).
7. Fix: replaced every assembled text logo with three locked transparent PNG assets: `h-mark.png`, `hari-om-raj-kumar-logo.png`, and `omira-logo.png`. The same pixels now render in the navigation, brand cards, contact page and footer.

## Primary interactions tested

- All six routes returned HTTP 200 locally: Home, Our Brands, Our Customers, Contact, Privacy and Support.
- Main navigation links were opened in the in-app browser.
- Contact form script passed JavaScript syntax validation and constructs a pre-addressed email to `support@hork.in`.
- No browser-visible loading failures appeared during route checks.

## Implementation checklist

- [x] Responsive page system
- [x] Locked Home, Our Brands, Our Customers and Contact layouts
- [x] Shared navigation and footer
- [x] Privacy and Support retained and visually connected
- [x] Expanded India and international customer reach
- [x] Browser render review and route validation

## Follow-up polish

- P3: replace the email-client contact action with a server-backed form if HORK later needs stored enquiries or automated acknowledgements.

## September 21 logo correction

The earlier recreated PNGs did not faithfully match the accepted marks. They have been replaced with SVG image viewports containing the original raster artwork from the approved homepage reference. A display filter removes the near-white paper around the artwork; lettering and lotus shapes are no longer recreated from fonts. The embedded raster retains the resolution limits of the supplied mockup.

Both homepage cards now use the same 390px height and shared label, image and caption rows. Browser screenshots at 1280px confirmed matching top/bottom edges and the original artwork. Intermediate-width hero contrast and the missing space at the heading line break were also corrected.

final result: logo and card alignment correction visually verified locally; wider website fidelity is not claimed by this check.
