---
layout: page
permalink: /competitive-programming/
title: Competitive Programming
description:
nav: false
---

<style>
  .cp-page {
    --cp-ink: #25313b;
    --cp-accent: #0f766e;
    --cp-coral: #c05640;
    color: var(--cp-ink);
  }

  .cp-page .cp-masthead {
    display: grid;
    grid-template-columns: 8rem minmax(0, 1fr);
    gap: 1.5rem;
    align-items: center;
    margin: 0 0 3rem;
    border-radius: 4px;
    background: #183c3b;
    padding: 1.75rem 2rem;
    color: #f7faf9;
  }

  .cp-page .cp-mark {
    color: #9bd3c8;
    font-size: 6rem;
    font-weight: 800;
    letter-spacing: 0.04em;
    line-height: 0.8;
  }

  .cp-page .cp-kicker {
    margin: 0 0 0.4rem;
    color: #f1b78a;
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.12em;
    text-transform: uppercase;
  }

  .cp-page .cp-masthead h2 {
    margin: 0;
    border: 0;
    padding: 0;
    color: #ffffff;
    font-size: 1.8rem;
  }

  .cp-page .cp-masthead p {
    max-width: 38rem;
    margin: 0.65rem 0 0;
    color: #d8e9e5;
    line-height: 1.65;
  }

  .cp-page .cp-section {
    margin-top: 2.5rem;
  }

  .cp-page .cp-section-heading {
    display: flex;
    align-items: baseline;
    gap: 0.75rem;
    margin-bottom: 0.75rem;
    border-bottom: 2px solid var(--cp-accent);
    padding-bottom: 0.5rem;
  }

  .cp-page .cp-section-heading h2 {
    margin: 0;
    border: 0;
    padding: 0;
  }

  .cp-page .cp-section-index {
    color: var(--cp-accent);
    font-size: 0.85rem;
    font-weight: 700;
    letter-spacing: 0.08em;
  }

  .cp-page .cp-section--services .cp-section-heading {
    border-color: var(--cp-coral);
  }

  .cp-page .cp-section--services .cp-section-index {
    color: var(--cp-coral);
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
    padding: 0.85rem 0;
    border-bottom: 1px solid var(--global-divider-color);
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
    --cp-ink: #e6edf3;
  }

  @media (max-width: 575.98px) {
    .cp-page .cp-masthead {
      grid-template-columns: 1fr;
      gap: 1rem;
      padding: 1.4rem;
    }

    .cp-page .cp-mark {
      font-size: 4.5rem;
    }

    .cp-page .cp-masthead h2 {
      font-size: 1.5rem;
    }

    .cp-page .cp-list li {
      grid-template-columns: 5.5rem minmax(0, 1fr);
      gap: 0.75rem;
    }
  }
</style>

<div class="cp-page">
  <div class="cp-masthead">
    <div class="cp-mark" aria-hidden="true">CP</div>
    <div>
      <p class="cp-kicker">Algorithms under pressure</p>
      <h2>Simple, effective ideas.</h2>
      <p>Competitive programming has shaped how I approach algorithms: start from a precise model, find the essential structure, and build a solution that works.</p>
    </div>
  </div>

  <section class="cp-section" aria-labelledby="cp-awards">
    <div class="cp-section-heading">
      <span class="cp-section-index">01</span>
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
      <span class="cp-section-index">02</span>
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
