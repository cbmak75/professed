# professed.ai

A declaration for AI-native law. The manifesto and thesis by Chris Dias, solicitor of England and Wales, on why the race to make law firms AI-native is right, and why the public declaration at the heart of the legal profession is the line AI must never cross.

Live at [www.professed.ai](https://www.professed.ai), hosted on Netlify.

## The site

Five pages, static HTML, no build step, no frameworks.

| Page | File | What it is |
|---|---|---|
| Home | `index.html` | The idea in brief: the etymology of profess, the line, and the mantra. |
| The manifesto | `manifesto.html` | Twelve declarations on AI-native legal practice, in the tradition of the Twelve Tables. |
| The thesis | `thesis.html` | The full essay: to profess, what clients are buying, the line, the bottleneck, and the line of ink. |
| The codes | `codes.html` | The twelve declarations mapped, provision by provision, against the SRA Standards and Regulations and the BSB Handbook, with both regulators' AI positions. |
| See it in practice | `in-practice.html` | The declaration of interest, what we are building, and the loop: Lawyery, Professed, Countersigned, NativeLaw. |

`404.html` is served by Netlify for unknown paths and is noindexed.

## Structure and conventions

- `styles.css` carries all styling, including the page-specific cycle diagram and codes table sections. No page has its own style block.
- The header is identical on every page: brand, a standalone manifesto button, and a burger menu at all screen sizes. The dropdown is green with uniform link colouring.
- Each page hero carries its own version of the wax seal: PROFITERI on the home page, then MANIFESTO, THESIS, CODES and PRACTICE (`seal-*.svg`). The nav mark, favicon and share image use the original seal.
- Quote bands cite the declarations (for example Declaration XII), not the author.
- UK English throughout. No em-dashes.

## SEO and sharing

- Every content page has a canonical URL, full Open Graph and Twitter card tags, and JSON-LD structured data.
- `og-image.png` (1200 by 630) is the share card for all pages.
- `sitemap.xml` and `robots.txt` are in the root. Canonical URLs use the extensionless form (Netlify pretty URLs), for example `/manifesto`.

## Maintenance notes

- Regulatory quotations on the codes page were verified against the versions in force on 22 July 2026, including BSB Handbook version 5.0 (in force 15 June 2026) and the SRA Codes as then published. Re-verify against current published versions before citing.
- After deploying content changes, update the `lastmod` dates in `sitemap.xml`.
- DNS: apex ALIAS to `apex-loadbalancer.netlify.com`, `www` CNAME to the Netlify site subdomain.

## Legal

Commentary and opinion, not legal advice. Legal services referred to on the site are provided by Lawyery Limited, authorised and regulated by the Solicitors Regulation Authority (SRA 8001894).

Copyright 2026 Chris Dias. All rights reserved.
