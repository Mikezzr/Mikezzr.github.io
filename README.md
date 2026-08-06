# Zirong Zeng's Personal Homepage

Source code for [Mikezzr.github.io](https://Mikezzr.github.io), built with Jekyll and the al-folio starter.

## Main content

- Homepage: `_pages/about.md`
- Publications: `_bibliography/papers.bib`
- Projects: `_projects/`
- CV page: `_data/cv.yml`
- CV PDF: `assets/pdf/cv.pdf`
- News: `_news/`
- Teaching: `_teachings/`
- Social links: `_data/socials.yml`
- Site settings: `_config.yml`

## Local development

Install the Ruby dependencies and start the development server:

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://localhost:4000>.

## Formatting

```bash
npm ci
npm run lint:prettier
```

To fix formatting automatically:

```bash
npx prettier . --write
```

## Deployment

Pushing to `main` runs `.github/workflows/deploy.yml`, builds the site, and publishes the generated `_site` directory to the `gh-pages` branch.
