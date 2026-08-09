---
layout: page
permalink: /competitive-programming/
title: Competitive Programming
description:
nav: false
---

<style>
  .cp-page {
    --cp-accent: #0f766e;
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
        <span class="cp-year">2023</span>
        <div><strong>Gold Medal, 48th ICPC Jinan Regional</strong></div>
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
