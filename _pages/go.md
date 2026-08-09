---
layout: page
permalink: /go/
title: go
description: Go records.
nav: false
---

<style>
  .go-page {
    --go-accent: #0f766e;
    color: #2f3437;
  }

  .go-page h2 {
    margin-top: 1rem;
    margin-bottom: 1.25rem;
    border-bottom: 2px solid var(--go-accent);
    padding-bottom: 0.5rem;
  }

  .go-page .go-records {
    margin: 0;
    padding: 0;
    list-style: none;
  }

  .go-page .go-records li {
    counter-increment: go-record;
    border-bottom: 1px solid var(--global-divider-color);
  }

  .go-page .go-records li::before {
    content: '0' counter(go-record);
    color: var(--go-accent);
    font-size: 0.8rem;
    font-weight: 700;
    letter-spacing: 0.08em;
  }

  .go-page .go-records a {
    display: flex;
    align-items: baseline;
    justify-content: space-between;
    gap: 1rem;
    padding: 1rem 0;
  }

  .go-page .go-records strong {
    color: #25313b;
    font-size: 1.05rem;
  }

  .go-page .go-records span {
    color: #5b6470;
    font-size: 0.92rem;
  }

  .go-page .go-records {
    counter-reset: go-record;
  }

  .go-page .go-records li {
    display: grid;
    grid-template-columns: 2rem minmax(0, 1fr);
    align-items: baseline;
    gap: 0.75rem;
    padding: 0.9rem 0;
  }

  html[data-theme='dark'] .go-page .go-records strong {
    color: #e6edf3;
  }

  html[data-theme='dark'] .go-page {
    color: #e6edf3;
  }

  html[data-theme='dark'] .go-page .go-records span {
    color: #b8c2cc;
  }

  @media (max-width: 575.98px) {
    .go-page .go-records a {
      display: block;
    }

    .go-page .go-records span {
      display: block;
      margin-top: 0.25rem;
    }
  }
</style>

<div class="go-page">
  <h2>Records</h2>
  <ul class="go-records">
    <li>
      <a href="https://119020.github.io/LGU-Go/awards.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener">
        <strong>awards</strong>
        <span>Competition awards and honors</span>
      </a>
    </li>
    <li>
      <a href="https://119020.github.io/LGU-Go/history.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener">
        <strong>history</strong>
        <span>Historical games and participation</span>
      </a>
    </li>
    <li>
      <a href="https://119020.github.io/LGU-Go/records.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener">
        <strong>records</strong>
        <span>Detailed Go records</span>
      </a>
    </li>
  </ul>
</div>
