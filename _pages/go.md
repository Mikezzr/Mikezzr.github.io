---
layout: page
permalink: /go/
title: go
nav: false
---

<style>
  .go-page {
    --go-board: #d8ad68;
    --go-ink: #27313a;
    --go-accent: #0f766e;
    color: var(--go-ink);
  }

  .go-page .go-layout {
    display: grid;
    grid-template-columns: minmax(240px, 0.8fr) minmax(0, 1fr);
    gap: 2.5rem;
    align-items: center;
    margin-top: 1.5rem;
  }

  .go-page .go-board-frame {
    border: 1px solid #b58b4f;
    background: #f1e2c2;
    padding: 0.85rem;
  }

  .go-page .go-board {
    position: relative;
    aspect-ratio: 1;
    border: 1px solid #78572f;
    background-color: var(--go-board);
    background-image: repeating-linear-gradient(to right, transparent 0, transparent calc(11.111% - 1px), #78572f calc(11.111% - 1px), #78572f 11.111%), repeating-linear-gradient(to bottom, transparent 0, transparent calc(11.111% - 1px), #78572f calc(11.111% - 1px), #78572f 11.111%);
  }

  .go-page .go-stone {
    position: absolute;
    width: 9%;
    aspect-ratio: 1;
    transform: translate(-50%, -50%);
    border-radius: 50%;
    box-shadow: 0 0.2rem 0.35rem rgba(39, 49, 58, 0.28);
  }

  .go-page .go-stone--black {
    background: #18232c;
  }

  .go-page .go-stone--white {
    border: 1px solid #9b8a72;
    background: #f6f1e7;
  }

  .go-page .go-stone--one {
    top: 22.2%;
    left: 33.3%;
  }

  .go-page .go-stone--two {
    top: 33.3%;
    left: 55.6%;
  }

  .go-page .go-stone--three {
    top: 55.6%;
    left: 44.4%;
  }

  .go-page .go-stone--four {
    top: 66.7%;
    left: 66.7%;
  }

  .go-page .go-stone--five {
    top: 77.8%;
    left: 22.2%;
  }

  .go-page .go-records {
    margin: 0;
    padding: 0;
    list-style: none;
    counter-reset: go-record;
  }

  .go-page .go-records li {
    display: grid;
    grid-template-columns: 2.25rem minmax(0, 1fr);
    gap: 0.75rem;
    align-items: baseline;
    border-bottom: 1px solid var(--global-divider-color);
    counter-increment: go-record;
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
    color: var(--go-ink);
    font-size: 1.08rem;
    text-transform: lowercase;
  }

  .go-page .go-records a::after {
    content: '->';
    color: var(--go-accent);
    font-size: 1.1rem;
    transition: transform 160ms ease;
  }

  .go-page .go-records a:hover::after {
    transform: translateX(0.3rem);
  }

  html[data-theme='dark'] .go-page {
    --go-ink: #e6edf3;
  }

  @media (max-width: 700px) {
    .go-page .go-layout {
      grid-template-columns: 1fr;
      gap: 1.75rem;
    }
  }

  @media (max-width: 575.98px) {
    .go-page .go-records a {
      display: block;
    }

    .go-page .go-records a::after {
      display: block;
      margin-top: 0.25rem;
    }
  }
</style>

<div class="go-page">
  <div class="go-layout">
    <div class="go-board-frame" aria-hidden="true">
      <div class="go-board">
        <span class="go-stone go-stone--black go-stone--one"></span>
        <span class="go-stone go-stone--white go-stone--two"></span>
        <span class="go-stone go-stone--black go-stone--three"></span>
        <span class="go-stone go-stone--white go-stone--four"></span>
        <span class="go-stone go-stone--black go-stone--five"></span>
      </div>
    </div>

    <div>
      <h2>Records</h2>
      <ul class="go-records">
        <li>
          <a href="https://119020.github.io/LGU-Go/awards.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener"><strong>awards</strong></a>
        </li>
        <li>
          <a href="https://119020.github.io/LGU-Go/history.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener"><strong>history</strong></a>
        </li>
        <li>
          <a href="https://119020.github.io/LGU-Go/records.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener"><strong>records</strong></a>
        </li>
      </ul>
    </div>

  </div>
</div>
