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
    --global-theme-color: #7654b5;
    --global-hover-color: #5b3e92;
    --global-divider-color: rgba(118, 84, 181, 0.2);
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
    --global-theme-color: #c0a8ed;
    --global-hover-color: #e0d4ff;
    --global-divider-color: rgba(192, 168, 237, 0.28);
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
    border-bottom: 1px solid rgba(118, 84, 181, 0.18);
    background: rgba(222, 239, 255, 0.72) !important;
    backdrop-filter: blur(12px);
  }

  html[data-theme='dark'] body:has(.publication-page) #navbar,
  html[data-theme='dark'] body:has(.publication-page) .navbar {
    border-bottom-color: rgba(192, 168, 237, 0.25);
    background: rgba(20, 30, 46, 0.74) !important;
  }

  .post-header .post-title {
    color: #5a3f91;
    font-weight: 700;
  }

  .post article {
    color: #3f474e;
    font-weight: 400;
  }

  html[data-theme='dark'] .post-header .post-title {
    color: #f3f6f8;
  }

  html[data-theme='dark'] .post article {
    color: #e6edf3;
  }

  .publication-page a {
    color: #7654b5;
  }

  .publication-page a:hover {
    color: #5b3e92;
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
