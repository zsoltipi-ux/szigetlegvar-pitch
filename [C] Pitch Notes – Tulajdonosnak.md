---
created: 2026-05-09
type: pitch-notes
audience: Zsolt-only
---

# Szigetlégvár — Pitch jegyzet (csak nekem)

## Mi van az oldalon

Két fájl, egy mappában (`02 Projects/Szigetlégvár – Pitch/`):

- **`index.html`** — modern demo landing oldal a Szigetlégvárnak. Foglalási rendszerrel, naptárral, chat widgettel, tulajdonosi nézettel. Ez az, amit a tulajnak megmutatok mint "ezt építem neked".
- **`ajanlat.html`** — sales pitch oldal Krisztiánnak (a tulajdonosnak). Mit tud a rendszer, hogyan spórol időt, csomagok és árak. A landing tetején lévő banner ide visz.

Mindkettő áll, képek (`img/`) helyileg vannak letöltve a szigetlegvar.hu-ról — saját képei, így "magát ismeri fel" rajta.

## Mit építettem be (gyors checklist)

- ✅ Valós idejű foglalási naptár (foglalt napok pirossal, kiválasztott napok aranyban)
- ✅ Szűrhető katalógus 13 légvárral, valódi képekkel
- ✅ 4 lépéses foglaló wizard (Naptár → Légvár → Extrák → Kontakt)
- ✅ Automata árszámítás (vár + 2 napos kedvezmény + km×240 + extrák + kaució)
- ✅ Extrák: vattacukor, popcorn, hangosítás, animátor, sátor, generátor
- ✅ **Beépített chat widget** keyword-alapú Q&A-val (~17 témakör), pulzáló FAB, suggested kérdések
- ✅ "Tulajdonosi nézet" preview szekció (mit lát csak ő — napi foglalások, heti forgalom, melyik vár mennyire foglalt)
- ✅ FAQ, vélemények, mobil sticky CTA, demo banner ami az ajánlatra visz
- ✅ Ajanlat.html: hero + 6 problem card + 9 feature card + before/after szombat-reggel összehasonlítás + 6 vevői benefit + 2 csomag pricing + ROI math + 7 FAQ + final CTA

## Csomagok és árak (amit ráírtam)

**Indító — 9 900 Ft / hó** (vagy 99 000 Ft / év — 2 hó kedvezmény)
- Foglaló + naptár + email visszaigazolás + chat (FAQ-alapú) + tulajdonosi nézet + hosting/SSL/domain

**Profi — 19 900 Ft / hó** (vagy 199 000 Ft / év)
- Minden + SMS visszaigazolás (50/hó) + 24h előtti SMS emlékeztető + Barion online fizetés + Google Calendar szinkron + élő AI chat (Claude alapú) + havi forgalmi riport + telefonos support

**Setup egyszer**: 79 000 Ft. **Akció:** 12 hónapos szerződésnél a setup ingyen.

**ROI érv**: Egy plusz foglalás havonta már megtéríti a Profi havidíjat. Reális becslés 3–8/hó plusz foglalás (este 8 utáni online vevők).

## Kontakt amit a Szigetlégvár oldalán találtam

- Email: szeak87@gmail.com
- Telefon: +36 70 246 5464
- Krisztián a tulaj (a chatbe is így tettem be)
- Szigetszentmiklós, 50 km-es körzet

## Mit nem tudok még / pontosítani kell ha komoly lesz

- A tulaj **valódi nevét** nem találtam, csak hogy Krisztián. A chatben és az ajanlat.html hero-ban "Krisztiánnak" szólítom — ha másnak szól, át kell írni.
- **Saját telefonszámomat** nem tettem be az ajanlat.html-be (helyettesítettem `+36 30 ...`-zel) — pótolni kell, mielőtt elküldöm neki.
- **Szállítási területek**: 50 km-et írtam, de pontos lista (mely városok) nincs. Igazából elég is így.
- **Légvárszámok** és technikai paramétereket az `/ugralovarak/` aloldal alapján vettem át — ha bármi változik, frissíteni kell.
- A **tulajdonosi nézet** csak vizuális preview, valódi backend nincs mögötte. Ha eladjuk, ez igazi adminra cserélődik.

## Hogyan adom el — pitch flow

1. **Megkeresés** — email vagy Messenger neki, "csináltam egy demót, nézd meg":
   - Subject: "Demo: modern foglalórendszer a Szigetlégvárnak"
   - Body: 3-4 sor: ki vagyok, mit építettem, link a demóra (ajanlat.html-re), kérek 20 perc hívást ha érdekes.
2. **Demo URL-eket élesíteni kell** (most csak helyi fájlok). Lehet GitHub Pages, Netlify, Vercel — bármi ingyenes static hosting. Egy kattintásból.
3. **Hívás** ha érdekli — végigvezetem a demón, megkérdezem mennyi foglalása van havonta, mennyi időt tölt foglalásokkal, és hogy ezek a számok stimmelnek-e a fájdalompontokkal amiket írtam.
4. **Záróhúzó:** "Kipróbáljuk 1 hónapot a setup-fee nélkül? Ha a havonta lefoglalt összeg nem nő, visszamondjuk." — ha bizonytalan.

## Élesítés — mi kell ha igent mond

- Domain: szigetlegvar.hu marad — DNS-re hozzáférés (cnamekkel rámegyünk a hostingunkra), VAGY a Wix oldalt lecseréljük (kell admin login a Webnodehoz / ami most van).
- Email-küldés: SendGrid / Resend ingyenes tier (100 email/nap bőven elég)
- SMS: Vatera / Twilio EU régió, kb. 10 Ft/SMS, 50/hó belefér a Profi havidíjba
- Barion online fizetés (Profi csomagban): 1.5% + 30 Ft tranzakciós díj — neki ez plusz költség, de a megrendelők szeretik
- Google Calendar API: ingyenes, ~30 perc setup
- AI chat élővé tétele: Claude API, kb. 1-2 USD / havonta a tipikus kérdésszámra

## Hosszú távú lehetőség

Ha jól megy ez vele, ezt a foglalórendszert tudom **ugrálóvár-bérlőknek általánosan** is áruba bocsátani — Magyarországon kb. 50-100 ilyen vállalkozás van. Ha mindegyik 19 900 Ft / hó × ~30 vevő = ~600 e Ft / hó MRR. Ez egy önálló SaaS lehetőség lenne mellékprojektnek (egy kódbázis, vevőnként sub-domain + saját tartalom).
