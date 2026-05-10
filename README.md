# Szigetlégvár — Modern foglalórendszer (demo)

Modern foglalási weboldal a [szigetlegvar.hu](https://www.szigetlegvar.hu/) számára — élő naptárral, automata árszámítással, beépített chat-tel, és tulajdonosi nézettel.

## Tartalom

- **`index.html`** — modern landing oldal a vevőknek (foglalórendszer, chat widget, katalógus, FAQ)
- **`ajanlat.html`** — sales pitch a tulajdonosnak (Ákosnak): mit tud a rendszer, hogyan spórol időt, csomagok és árak
- **`img/`** — légvár-fotók a meglévő weboldalról

## Demo

Helyileg megnyitható: `python3 -m http.server 8766` majd [http://localhost:8766](http://localhost:8766).

GitHub Pages-en is futtatható — repo Settings → Pages → Branch: `main` → `/` (root).

## Stack

Egyszerű statikus HTML/CSS/JS — semmi build, semmi framework, semmi dependency. Sigmar One + Manrope a Google Fonts-ról (mindkettő teljes magyar karakter-támogatással, beleértve az Ő/ő/Ű/ű glyph-eket — fonttools-szal verifikálva).

## Készítette

Pintér Zsolt — zsoltipi@gmail.com
