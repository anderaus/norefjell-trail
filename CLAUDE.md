# Norefjell Trail 22K — Treningsplan

Dette repoet inneholder en interaktiv treningsplan for Hoka Norefjell Trail 22K (20. juni 2026).
Vedlikeholdes av Claude Code. Live på https://norefjell-trail-plan.netlify.app

---

## Repo-struktur

```
norefjell-trail/
├── index.html                  # UI — endres sjelden
├── plan.json                   # Treningsdata — oppdateres av Claude
├── Norefjell_Trail_-_22K.gpx   # Løypefil — aldri endre
├── CLAUDE.md                   # Denne filen
├── netlify.toml                # Netlify-konfig (publish = ".")
└── README.md
```

**Arbeidsflyt:**
1. Gjør endringer i `plan.json` (og evt. `index.html`)
2. Commit og push: `git add . && git commit -m "beskrivelse" && git push`
3. Netlify deployer automatisk innen ~30 sekunder

---

## Løperprofil

| | |
|--|--|
| **Navn** | Anders |
| **Født** | 1978 (46–47 år på løpsdagen) |
| **Bosted** | Eiksmarka, Bærum (relativt flatt treningsområde) |
| **Primærsport** | Trail- og veiløping, 4 dager/uke |
| **Treningsdager** | Tirsdag, torsdag, lørdag, søndag |
| **Aktivitetslogg** | Garmin + Strava siden 2009 |

### Treningsdagenes rolle
- **Tirsdag** — Lett Z2-løp (restitusjon etter søndagens langtur)
- **Torsdag** — Intervalløkt med treningsgruppe på flat grusvei. Gruppen bestemmer type. Plan inneholder fallback-økt hvis gruppen avlyses.
- **Lørdag** — Kvalitetsøkt: bakkeintervaller, race-sim eller teknisk trail
- **Søndag** — Alltid langturen (viktigste dag i uka)

### Fysiologiske data (fra Strava-analyse, 274 aktiviteter)
- **LTHR:** 176 bpm (estimert fra 5km-løp apr 2025: 22:08, avg HR 174.6)
- **MaxHR:** 190 bpm (registrert i race juli 2024)
- **Grå-sone-problem:** Snitt-HR alle løp 2 år: 158,9 bpm (S3) — historisk for hardt på lette dager
- **Terskelfarr (flat):** ~4:40/km

### Treningssoner (Friel 7-sone, basert på LTHR 176)

| Sone | Navn | HR | Flat pace |
|------|------|----|-----------|
| S1 | Restitusjon | <143 | – |
| S2 | Aerob base | 143–157 | 5:30–6:10/km |
| S3 | Tempo | 158–164 | 4:50–5:05/km |
| S4 | Sub-terskel | 165–174 | 4:45–4:55/km |
| S5a | Terskel | 175–179 | 4:35–4:50/km |
| S5b | VO2maks | 180–186 | 4:10–4:25/km |

### Nøkkelresultater (referanseytelser)

| Løp | Dist | Stigning | Tid | Snitt HR | Merknad |
|-----|------|---------|-----|----------|---------|
| 5km Oslo Løpsfestival | 5,0km | +11m | 22:08 | 175 | Flat vei, fullt race-effort |
| Sørkedalsløpet | 10,8km | +311m | 63:44 | 173 | Trail, race-effort |
| Oslo Nightrun | 9,7km | +186m | 63:06 | 173 | Trail, race-effort |
| Ivar Formos Minneløp | 16,1km | +442m | 1:50:37 | 172 | Trail, race-effort |
| **Lommedalen Rundt** | **18,6km** | **+672m** | **2:09:21** | **167** | **Svært våte forhold** |
| Brunkollen (trening) | 19,3km | +358m | 1:51:47 | 158 | Treningstur, ikke race |

**Viktig om Lommedalen:** Løpt i svært våte forhold — tørr-ekvivalent estimert til ~1:59.
Dette er primærreferansen for Norefjell-prognosen.

---

## Målløp: Hoka Norefjell Trail 22K

**Dato:** 20. juni 2026  
**Distanse:** 22,45 km  
**Stigning:** 867m (GPX-analysert med 2m støyfilter)  
**Nedstigning:** 868m  
**Start/Slutt:** 789m over havet

### Løypeprofil (GPX-analysert, 662 trackpoints)

