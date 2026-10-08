# Printaverses

A static, responsive website for Printaverses and its 17 collections. Nineteen related registered domains map to these pages; `printandroid.com` and `printapod.com` are aliases. Scope was confirmed by the user on 8 October 2026. ASIprints and Starprints are excluded.

## Local use

```text
npm run build
npm run check
npm run preview
```

No package installation is needed. Node.js builds the static HTML from `brands.json`. The stylesheet and browser script are maintained in `dist/`. All site paths are relative and work under the custom domain or a GitHub project path.

The public repository currently contains `website-source.zip`, the editable source and optimized assets. Extract it before local development. Its root workflow extracts the archive, builds and checks the website, then deploys `dist/`. The workflow inside the archive also supports publishing a normal extracted checkout.

## Artwork

Eighteen new AI-generated concepts (one main hero and one per collection), plus three existing concept-journal images and the established gray P icon. All generated artwork is identified as concept imagery; no inventory, print-tested models, product safety or availability is claimed. `concept-prompts.json` preserves the new prompts. Optimized WebP assets are tracked; full-resolution PNG originals remain locally in `artwork/`.

## Business identity

Every page links back to Printaverses and includes Metaversal Arts attribution, Metaversalarts e.U., Roger Bootsma, Vienna and company registration FN 687427 y. The legal notice follows the public business details in https://metaversalarts.io/legal.html and the existing Metaversal Arts project files. No authentication credentials are included.

## Security and privacy

The site contains only local static assets and browser interactions. It has no accounts, payment processing, analytics, cookies, personal-data storage, dependencies loaded from CDNs, or server endpoints. Content Security Policy restricts scripts, styles, images and fonts to the site's own origin, disables network connections, plugins, base tags and form submission. Referrers use strict-origin-when-cross-origin. Search and dialogue content use textContent, not HTML injection.

GitHub Pages must issue the custom-domain certificate and have Enforce HTTPS enabled before the domain is considered ready. GitHub Pages does not support arbitrary custom response headers; this is not a penetration test or a claim of complete security. DNS and TLS state must be verified after deployment.

## Deployment status, 8 October 2026

The main deployment passed. Main-domain DNS and nine companion domains have verified Pages bindings and DNS. Ten further companion domains have prepared redirect files, but GitHub temporarily blocked additional repository creation. Certificates were still pending at the last actual TLS check. This is not yet a verified HTTPS launch. See `deployment-status.json` for the exact domains and next steps.

## Domain routing

`domain-map.json` lists all nineteen related domains and the corresponding canonical pages on `https://printaverses.com/`. Do not point all hostnames at a single Pages repository and assume path routing. Use one HTTPS redirect Pages repository per domain, each bound to that hostname, or an HTTPS-capable redirect host. Namecheap URL forwarding alone does not establish HTTPS support for the source hostname.

Configure each hostname on its hosting repository before changing DNS. Preserve unrelated MX/TXT and other service records. No wildcard DNS is needed. See GitHub's custom-domain documentation: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site

Copyright © 2026 Roger Bootsma / Metaversal Arts.
