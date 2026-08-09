---
layout: page
permalink: /competitive-programming/
title: Competitive Programming
nav: false
---

<style>
  body:has(.cp-page) {
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

  html[data-theme='dark'] body:has(.cp-page) {
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

  body:has(.cp-page) #navbar,
  body:has(.cp-page) .navbar {
    border-bottom: 1px solid rgba(118, 84, 181, 0.18);
    background: rgba(222, 239, 255, 0.72) !important;
    backdrop-filter: blur(12px);
  }

  html[data-theme='dark'] body:has(.cp-page) #navbar,
  html[data-theme='dark'] body:has(.cp-page) .navbar {
    border-bottom-color: rgba(192, 168, 237, 0.25);
    background: rgba(20, 30, 46, 0.74) !important;
  }

  .cp-page {
    --cp-accent: #7654b5;
    --cp-coral: #c05640;
    color: #2f3437;
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
    background-color: rgba(15, 118, 110, 0.06);
  }

  .cp-page .cp-section--services .cp-list li:hover {
    border-left-color: var(--cp-coral);
    background-color: rgba(192, 86, 64, 0.06);
  }

  .cp-page .cp-year {
    color: var(--cp-accent);
    font-variant-numeric: tabular-nums;
    font-weight: 700;
  }

  .cp-page .cp-section--services .cp-year {
    color: var(--cp-coral);
  }

  html[data-theme='dark'] .cp-page {
    color: #e6edf3;
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
