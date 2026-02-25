# PL-DCD-GENERATOR

Desktop-app om snel een **Data Collection Document (DCD)** en bijbehorende documenten te genereren op basis van gestructureerde input.  
Deze repository bevat **alleen releases (installers)**, geen broncode.

> Let op: huidige builds zijn voor **macOS (Apple Silicon)**. Windows-builds volgen later.

---

## Download

- **Laatste versie:**  
  [Download via de GitHub Releases-pagina](https://github.com/postlounge/PL-DCD-GENERATOR-RELEASES/releases/latest)

Op de Releases-pagina vind je per versie o.a.:

- `DCD Generator-x.y.z-arm64.dmg` – installer voor macOS (Apple Silicon)
- `DCD Generator-x.y.z-arm64.zip` – dezelfde app als zip, voor handmatige installatie


---

## Platform & systeemvereisten

### macOS

- Apple Silicon (M1/M2/M3) – arm64 build
- macOS 12 (Monterey) of hoger aanbevolen

> Intel-Mac ondersteuning en Windows-builds staan op de roadmap.

---

## Installatie (macOS)

1. Ga naar de [laatste release](https://github.com/postlounge/PL-DCD-GENERATOR-RELEASES/releases/latest)
2. Download de `DCD Generator-…-arm64.dmg`.
3. Open het `.dmg`-bestand.
4. Sleep **DCD Generator** naar de map **Applications**.
5. Open de app vanuit **Applications**.
   - Bij de eerste keer openen kan macOS melden dat de app van een “niet-geïdentificeerde ontwikkelaar” komt.
   - In dat geval:
     - Ctrl-klik op de app → **Open** → nogmaals **Open**.
     - Daarna kun je de app normaal starten.

---

## Gebruik (korte uitleg)

Na het starten van de app:

1. Je komt op het **startscherm** met keuze voor:
   - **Datasheet / DCD** – Data Collection Document generator
   - **Data calculator** – bitrate en opslagcalculaties
   - **Conversie** – conversie-sheet (andere layout, zelfde onderliggende data)
2. Kies het gewenste onderdeel en vul de velden in (codec, resolutie, framerate, aantal camera-units, etc.).
3. De app rekent automatisch:
   - opslag per uur,
   - totale opslag,
   - opslag op locatie (DIT/DLO caps),
   - overige benodigde parameters.
4. Kies **Generate PDF** om een PDF te maken, of exporteer de parameters als JSON.

---

## Automatische update-melding

De app checkt bij het opstarten of er een **nieuwere versie** beschikbaar is op deze release-repo:

- De app leest de eigen versie (bijv. `0.1.0`).
- Hij vraagt via de GitHub API de **latest release tag** van deze repo op (bijv. `v0.2.0`).
- Als er een nieuwere versie is, verschijnt er een popup met de vraag of je naar de nieuwe release-pagina wilt gaan.

Zorg dus dat:

- Elke nieuwe versie hier als **GitHub Release** wordt gepubliceerd.
- De release-tag (bijv. `v0.2.0`) netjes oploopt t.o.v. de vorige versie.

---

## Versiebeheer & changelog

- Deze repo gebruikt semver-achtige tags, bijv. `v0.1.0`, `v0.2.0`, …
- Release notes per versie staan bij de betreffende **GitHub Release**.

---

## Feedback & contact

Heb je vragen, suggesties of bugs gevonden?

- Maak een issue aan in deze release-repo of
- Neem direct contact op met de auteur: **Sonny Tundo**.
