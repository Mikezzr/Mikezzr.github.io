---
layout: page
permalink: /badminton/
title: Badminton
nav: false
---

<style>
  body {
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
    --badminton-accent-soft: rgba(118, 84, 181, 0.12);
    background-color: #eef8ff;
    background-image:
      radial-gradient(ellipse 19rem 5.5rem at 9% 8%, rgba(255, 255, 255, 0.84) 0 44%, transparent 72%),
      radial-gradient(ellipse 15rem 4.5rem at 24% 14%, rgba(255, 255, 255, 0.68) 0 42%, transparent 72%),
      radial-gradient(ellipse 21rem 6rem at 83% 18%, rgba(255, 255, 255, 0.75) 0 40%, transparent 72%),
      linear-gradient(180deg, #d9efff 0%, #edf8ff 42%, #ffffff 100%);
    background-attachment: fixed;
  }

  html[data-theme='dark'] body {
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
    --badminton-accent-soft: rgba(200, 182, 239, 0.14);
    background-color: #101d29;
    background-image:
      radial-gradient(ellipse 19rem 5.5rem at 9% 8%, rgba(147, 194, 229, 0.16) 0 44%, transparent 72%),
      radial-gradient(ellipse 15rem 4.5rem at 24% 14%, rgba(147, 194, 229, 0.12) 0 42%, transparent 72%),
      radial-gradient(ellipse 21rem 6rem at 83% 18%, rgba(147, 194, 229, 0.14) 0 40%, transparent 72%),
      linear-gradient(180deg, #122b40 0%, #101d29 55%, #0d151d 100%);
  }

  #navbar,
  .navbar {
    border-bottom: 1px solid var(--site-line);
    background: rgba(222, 239, 255, 0.72) !important;
    backdrop-filter: blur(12px);
  }

  html[data-theme='dark'] #navbar,
  html[data-theme='dark'] .navbar {
    border-bottom-color: var(--site-line);
    background: rgba(20, 30, 46, 0.74) !important;
  }

  #navbar a:hover,
  .navbar a:hover {
    border-radius: 0.25rem;
    background-color: rgba(118, 84, 181, 0.14) !important;
    color: var(--site-link-hover) !important;
  }

  html[data-theme='dark'] #navbar a:hover,
  html[data-theme='dark'] .navbar a:hover {
    background-color: rgba(200, 182, 239, 0.26) !important;
    color: #f5f8fb !important;
  }

  .badminton-page {
    --badminton-accent: var(--site-link);
    color: var(--site-ink);
  }

  .badminton-page .badminton-section {
    margin-top: 2.25rem;
  }

  .badminton-page .badminton-section:first-child {
    margin-top: 0.5rem;
  }

  .badminton-page .badminton-section-heading {
    margin-bottom: 0.75rem;
    border-bottom: 3px solid var(--badminton-accent);
    padding-bottom: 0.5rem;
  }

  .badminton-page .badminton-section-heading h2 {
    margin: 0;
    border: 0;
    color: var(--site-heading);
    padding: 0;
  }

  .badminton-page .badminton-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .badminton-page .badminton-list li {
    display: grid;
    grid-template-columns: 7rem minmax(0, 1fr);
    gap: 1rem;
    border-bottom: 1px solid var(--global-divider-color);
    border-left: 3px solid transparent;
    padding: 0.85rem 0.75rem;
    transition: border-color 160ms ease, background-color 160ms ease;
  }

  .badminton-page .badminton-list li:hover {
    border-left-color: var(--badminton-accent);
    background-color: var(--badminton-accent-soft);
  }

  .badminton-page .badminton-year {
    color: var(--badminton-accent);
    font-variant-numeric: tabular-nums;
    font-weight: 700;
  }

  @media (max-width: 575.98px) {
    .badminton-page .badminton-list li {
      grid-template-columns: 5.5rem minmax(0, 1fr);
      gap: 0.75rem;
      padding-right: 0.5rem;
      padding-left: 0.5rem;
    }
  }
</style>

<div class="badminton-page">
  <section class="badminton-section" aria-labelledby="badminton-awards">
    <div class="badminton-section-heading">
      <h2 id="badminton-awards">Awards</h2>
    </div>
    <ul class="badminton-list">
      <li>
        <span class="badminton-year">2026</span>
        <div><strong>Champion, Mixed Doubles, CUHK-Shenzhen Freshman Cup Badminton Tournament</strong></div>
      </li>
      <li>
        <span class="badminton-year">2026</span>
        <div><strong>Third Place, Men's Singles, CUHK-Shenzhen Freshman Cup Badminton Tournament</strong></div>
      </li>
    </ul>
  </section>
</div>
