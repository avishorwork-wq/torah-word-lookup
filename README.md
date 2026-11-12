# Torah Word Lookup

A single-page word lookup for Shas (Gemara), Chumash, and Rashi on Chumash.
Type or paste a Hebrew/Aramaic word and get an instant offline gloss, plus
dictionary entries from Sefaria (Jastrow, BDB, and more) when online.

Based on the original `GemaraLookup.html` (Gemara words only). This version adds
the full Chumash and Rashi-on-Chumash word lists.

## Data

- `index.html` - the app, including the built-in Shas quick-gloss list (37,607 words).
- `data-chumash.js` - 12,840 unique Chumash words: occurrences, translation, grammatical form, source, confidence, example verse.
- `data-rashi.js` - 29,415 unique Rashi-on-Chumash words, same format.

The Chumash and Rashi lists come from the "Mefarshei HaOtzar - Chumash & Rashi
Word Lists" Google Sheet (built 2026-11-12). Every row keeps its own source and
confidence label from the sheet (e.g. "BDB via OSHB lemma", "Jastrow",
"AI-written, unverified"). Rows that could not be read confidently say
"uncertain; see context" rather than a guess. This is a study aid, not a
checked sefer - verify against the text before relying on a gloss.

## Running

It is a static site: open `index.html` or serve the folder. Hosted with GitHub Pages.
