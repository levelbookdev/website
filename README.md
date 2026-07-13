# Levelbook website

Source for the Levelbook landing page at [levelbook.dev](https://levelbook.dev).

Levelbook is the umbrella brand for a family of open-source, self-hostable
construction field-records tools. Tag a physical thing, scan it with a stock
phone camera, capture the work in the field, and produce an append-only record
that stands as an accepted contractual deliverable.

The site is a single self-contained page: `docs/index.html`, with inline CSS,
no JavaScript, no webfonts, and no external requests. Total page weight is well
under 50 KB.

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
