# 1,200 Months

A life calendar plugin for [TRMNL](https://trmnl.com) e-ink displays. Each dot is one month. Each row is four years. One hundred years on a single screen.

![TRMNL e-ink display](https://img.shields.io/badge/TRMNL-e--ink-black)

## Concept

Inspired by Oliver Burkeman's *Four Thousand Weeks* and Tim Urban's [Your Life in Weeks](https://waitbutwhy.com/2014/05/life-weeks.html). The idea is simple: seeing your entire life as a finite grid of dots makes time tangible.

- **Black dots** — months you've lived
- **Ring dot** — the month you're in right now
- **Gray dots** — months remaining

## Layout

- **48 columns × 25 rows** = 1,200 dots (100 years)
- Compact header with month count, progress bar, and current position
- Age labels every 10 years along the left edge
- Optimized for 800×480 e-ink (TRMNL OG) and 1040×780 (TRMNL V2)

## Configuration

Edit the birth date at the top of the `<script>` block in `index.html`:

```js
var BIRTH_DATE = '1976-04-11';  // YYYY-MM-DD
```

For the TRMNL recipe editor, replace with a template variable:

```js
var BIRTH_DATE = '{{ birth_date }}';
```

Then add a `birth_date` setting (text, YYYY-MM-DD format) in your recipe configuration.

## Typography

- **Instrument Serif** — title
- **IBM Plex Mono** — stats and labels

## Credits

- [Four Thousand Weeks](https://www.oliverburkeman.com/books) by Oliver Burkeman
- [Your Life in Weeks](https://waitbutwhy.com/2014/05/life-weeks.html) by Tim Urban / Wait But Why
- [TRMNL](https://trmnl.com) e-ink display platform
