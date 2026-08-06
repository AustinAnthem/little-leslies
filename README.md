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

The local site is available at `http://localhost:4321/`.

Create and preview a production build with:

```sh
npm run build
npm run preview
```

## Deployment

Pushes to `main` automatically build and deploy the static site through `.github/workflows/deploy.yml`.

The production site is available at:

`https://littleleslies.org`

GitHub Pages must be configured to use **GitHub Actions** as its source. The custom domain is configured in `astro.config.mjs` and `public/CNAME`.

For the Namecheap DNS configuration, point the apex domain to GitHub Pages with these records:

```text
A     @     185.199.108.153
A     @     185.199.109.153
A     @     185.199.110.153
A     @     185.199.111.153
AAAA  @     2606:50c0:8000::153
AAAA  @     2606:50c0:8001::153
AAAA  @     2606:50c0:8002::153
AAAA  @     2606:50c0:8003::153
CNAME www   austinanthem.github.io
```

Enable **Enforce HTTPS** in the repository's GitHub Pages settings after DNS propagation and certificate provisioning complete.

## Before campaign launch

The public preview still contains launch placeholders. Complete the following before accepting entries:

- Real Venmo URL in `src/pages/index.astro`
- Real webstore URL in `src/pages/index.astro`
- Real footer contact email in `src/pages/index.astro` (currently `hello@example.com`)
- Final legal and beneficiary review

Do not accept public entries until the purchase links, official rules, and required disclosures are complete.

## License

This project is licensed under the Mozilla Public License 2.0. See [`LICENSE`](LICENSE).
