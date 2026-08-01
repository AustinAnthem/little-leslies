# League of Little Leslies

The League of Little Leslies campaign site for Austin Anthem and The Fighting Leslies Drinking Club. The campaign supports Equality Texas and is operated by MLS in Austin Supporters Group, a Texas 501(c)(3) nonprofit.

## Stack

- Astro static site
- Plain CSS
- GitHub Pages deployment through GitHub Actions
- Mozilla Public License 2.0

## Local development

Install dependencies and start the development server:

```sh
npm install
npm run dev
```

The local site is available at `http://localhost:4321/little-leslies`.

Create and preview a production build with:

```sh
npm run build
npm run preview
```

## Deployment

Pushes to `main` automatically build and deploy the static site through `.github/workflows/deploy.yml`.

The current project deployment URL is:

`https://austinanthem.github.io/little-leslies`

GitHub Pages must be configured to use **GitHub Actions** as its source. When a custom domain is available, update `site` in `astro.config.mjs` and add a `public/CNAME` file.

## Before campaign launch

The public preview intentionally contains placeholders. Replace or publish the following before accepting entries:

- Real Venmo URL in `src/pages/index.astro`
- Real webstore URL in `src/pages/index.astro`
- Approved artwork and organization logos
- Real contact email and social links
- Formal raffle rules, eligibility details, and required disclosures
- Final legal and beneficiary review

Do not accept public entries until the purchase links, official rules, and required disclosures are complete.

## License

This project is licensed under the Mozilla Public License 2.0. See [`LICENSE`](LICENSE).
