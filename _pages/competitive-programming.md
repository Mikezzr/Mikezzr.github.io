---
layout: page
permalink: /competitive-programming/
title: competitive programming
description: Selected competitive programming results.
nav: false
---

<style>
  .activity-page {
    --activity-accent: #0f766e;
  }

  .activity-page .activity-lead {
    max-width: 44rem;
    font-size: 1.08rem;
    line-height: 1.7;
  }

  .activity-page .activity-summary {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin: 2rem 0 2.5rem;
  }

  .activity-page .activity-stat {
    border-top: 3px solid var(--activity-accent);
    padding: 0.8rem 0.2rem 0;
  }

  .activity-page .activity-stat strong,
  .activity-page .activity-stat span {
    display: block;
  }

  .activity-page .activity-stat strong {
    color: var(--activity-accent);
    font-size: 1.15rem;
  }

  .activity-page .activity-stat span {
    margin-top: 0.3rem;
    color: var(--global-text-color-light);
    font-size: 0.9rem;
    line-height: 1.45;
  }

  .activity-page .activity-section {
    margin-top: 2.5rem;
  }

  .activity-page .activity-section h2 {
    margin-bottom: 0.8rem;
  }

  .activity-page .award-list {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .activity-page .award-item {
    display: grid;
    grid-template-columns: 7rem minmax(0, 1fr);
    gap: 1rem;
    padding: 0.9rem 0;
    border-top: 1px solid var(--global-divider-color);
  }

  .activity-page .award-item time {
    color: var(--activity-accent);
    font-variant-numeric: tabular-nums;
    font-weight: 700;
  }

  .activity-page .award-item strong {
    font-weight: 600;
  }

  .activity-page .award-item p {
    margin: 0.25rem 0 0;
    color: var(--global-text-color-light);
    font-size: 0.92rem;
  }

  @media (max-width: 575.98px) {
    .activity-page .activity-summary {
      grid-template-columns: 1fr;
      gap: 1.25rem;
    }

    .activity-page .award-item {
      grid-template-columns: 5.5rem minmax(0, 1fr);
      gap: 0.75rem;
    }
  }
</style>

<div class="activity-page">
  <p class="activity-lead">
    Competitive programming has shaped how I approach algorithms: start from a precise model, find the essential structure, and build a solution that is both simple and effective.
  </p>

  <div class="activity-summary">
    <div class="activity-stat">
      <strong>World Finals</strong>
      <span>Advanced through the 48th ICPC Macau Regional</span>
    </div>
    <div class="activity-stat">
      <strong>Five gold medals</strong>
      <span>ICPC, CCPC, and collegiate programming contests</span>
    </div>
    <div class="activity-stat">
      <strong>NOI / APIO</strong>
      <span>Silver medals in 2021</span>
    </div>
  </div>

  <section id="icpc-ccpc" class="activity-section">
    <h2>ICPC, CCPC, and other contests</h2>
    <ul class="award-list">
      <li class="award-item">
        <time datetime="2023">2023</time>
        <div>
          <strong>Third Place, 48th ICPC Macau Regional</strong>
          <p>Advanced to the 48th ICPC World Finals.</p>
        </div>
      </li>
      <li class="award-item">
        <time datetime="2024">2024</time>
        <div><strong>Second Place, 2nd CUHK-Shenzhen Programming Contest</strong></div>
      </li>
      <li class="award-item">
        <time datetime="2023">2023</time>
        <div><strong>Gold Medal, 47th ICPC Hong Kong Regional</strong></div>
      </li>
      <li class="award-item">
        <time datetime="2024">2024</time>
        <div><strong>Gold Medal, 48th ICPC Jinan Regional</strong></div>
      </li>
      <li class="award-item">
        <time datetime="2024">2024</time>
        <div><strong>Gold Medal, 49th ICPC Kunming Regional</strong></div>
      </li>
      <li class="award-item">
        <time datetime="2023">2023</time>
        <div><strong>Gold Medal, 9th CCPC Shenzhen Regional</strong></div>
      </li>
      <li class="award-item">
        <time datetime="2023">2023</time>
        <div><strong>Gold Medal, 19th Baidu Star Programming Contest (Collegiate Section)</strong></div>
      </li>
    </ul>
  </section>

  <section id="olympiads" class="activity-section">
    <h2>Olympiads</h2>
    <ul class="award-list">
      <li class="award-item">
        <time datetime="2021">2021</time>
        <div><strong>Silver Medal, National Olympiad in Informatics (NOI)</strong></div>
      </li>
      <li class="award-item">
        <time datetime="2021">2021</time>
        <div><strong>Silver Medal, Asia-Pacific Informatics Olympiad (APIO)</strong></div>
      </li>
    </ul>
  </section>
</div>
