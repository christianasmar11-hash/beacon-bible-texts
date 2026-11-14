# Beacon Bible texts

Public-domain and openly licensed Bible texts for [Beacon Bible](https://beacon-bible.com), hosted as static JSON for verse lookup.

This repository is a data library. It is not the Beacon Bible application.

## Base URL

https://christianasmar11-hash.github.io/beacon-bible-texts

## Layout

- `https://christianasmar11-hash.github.io/beacon-bible-texts/index.json` — every translation (`code`, `name`, `language`, `languageName`, `license`, `attribution`, `sourceUrl`, `psalmNumbering`)
- `https://christianasmar11-hash.github.io/beacon-bible-texts/books.json` — 66 English book names, Spanish names, and common abbreviations
- `https://christianasmar11-hash.github.io/beacon-bible-texts/<CODE>/<book_number>.json` — one book, for example `https://christianasmar11-hash.github.io/beacon-bible-texts/KJV/43.json` for John in the King James Version
- `https://christianasmar11-hash.github.io/beacon-bible-texts/LICENSES.md` — licenses and required attribution

`psalmNumbering` is `hebrew` for most editions and `vulgate` for Douay-Rheims (DRA), the Clementine Vulgate (VUC), and the Russian Synodal (SYN). In those three, the shepherd psalm is Psalm 22:1.

Book JSON shape:

```json
{
  "book": "John",
  "chapters": {
    "3": {
      "16": "For God so loved the world..."
    }
  }
}
```

See `LICENSES.md` before redistributing a Creative Commons text.
