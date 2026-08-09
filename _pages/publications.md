---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<style>
  body:has(.publication-page) {
    --site-ink: #263746;
    --site-heading: #1d2c3b;
    --site-muted: #526474;
    --site-link: #7654b5;
    --site-link-hover: #5d3c8f;
    --site-line: rgba(38, 55, 70, 0.22);
    --global-text-color: var(--site-ink);
    --global-text-color-light: var(--site-muted);
    --global-theme-color: var(--site-link);
    --global-hover-color: var(--site-link-hover);
    --global-divider-color: var(--site-line);
    --global-footer-bg-color: #4b3778;
    --global-footer-text-color: #e7def8;
    --global-footer-link-color: #fbf9ff;
    background-color: #eef8ff;
    background-image:
      radial-gradient(ellipse 19rem 5.5rem at 9% 8%, rgba(255, 255, 255, 0.84) 0 44%, transparent 72%),
      radial-gradient(ellipse 15rem 4.5rem at 24% 14%, rgba(255, 255, 255, 0.68) 0 42%, transparent 72%),
      radial-gradient(ellipse 21rem 6rem at 83% 18%, rgba(255, 255, 255, 0.75) 0 40%, transparent 72%),
      linear-gradient(180deg, #d9efff 0%, #edf8ff 42%, #ffffff 100%);
    background-attachment: fixed;
  }

  html[data-theme='dark'] body:has(.publication-page) {
    --site-ink: #e6edf3;
    --site-heading: #f5f8fb;
    --site-muted: #b8c5d1;
    --site-link: #c8b6ef;
    --site-link-hover: #e6dcff;
    --site-line: rgba(230, 237, 243, 0.24);
    --global-text-color: var(--site-ink);
    --global-text-color-light: var(--site-muted);
    --global-theme-color: var(--site-link);
    --global-hover-color: var(--site-link-hover);
    --global-divider-color: var(--site-line);
    --global-footer-bg-color: #2a2146;
    --global-footer-text-color: #d8cef0;
    --global-footer-link-color: #fbf9ff;
    background-color: #101d29;
    background-image:
      radial-gradient(ellipse 19rem 5.5rem at 9% 8%, rgba(147, 194, 229, 0.16) 0 44%, transparent 72%),
      radial-gradient(ellipse 15rem 4.5rem at 24% 14%, rgba(147, 194, 229, 0.12) 0 42%, transparent 72%),
      radial-gradient(ellipse 21rem 6rem at 83% 18%, rgba(147, 194, 229, 0.14) 0 40%, transparent 72%),
      linear-gradient(180deg, #122b40 0%, #101d29 55%, #0d151d 100%);
  }

  body:has(.publication-page) #navbar,
  body:has(.publication-page) .navbar {
    border-bottom: 1px solid var(--site-line);
    background: rgba(222, 239, 255, 0.72) !important;
    backdrop-filter: blur(12px);
  }

  html[data-theme='dark'] body:has(.publication-page) #navbar,
  html[data-theme='dark'] body:has(.publication-page) .navbar {
    border-bottom-color: var(--site-line);
    background: rgba(20, 30, 46, 0.74) !important;
  }

  body:has(.publication-page) #navbar a:hover,
  body:has(.publication-page) .navbar a:hover {
    border-radius: 0.25rem;
    background-color: rgba(118, 84, 181, 0.14) !important;
    color: var(--site-link-hover) !important;
  }

  .post-header .post-title {
    color: var(--site-heading);
    font-weight: 700;
  }

  .post article {
    color: var(--site-ink);
    font-weight: 400;
  }

  .publication-page a {
    color: var(--site-link);
  }

  .publication-page a:hover {
    color: var(--site-link-hover);
  }

  .publication-list .publications .row {
    display: flex;
    flex-wrap: nowrap;
    align-items: flex-start;
  }

  .publication-list .publications .row > .abbr {
    flex: 0 0 clamp(180px, 30%, 300px);
    width: auto;
    max-width: none;
  }

  .publication-list .publications .row > .abbr .preview {
    display: block;
    width: 100%;
    height: auto;
  }

  .publication-list .publications .row > [id] {
    flex: 1 1 auto;
    width: auto;
    max-width: none;
  }

  .publication-list .publications .author em,
  .publication-list .publications .author u,
  .publication-list .publications .author strong {
    font-weight: 400;
  }

  .publication-list .publications .links a[href*='arxiv.org'],
  .publication-list .publications .links a[href*='doi.org'],
  .publication-list .publications .links a[href*='github.com'],
  .publication-list .publications .links a[href*='gitlab.com'],
  .publication-list .publications .links a[href*='codeberg.org'] {
    font-size: 0;
  }

  .publication-list .publications .links a[href*='arxiv.org']::after,
  .publication-list .publications .links a[href*='doi.org']::after {
    content: 'paper';
    font-size: 0.875rem;
  }

  .publication-list .publications .links a[href*='github.com']::after,
  .publication-list .publications .links a[href*='gitlab.com']::after,
  .publication-list .publications .links a[href*='codeberg.org']::after {
    content: 'code';
    font-size: 0.875rem;
  }

  @media (max-width: 575.98px) {
    .publication-list .publications .row {
      display: block;
    }

    .publication-list .publications .row > .abbr {
      width: 240px;
      max-width: 72%;
      margin-bottom: 0.75rem;
    }

  }
</style>

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publication-list publication-page">
  <div class="publications">

{% bibliography %}

  </div>
</div>
