# Vakantie-Directief 🛰️

Een taken-app in de stijl van een Imperiale agent-tablet, gebouwd voor de vakantieweek
**zaterdag 18 t/m zondag 26 juli 2026**. Dagorders, ongeplande directieven,
weekconformiteit en een VOLTOOID-stempel met terminal-blip bij het afvinken.

## Gebruik

- **Afvinken**: tik op het vinkvak links van een taak.
- **Bewerken / verplaatsen / wissen**: tik op de taak zelf — er opent een paneel
  waarin je omschrijving, dag en sector kunt aanpassen.
- **Nieuwe taak**: knop **+ DIRECTIEF** rechtsonder.
- **Backup**: menu **⋯** → exporteer of importeer je taken als JSON-bestand
  (handig om je lijst van telefoon naar PC te verhuizen).

Alle taken worden lokaal op het apparaat opgeslagen (localStorage) — er is geen
server en geen account nodig.

## Installeren als app

Open de site op je telefoon en kies:

- **Android / Chrome**: menu ⋮ → *App installeren* (of *Toevoegen aan startscherm*).
- **iPhone / Safari**: deelknop → *Zet op beginscherm*.

De app werkt daarna ook offline dankzij de service worker.

## Hosten via GitHub Pages

1. Push deze repo naar GitHub.
2. Ga naar **Settings → Pages**, kies *Deploy from a branch*, branch `main`, map `/ (root)`.
3. Na een minuut staat de app op `https://<gebruikersnaam>.github.io/<reponaam>/`.

## Structuur

| Bestand | Doel |
|---|---|
| `index.html` | De volledige app (HTML/CSS/JS, geen dependencies) |
| `manifest.webmanifest` | PWA-manifest voor installatie |
| `sw.js` | Service worker (offline cache) |
| `icon-*.png` | App-iconen |
