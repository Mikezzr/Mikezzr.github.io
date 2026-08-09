---
layout: page
permalink: /go/
nav: false
---

<style>
  .go-page {
    --go-ink: #27313a;
    --go-accent: #0f766e;
    position: relative;
    isolation: isolate;
    min-height: 26rem;
    overflow: hidden;
    margin-top: 1.5rem;
    background: #f1e5cf;
    color: var(--go-ink);
  }

  .go-page::before {
    position: absolute;
    z-index: 0;
    inset: 0;
    background-image: url('{{ "/assets/img/go.png" | relative_url }}');
    background-position: center;
    background-size: cover;
    content: '';
    filter: saturate(0.65) contrast(0.92);
    opacity: 0.16;
  }

  .go-page .go-layout {
    position: relative;
    z-index: 1;
    display: flex;
    min-height: 26rem;
    align-items: flex-end;
    padding: 2rem;
  }

  .go-page .go-nav {
    width: 100%;
    border-top: 4px solid var(--go-accent);
    background: rgba(255, 255, 255, 0.91);
    padding: 1.25rem 1.5rem 1.35rem;
    box-shadow: 0 0.75rem 2rem rgba(39, 49, 58, 0.14);
  }

  .go-page .go-records {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    margin: 0;
    padding: 0;
    list-style: none;
    counter-reset: go-record;
  }

  .go-page .go-records li {
    counter-increment: go-record;
    border-left: 1px solid #c7d0d0;
    padding: 0 1rem;
  }

  .go-page .go-records li:first-child {
    border-left: 0;
    padding-left: 0;
  }

  .go-page .go-records li::before {
    display: block;
    content: '0' counter(go-record);
    color: var(--go-accent);
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.08em;
  }

  .go-page .go-records a {
    display: flex;
    min-height: 4.5rem;
    flex-direction: column;
    justify-content: space-between;
    gap: 0.75rem;
    padding-top: 0.35rem;
  }

  .go-page .go-records strong {
    color: var(--go-ink);
    font-size: 1.45rem;
    letter-spacing: 0.03em;
  }

  .go-page .go-records a::after {
    align-self: flex-end;
    content: '->';
    color: var(--go-accent);
    font-size: 1.15rem;
    transition: transform 160ms ease;
  }

  .go-page .go-records a:hover::after {
    transform: translateX(0.3rem);
  }

  .go-page .go-records a:hover strong {
    color: var(--go-accent);
  }

  html[data-theme='dark'] .go-page {
    --go-ink: #e6edf3;
    background: #283238;
  }

  html[data-theme='dark'] .go-page .go-nav {
    background: rgba(24, 35, 44, 0.92);
  }

  html[data-theme='dark'] .go-page .go-records li {
    border-left-color: #506068;
  }

  @media (max-width: 700px) {
    .go-page {
      min-height: 30rem;
    }

    .go-page .go-layout {
      min-height: 30rem;
      padding: 1rem;
    }

    .go-page .go-records {
      grid-template-columns: 1fr;
      gap: 1rem;
    }

    .go-page .go-records li,
    .go-page .go-records li:first-child {
      border-top: 1px solid #c7d0d0;
      border-left: 0;
      padding: 0.9rem 0 0;
    }

    .go-page .go-records li:first-child {
      border-top: 0;
      padding-top: 0;
    }
  }
</style>

<div class="go-page">
  <div class="go-layout">
    <nav class="go-nav" aria-label="Go records">
      <ul class="go-records">
        <li>
          <a href="https://119020.github.io/LGU-Go/awards.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener"><strong>Awards</strong></a>
        </li>
        <li>
          <a href="https://119020.github.io/LGU-Go/history.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener"><strong>History</strong></a>
        </li>
        <li>
          <a href="https://119020.github.io/LGU-Go/records.html?player_id=2&amp;player_name=%E6%9B%BE%E5%AD%90%E8%8D%A3" target="_blank" rel="noopener"><strong>Records</strong></a>
        </li>
      </ul>
    </nav>
  </div>
</div>
