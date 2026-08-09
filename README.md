# Arie's laatste bus 🚌

Een klein, rustig plekje op internet met een overzicht van alle plekken waar Arie is uitgestrooid — met een kaart en per plek een herinnering.

## Een plek toevoegen of aanpassen

Alles staat in één bestand: **`plekken.js`**. Bovenin dat bestand staat stap voor stap uitgelegd hoe je een plek toevoegt. Kort samengevat:

1. Open `plekken.js` (dat kan direct op github.com: klik op het bestand en dan op het potloodje ✏️).
2. Kopieer een bestaand blok tussen `{` en `},` en plak het onderaan de lijst.
3. Vul de naam, plaats, datum, coördinaten en een herinnering in.
4. Sla op ("Commit changes") — de site wordt vanzelf bijgewerkt.

Coördinaten vinden: zoek de plek op Google Maps, klik met de rechtermuisknop op de plek en klik op de coördinaten om ze te kopiëren.

## Een foto toevoegen

1. Zet de foto in de map `fotos/` (op github.com: open de map en kies "Add file" → "Upload files").
2. Vul in `plekken.js` bij die plek de bestandsnaam in, bijvoorbeeld: `foto: "fotos/kleve.jpg"`.

Zonder foto ziet het kaartje er ook gewoon netjes uit.

## De site online zetten (eenmalig)

De site draait gratis via GitHub Pages:

1. Ga naar deze repository op github.com.
2. Klik op **Settings** → **Pages** (in het linkermenu).
3. Kies bij "Build and deployment" → Source: **Deploy from a branch**, en kies de branch **main** (map: `/ (root)`).
4. Klik op **Save**. Na een paar minuten staat de site op:

   **https://mdevree.github.io/Laatste-bus/**

Die link kun je delen met familie; de site werkt op telefoon, tablet en computer.

## Techniek

Bewust zo simpel mogelijk: één HTML-pagina, geen frameworks, geen build-stap. De kaart is [Leaflet](https://leafletjs.com) (meegeleverd in de map `leaflet/`) met [OpenStreetMap](https://www.openstreetmap.org)-kaarten — gratis en zonder API-sleutel.
