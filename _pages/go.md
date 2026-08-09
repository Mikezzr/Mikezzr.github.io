---
layout: page
permalink: /go/
nav: false
---

<style>
  body:has(.go-page) {
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
    --go-hover-bg: rgba(118, 84, 181, 0.12);
    background-color: #eef8ff;
    background-image:
      radial-gradient(ellipse 19rem 5.5rem at 9% 8%, rgba(255, 255, 255, 0.84) 0 44%, transparent 72%),
      radial-gradient(ellipse 15rem 4.5rem at 24% 14%, rgba(255, 255, 255, 0.68) 0 42%, transparent 72%),
      radial-gradient(ellipse 21rem 6rem at 83% 18%, rgba(255, 255, 255, 0.75) 0 40%, transparent 72%),
      linear-gradient(180deg, #d9efff 0%, #edf8ff 42%, #ffffff 100%);
    background-attachment: fixed;
  }

  html[data-theme='dark'] body:has(.go-page) {
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
    --go-hover-bg: rgba(200, 182, 239, 0.14);
    background-color: #101d29;
    background-image:
      radial-gradient(ellipse 19rem 5.5rem at 9% 8%, rgba(147, 194, 229, 0.16) 0 44%, transparent 72%),
      radial-gradient(ellipse 15rem 4.5rem at 24% 14%, rgba(147, 194, 229, 0.12) 0 42%, transparent 72%),
      radial-gradient(ellipse 21rem 6rem at 83% 18%, rgba(147, 194, 229, 0.14) 0 40%, transparent 72%),
      linear-gradient(180deg, #122b40 0%, #101d29 55%, #0d151d 100%);
  }

  body:has(.go-page) #navbar,
  body:has(.go-page) .navbar {
    border-bottom: 1px solid var(--site-line);
    background: rgba(222, 239, 255, 0.72) !important;
    backdrop-filter: blur(12px);
  }

  html[data-theme='dark'] body:has(.go-page) #navbar,
  html[data-theme='dark'] body:has(.go-page) .navbar {
    border-bottom-color: var(--site-line);
    background: rgba(20, 30, 46, 0.74) !important;
  }

  body:has(.go-page) #navbar a:hover,
  body:has(.go-page) .navbar a:hover {
    border-radius: 0.25rem;
    background-color: rgba(118, 84, 181, 0.14) !important;
    color: var(--site-link-hover) !important;
  }

  .go-page {
    --go-ink: var(--site-ink);
    --go-accent: var(--site-link);
    position: relative;
    isolation: isolate;
    min-height: clamp(28rem, 64vh, 44rem);
    margin: 0.75rem 0 1rem;
    border: 0;
    background: transparent;
    color: var(--go-ink);
    box-shadow: none;
  }

  .go-page .go-layout {
    position: relative;
    z-index: 1;
    display: flex;
    min-height: inherit;
    align-items: center;
    padding: clamp(1rem, 4vw, 3.5rem) 0;
  }

  .go-page .go-nav {
    width: 100%;
    max-width: 980px;
    margin: 0 auto;
    border-top: 1px solid var(--site-line);
    border-bottom: 1px solid var(--site-line);
    background: rgba(248, 251, 255, 0.52);
    padding: clamp(0.75rem, 2.2vw, 1.25rem) 0;
    box-shadow: 0 1.5rem 3rem rgba(68, 53, 105, 0.12);
    backdrop-filter: blur(8px);
  }

  .go-page .go-records {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 0;
    margin: 0;
    padding: 0;
    list-style: none;
    counter-reset: go-record;
  }

  .go-page .go-records li {
    counter-increment: go-record;
    border-left: 1px solid var(--site-line);
    padding: 1.35rem clamp(1.15rem, 3vw, 2.4rem) 1.5rem;
    transition: background-color 160ms ease, color 160ms ease;
  }

  .go-page .go-records li:hover {
    background: var(--go-hover-bg);
  }

  .go-page .go-records li:first-child {
    border-left: 0;
  }

  .go-page .go-records li::before {
    display: block;
    content: '0' counter(go-record) ' /';
    color: var(--go-accent);
    font-size: 0.78rem;
    font-weight: 700;
    letter-spacing: 0.08em;
  }

  .go-page .go-records a {
    display: flex;
    min-height: 10rem;
    flex-direction: column;
    justify-content: space-between;
    gap: 1.5rem;
    padding-top: 0.9rem;
    text-decoration: none;
  }

  .go-page .go-records strong {
    color: var(--go-ink);
    font-size: clamp(1.8rem, 4vw, 3rem);
    letter-spacing: 0.01em;
  }

  .go-page .go-records a::after {
    align-self: flex-end;
    content: '\2197';
    color: var(--go-accent);
    font-size: 1.35rem;
    transition: transform 160ms ease;
  }

  .go-page .go-records a:hover::after {
    transform: translateX(0.3rem);
  }

  .go-page .go-records a:hover strong {
    color: var(--go-accent);
  }

  html[data-theme='dark'] .go-page .go-nav {
    border-top-color: var(--site-line);
    border-bottom-color: var(--site-line);
    background: rgba(20, 30, 46, 0.54);
  }

  html[data-theme='dark'] .go-page .go-records li {
    border-left-color: var(--site-line);
  }

  @media (max-width: 700px) {
    .go-page {
      min-height: 30rem;
    }

    .go-page .go-layout {
      min-height: inherit;
      padding: 1rem 0;
    }

    .go-page .go-records {
      grid-template-columns: 1fr;
      gap: 1rem;
    }

    .go-page .go-records li,
    .go-page .go-records li:first-child {
      border-top: 1px solid var(--site-line);
      border-left: 0;
      padding: 1rem 1.1rem 1.1rem;
    }

    .go-page .go-records li:first-child {
      border-top: 0;
      padding-top: 0.5rem;
    }

    .go-page .go-records a {
      min-height: 6rem;
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
