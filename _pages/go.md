---
layout: page
permalink: /go/
nav: false
---

<style>
  .go-page {
    --go-ink: #263746;
    --go-accent: #176b78;
    position: relative;
    isolation: isolate;
    min-height: clamp(36rem, 76vh, 52rem);
    overflow: hidden;
    margin: 0.5rem 0 1rem;
    border: 1px solid rgba(38, 55, 70, 0.16);
    border-radius: 1rem;
    background: #e9dfcc;
    color: var(--go-ink);
    box-shadow: 0 1.25rem 3rem rgba(38, 55, 70, 0.15);
  }

  .go-page::before {
    position: absolute;
    z-index: 0;
    inset: 0;
    background-image: url('{{ "/assets/img/go.png" | relative_url }}');
    background-position: center;
    background-size: cover;
    content: '';
    filter: saturate(0.65) contrast(0.9);
    opacity: 0.26;
    transform: scale(1.035);
  }

  .go-page::after {
    position: absolute;
    z-index: 0;
    inset: 0;
    background: linear-gradient(180deg, rgba(255, 252, 244, 0.12), rgba(255, 252, 244, 0.56));
    content: '';
    pointer-events: none;
  }

  .go-page .go-layout {
    position: relative;
    z-index: 1;
    display: flex;
    min-height: inherit;
    align-items: flex-end;
    padding: clamp(1rem, 4vw, 3.5rem);
  }

  .go-page .go-nav {
    width: 100%;
    max-width: 960px;
    margin: 0 auto;
    border: 1px solid rgba(38, 55, 70, 0.2);
    border-top: 6px solid var(--go-accent);
    background: rgba(255, 255, 255, 0.86);
    padding: clamp(1.35rem, 3.2vw, 2.6rem);
    box-shadow: 0 1rem 2.5rem rgba(39, 49, 58, 0.2);
    backdrop-filter: blur(4px);
  }

  .go-page .go-records {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 1rem;
    margin: 0;
    padding: 0;
    list-style: none;
    counter-reset: go-record;
  }

  .go-page .go-records li {
    counter-increment: go-record;
    border: 1px solid rgba(38, 55, 70, 0.16);
    border-top: 3px solid rgba(23, 107, 120, 0.42);
    background: rgba(255, 255, 255, 0.56);
    padding: 1.1rem 1.2rem 1.25rem;
    transition: transform 160ms ease, border-color 160ms ease, background-color 160ms ease;
  }

  .go-page .go-records li:hover {
    border-color: var(--go-accent);
    background: rgba(255, 255, 255, 0.8);
    transform: translateY(-0.35rem);
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
    min-height: 8.5rem;
    flex-direction: column;
    justify-content: space-between;
    gap: 1.2rem;
    padding-top: 0.6rem;
  }

  .go-page .go-records strong {
    color: var(--go-ink);
    font-size: clamp(1.7rem, 3.8vw, 2.6rem);
    letter-spacing: 0.02em;
  }

  .go-page .go-records a::after {
    align-self: flex-end;
    content: '->';
    color: var(--go-accent);
    font-size: 1.5rem;
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
    background: #26343d;
  }

  html[data-theme='dark'] .go-page .go-nav {
    background: rgba(24, 35, 44, 0.9);
  }

  html[data-theme='dark'] .go-page .go-records li {
    border-color: #506068;
    background: rgba(24, 35, 44, 0.64);
  }

  @media (max-width: 700px) {
    .go-page {
      min-height: 34rem;
    }

    .go-page .go-layout {
      min-height: inherit;
      padding: 1rem;
    }

    .go-page .go-records {
      grid-template-columns: 1fr;
      gap: 1rem;
    }

    .go-page .go-records li,
    .go-page .go-records li:first-child {
      border-top: 1px solid rgba(38, 55, 70, 0.16);
      padding: 0.9rem 0 0;
    }

    .go-page .go-records li:first-child {
      border-top: 0;
      padding-top: 0;
    }

    .go-page .go-records li {
      padding: 1rem 1.1rem 1.1rem;
    }

    .go-page .go-records a {
      min-height: 6.5rem;
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
