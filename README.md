# Unsolicited Deck Pics 🌲🐙🦊🦇

A free, browser-based tarot & oracle reading site featuring four original decks, built and illustrated by [G33KY](https://github.com/ad0rkableg33k). No sign-up, no app store, no nonsense — just open the page and pull cards.

**Live site:** https://ad0rkableg33k.github.io/Nightwood-Oracle/

---

## The Decks

| Deck | Cards | Vibe |
|---|---|---|
| 🌲 **Nightwood Oracle** | 20 | A forest divination deck — animal guides (Wolf, Owl, Firefly, Turtle, and more) delivering grounded, poetic wisdom. |
| 🐙 **Cutesy Chaos Tarot** | 78 | Full traditional tarot structure, reskinned with maximum chaos and zero chill. |
| 🐾 **Colorful Creatures Oracle** | 31 | Bright, playful animal-spirit cards (Dragon, Penguin, Lion, Bat, and more). |
| 🦇 **FangFluff Tarot** | 78 | A complete Major + Minor Arcana tarot deck with a gothic bat-and-shadow aesthetic. |

Switch decks anytime using the banner tiles at the top of the page — each deck has its own color theme, particle effects (fireflies for Nightwood, skulls for Cutesy Chaos, etc.), and card-back styling.

## Features

- **Multiple spread types per deck** — Single Card, Three Card, Five Card, and deck-specific spreads (Shadow & Light, Heart Check, Full Chaos Spread, and more).
- **Cross-deck combo spreads** — pull from two, three, or all four decks at once (e.g. "All Four Decks," "Tarot + Oracle," "FangFluff + Oracle") for readings that blend energies across the whole card library.
- **Reversed cards** — cards can pull upright or reversed, each with its own tag and meaning.
- **3D card flip animations** with a placeholder back for any card art that hasn't loaded yet.
- **Daily Horoscope section** — pick your zodiac sign for a deterministic, date-seeded daily reading (same sign + same day = same reading).
- **Export & share** — print/PDF export of your reading, plus share buttons for email, SMS, and Facebook, and a copy-link option.
- **Sticky nav bar** linking out to the other Unsolicited Deck Pics properties: Reality is Buffering (webcomic), Fancy Font Generator, Mizzverse, GitHub, and YouTube.

## Tech Notes

- Single-page, vanilla HTML/CSS/JS — no build step, no framework, hosted directly on GitHub Pages.
- Card data (names, keywords, meanings, file references) lives in per-deck JS arrays (`ORACLE_CARDS`-style objects) near the bottom of `index.html`.
- Spreads are defined per deck in dedicated arrays (`ORACLE_SPREADS`, `CUTESY_SPREADS`, `CC_SPREADS`, `FANGFLUFF_SPREADS`), with an `ORACLE_SPREADS_EXTRA` array for the multi-deck combo spreads.
- Deck switching is handled by a `setDeck()` function that swaps active banner state, theme classes on `<body>`, header text, and footer deck label.

## Contributing / Editing

This is a personal creative project — card art, copy, and site design are all original work by BabyyBat & G33KY. If you spot a bug or have a suggestion, open an issue on GitHub.

---

*Part of the [ad0rkableg33k](https://github.com/ad0rkableg33k) creative universe — see also [Reality is Buffering](https://ad0rkableg33k.github.io/realityisbuffering/) and the [Fancy Font Generator](https://ad0rkableg33k.github.io/FontGenerator.html).*
