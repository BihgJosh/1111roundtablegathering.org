# 11:11 Roundtable Gathering

Complete source and media for the MDGIFT event website.

## Build

Use Node.js 22 or later:

```sh
npm install
npm run build
npm run preview
```

The production output is `dist/`. The build extracts 12 optimized gallery
photos per year from the original 2023–2025 photo archives. Generated gallery
files and build output are not committed.

## Cloudflare Pages

Connect this repository, select the `main` branch, use `npm run build` as the
build command, and `dist` as the output directory. No framework preset or
server is required. Connect `1111roundtablegathering.org` and `www` through
the project's Custom domains page after deployment.

The original brochure is preserved in `source-media/`; the smaller web copy
in `public/resources/` retains all 16 pages and stays below Pages' asset limit.
The inquiry form validates input and hands off to WhatsApp; it does not store
registrations in a database or send email.

`tests/tests.json` documents the expected desktop and mobile UI workflows.