| Segment | Km | Stigning | Nedst. | Snittgradient | Nøkkelfakta |
|---------|-----|---------|--------|--------------|-------------|
| Inngang | 0–5 | +86m | -61m | +2,5% snitt | **FELLE:** reelt fall på ~50m ved km 4–5 (−4,8%) |
| Hoveddelen | 5–12 | +440m | -10m | +8,8% | Bratteste 500m: km 9,3 på +15,6%. Power-hike soner. |
| Toppplatå | 12–16 | +117m | -204m | Variabel | 6km over 1380m. Overraskende **motbakke ved km 16 (+2,3%)** |
| Overgang | 16–19 | +28m | -140m | −3,7% | Slak, løpbar nedstigning |
| Finale | 19–22,4 | +13m | -484m | **−13,1% snitt, opp til −24%** | Quadricepsdreperen |

**Topp:** 1458,6m ved km 12,3  
**Toppplatå:** km 10,5–16,4 (nesten 6km over 1380m)

### Tidsprognose

| | Tid |
|--|--|
| Optimistisk | 2:25–2:30 |
| **Realistisk** | **2:35–2:45** |
| Konservativt | 2:50–2:55 |

Basert på: Lommedalen tørr-ekvivalent + segmentvis GPX-estimat + 13 ukers spesifikk trening.

### Race-strategi sammendrag
1. **km 0–5:** HR <160, konservativt. Ikke bruk dalen ved km 4–5 til å hente inn tid.
2. **km 5–12:** HR 165–174. Power-hike alt over ~12%. Tre kjente power-hiking-soner.
3. **km 12–16:** Teknisk platå, variabel profil. Forbered deg på motbakken ved km 16.
4. **km 16–19:** Kontrollert rask nedstigning. Spar quads.
5. **km 19–22,4:** Teknisk bratt (-24% vinduer). Korte raske steg, len deg framover.
- **Gel:** km 7, km 13, km 18

---

## Treningsplan — struktur

**Periode:** 6. april – 20. juni 2026 (11 uker)  
**Faser:** Oppbygging (U1–3) → Restitusjonsuke (U4) → Spesifisitet (U5–7) → Restitusjonsuke (U8) → Toppuke (U9) → Nedtrapping (U10–11)

### Nøkkeløkter
- **U5 lørdag:** Vedvarende klatreøkt (2× 20–25min race-innsats oppover, Kolsåstoppen/Vettakollen)
- **U6 lørdag:** Race-simulering 15km +600m
- **U9 søndag:** Topptur 20km +700m (Norefjell-rekognosering anbefales)

### Lørdag/søndag-belastning — viktige hensyn (47 år, 4 dager/uke)
Noen par er justert for å beskytte mot overbelastning:
- **U5 søndag:** Lett 13km +80m flat (ikke 18km +380m) — etter hard klatrelørdag
- **U7 søndag:** 16km +200m (ikke 19km +420m) — tredje harde uke kumulativt
- **U9 lørdag:** 10km +80m flat (ikke 12km trail) — sett opp søndagens topptur

---

## `plan.json` — datastruktur

Hoved-datafilen. `index.html` fetcher den via `fetch('./plan.json')` ved lasting.

```
plan.json
├── version, meta
├── assessment          ← Løperprofil, styrker, begrensere
├── zones               ← HR-soner basert på LTHR 176
├── phases              ← Fasebeskrivelser
├── weeks[]             ← 11 uker
│   ├── weekNumber, phase, startDate, endDate
│   ├── focus           ← Ukas tema
│   ├── isRecoveryWeek
│   ├── days[]
│   │   ├── date, dayOfWeek (norsk: "Mandag" etc.)
│   │   └── workouts[]
│   │       ├── id      ← Format: "w{uke}-{dag}-{type}" f.eks. "w5-sat-climb"
│   │       ├── sport   ← "run" | "rest"
│   │       ├── type    ← "easy" | "hill_repeat" | "threshold" | "long" | "trail_medium" | "trail_easy" | "race_simulation" | "sustained_climb" | "fartlek" | "back_to_back" | "race" | "rest"
│   │       ├── name    ← Norsk navn på økten
│   │       ├── description   ← Fullstendig norsk beskrivelse
│   │       ├── durationMinutes
│   │       ├── distanceKm
│   │       ├── elevation     ← Stigning i meter
│   │       ├── primaryZone   ← f.eks. "Sone 2" eller "Sone 4 på drag, Sone 2 ellers"
│   │       ├── groupAlternative  ← Kun på torsdager: tekst om gruppetrening
│   │       └── completed     ← boolean, settes av brukeren i UI
│   └── summary.bySport.run{sessions, hours, km, elev}
├── coachingNotes       ← 4 nøkkelproblemer med fix-anbefalinger
└── raceStrategy        ← GPX-basert segmentvis strategi, ernæring, utstyr
```

