---
layout: page
permalink: /competitive-programming/
title: Competitive Programming
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
    --cp-accent-soft: rgba(118, 84, 181, 0.12);
    --cp-coral: #a6533d;
    --cp-coral-soft: rgba(166, 83, 61, 0.1);
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
    --cp-accent-soft: rgba(200, 182, 239, 0.14);
    --cp-coral: #e3aa95;
    --cp-coral-soft: rgba(227, 170, 149, 0.14);
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

  .cp-page {
    --cp-accent: var(--site-link);
    color: var(--site-ink);
  }

  .cp-page .cp-section {
    margin-top: 2.25rem;
  }

  .cp-page .cp-section:first-child {
    margin-top: 0.5rem;
  }

  .cp-page .cp-section-heading {
    margin-bottom: 0.75rem;
    border-bottom: 3px solid var(--cp-accent);
    padding-bottom: 0.5rem;
  }

  .cp-page .cp-section-heading h2 {
    margin: 0;
    border: 0;
    color: var(--site-heading);
    padding: 0;
  }

  .cp-page .cp-section--services .cp-section-heading {
    border-color: var(--cp-coral);
  }

  .cp-page .cp-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .cp-page .cp-list li {
    display: grid;
    grid-template-columns: 7rem minmax(0, 1fr);
    gap: 1rem;
    border-bottom: 1px solid var(--global-divider-color);
    border-left: 3px solid transparent;
    padding: 0.85rem 0.75rem;
    transition: border-color 160ms ease, background-color 160ms ease;
  }

  .cp-page .cp-list li:hover {
    border-left-color: var(--cp-accent);
    background-color: var(--cp-accent-soft);
  }

  .cp-page .cp-section--services .cp-list li:hover {
    border-left-color: var(--cp-coral);
    background-color: var(--cp-coral-soft);
  }

  .cp-page .cp-year {
    color: var(--cp-accent);
    font-variant-numeric: tabular-nums;
    font-weight: 700;
  }

  .cp-page .cp-section--services .cp-year {
    color: var(--cp-coral);
  }

  @media (max-width: 575.98px) {
    .cp-page .cp-list li {
      grid-template-columns: 5.5rem minmax(0, 1fr);
      gap: 0.75rem;
      padding-right: 0.5rem;
      padding-left: 0.5rem;
    }
  }
</style>

<div class="cp-page">
  <section class="cp-section" aria-labelledby="cp-awards">
    <div class="cp-section-heading">
      <h2 id="cp-awards">Awards</h2>
    </div>
    <ul class="cp-list">
      <li>
        <span class="cp-year">2024</span>
        <div><strong>Second Place, 2nd CUHK-Shenzhen Programming Contest</strong></div>
      </li>
      <li>
        <span class="cp-year">2024</span>
        <div><strong>Gold Medal, 49th ICPC Kunming Regional</strong></div>
      </li>
      <li>
        <span class="cp-year">2023</span>
        <div><strong>Third Place, 48th ICPC Macau Regional (Advanced to the 48th ICPC World Finals)</strong></div>
      </li>
      <li>
        <span class="cp-year">2023</span>
        <div><strong>Gold Medal, 48th ICPC Jinan Regional</strong></div>
      </li>
      <li>
        <span class="cp-year">2023</span>
        <div><strong>Gold Medal, 47th ICPC Hong Kong Regional</strong></div>
      </li>
      <li>
        <span class="cp-year">2023</span>
        <div><strong>Gold Medal, 9th CCPC Shenzhen Regional</strong></div>
      </li>
      <li>
        <span class="cp-year">2023</span>
        <div><strong>Gold Medal, 19th Baidu Star Programming Contest (Collegiate Section)</strong></div>
      </li>
      <li>
        <span class="cp-year">2021</span>
        <div><strong>Silver Medal, National Olympiad in Informatics (NOI)</strong></div>
      </li>
      <li>
        <span class="cp-year">2020</span>
        <div><strong>Silver Medal, Asia-Pacific Informatics Olympiad (APIO)</strong></div>
      </li>
    </ul>
  </section>

  <section class="cp-section cp-section--services" aria-labelledby="cp-services">
    <div class="cp-section-heading">
      <h2 id="cp-services">Services</h2>
    </div>
    <ul class="cp-list">
      <li>
        <span class="cp-year">2025-2026</span>
        <div><strong>Instructor for Competitive Programming Courses, X-Camp</strong></div>
      </li>
      <li>
        <span class="cp-year">2025-2026</span>
        <div><strong>Problem Setter, Greater Bay Area International Programming Contest</strong></div>
      </li>
      <li>
        <span class="cp-year">2023-2024</span>
        <div><strong>Organizing Committee Member, CUHK-Shenzhen Programming Contest</strong></div>
      </li>
    </ul>
  </section>
</div>
