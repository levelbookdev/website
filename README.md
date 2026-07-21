# Levelbook website

Source for the Levelbook landing page at [levelbook.dev](https://levelbook.dev).

Levelbook is the umbrella brand for a family of open-source, self-hostable
construction field-records tools. Tag a physical thing, scan it with a stock
phone camera, capture the work in the field, and produce an append-only record
that stands as an accepted contractual deliverable.

The site is a single self-contained page: `docs/index.html`, with inline CSS,
no JavaScript, no webfonts, and no external requests. Total page weight is well
under 50 KB.

## Content inventory

The page covers, and only covers:

- The umbrella statement — tag it, scan it, capture it, keep the record.
- One card per shipped product: a one-sentence pitch in field language, an
  honest status label, a repo link, and a product-page link where one exists.
  Current family: TrenchNote (active, v1.0), LoopCheck (active, pre-release),
  SlipSign (stable v1.0, maintenance), MainLine (dormant, feature-complete for
  shipped phases).
- How the tools are built — self-hosted PocketBase binary, static frontend,
  offline-first, append-only, AGPLv3, no trackers.
- A footer with the source link, the no-analytics statement, and the copyright.

Status labels are load-bearing. A dormant or maintenance-mode tool is labeled
as such on purpose: it signals a portfolio someone is still tending, not one
that was walked away from. Do not quietly upgrade a label to make the page look
busier.

**Rule:** Bindery, managed services, hosting, pricing, and any other commercial
layer stay off this page until further notice. That layer is deliberately
non-public. If a change would add commercial copy here, it does not belong on
this page.

## Local preview

Open the file directly:

```
docs/index.html
```

Or serve the folder over HTTP:

```
cd docs
python3 -m http.server
```

Then visit <http://localhost:8000>.

## Deployment

The site is served by GitHub Pages:

- Source: `main` branch, `/docs` folder.
- Custom domain: `levelbook.dev`, set in `docs/CNAME`.
- Enforce HTTPS is enabled in the repository Pages settings.

Pushing to `main` publishes automatically.

## Design tokens

The page uses the shared Levelbook design tokens, kept in sync with the product
landing pages:

```
--ink:    #14161a
--paper:  #ffffff
--steel:  #5b6470
--line:   #d8dce1
--safety: #ff5a1f
```

## License

[MIT](LICENSE). The Levelbook tools themselves are AGPLv3.