**Dagenavn er alltid på norsk:** Mandag, Tirsdag, Onsdag, Torsdag, Fredag, Lørdag, Søndag  
**Fasenavn er alltid på norsk:** Oppbygging, Restitusjonsuke, Spesifisitet, Toppuke, Nedtrapping  
**Alt innhold i plan.json er på norsk.**

---

## Coaching-prinsipper (fra coach-skill)

1. **Konsistens over heroisme** — Jevn trening slår sporadiske stormøkter
2. **Lette dager lett, harde dager harde** — Grå-sone-trening gir dårligst utbytte
3. **Respekter restitusjon** — Form bygges i hvile, ikke i treningsøkter
4. **Polarisert intensitet** — ~80% av volum i S1–2, ~20% i S4–5
5. **Spesifisitet øker over tid** — Tidlig generelt, sent løpsspesifikt
6. **Taper tilstrekkelig** — De fleste taper for lite; stol på formen
7. **Aldershensyn (47 år)** — Masters-løpere trenger ~25–35% mer restitusjonstid mellom harde økter
8. **Power-hiking er en ferdighet** — Øv det i trening; det er raskere enn treg jogging på >20% gradient

### Norefjell-spesifikke prinsipper
- Bakkespesifikk trening må hentes på Kolsåstoppen, Vettakollen, Lysakerelva eller Krokskogen
- Quadriceps excentrisk styrke er kritisk for finalefallets -24%-gradienter
- Torsdag-intervaller er på flat grusvei (gruppe) — løypespesifikk bakketrening skjer lørdag

---

## `index.html` — UI-oversikt

Statisk HTML/CSS/JS-fil. Laster `plan.json` asynkront. Struktur:

- **5 faner:** Treningsplan | Analyse | Soner | Race Strategy | Coaching-notater
- **Treningsplan-fanen:** Fase-tidslinje + utfoldbare ukekort generert fra `plan.json`
- **Race Strategy-fanen:** GPX-generert høydeprofil SVG (200 datapunkter, smoothet) + segmentkort
- **Fargetema:** Mørk bakgrunn (#1c1a17), Strava-oransje (#d95f2b), teal (#2a8a7f)
- **Fonter:** Playfair Display (headings), DM Mono (data), DM Sans (brødtekst)
- **Fullført-tilstand** lagres i `localStorage` under nøkkel `'norefjell-done'`

Fasereferanser i JS bruker norske navn (må stemme med `plan.json`):
```js
'Oppbygging': 'phase-build'
'Restitusjonsuke': 'phase-recovery'
'Spesifisitet': 'phase-specificity'
'Toppuke': 'phase-peak'
'Nedtrapping': 'phase-taper'
```

Workout-typer som rendres med fargekoder: `rest`, `easy`, `hill_repeat`, `tempo`, `threshold`, `long`, `trail_medium`, `trail_easy`, `race`, `fartlek`, `race_simulation`, `sustained_climb`, `back_to_back`

---

## GPX-fil

`Norefjell_Trail_-_22K.gpx` — aldri endre denne filen.

Parse med Python:
```python
import xml.etree.ElementTree as ET
import math

def haversine(lat1, lon1, lat2, lon2):
    R = 6371000
    phi1, phi2 = math.radians(lat1), math.radians(lat2)
    a = math.sin((phi2-phi1)/2)**2 + math.cos(phi1)*math.cos(phi2)*math.sin((math.radians(lon2-lon1))/2)**2
    return 2 * R * math.asin(math.sqrt(a))

tree = ET.parse('Norefjell_Trail_-_22K.gpx')
ns = {'gpx': 'http://www.topografix.com/GPX/1/1'}
points = [(float(pt.get('lat')), float(pt.get('lon')), float(pt.find('gpx:ele', ns).text))
          for pt in tree.getroot().findall('.//gpx:trkpt', ns)]
```

---

## Netlify

- **Site ID:** `09e89b54-ddc8-4ed1-aafe-c6e0e00d652e`
- **Site navn:** `norefjell-trail-plan`
- **URL:** https://norefjell-trail-plan.netlify.app
- **GitHub repo:** https://github.com/anderaus/norefjell-trail
- **Deploy:** Automatisk ved push til `main`
- **Build command:** (ingen — statisk site)
- **Publish directory:** `.`

Deploy manuelt ved behov:
```bash
netlify deploy --prod --dir . --site 09e89b54-ddc8-4ed1-aafe-c6e0e00d652e
```
