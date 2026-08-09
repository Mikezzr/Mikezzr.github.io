---
layout: page
permalink: /publications/
title: publications
description: Selected publications and research output.
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

<style>
  .post-header .post-title {
    color: #25313b;
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

<div class="publication-list">
  <div class="publications">

{% bibliography %}

  </div>
</div>
