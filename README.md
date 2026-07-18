# Vacation Directive 🛰️

Een taken-app in de stijl van een Imperiale agent-tablet (UI in sci-fi Engels),
gebouwd voor de vakantieweek **zaterdag 18 t/m zondag 26 juli 2026**. Daily orders,
unassigned directives, weekly compliance en een COMPLETE-stempel met terminal-blip
bij het afvinken.

## Gebruik

- **Afvinken**: tik op het vinkvak links van een taak. Is de hele dag af, dan
  verschijnt een **SECTOR SECURED**-stempel over het scherm.
- **Bewerken / verplaatsen / wissen**: tik op de taak zelf — er opent een paneel
  waarin je omschrijving, dag en sector kunt aanpassen. Na wissen kun je 5 seconden
  op **Undo** tikken.
- **Snel inplannen**: ongeplande taken hebben knopjes **▸ Today** / **▸ Tmrw**.
- **Weergaven**: schakel tussen **List** (één dag + backlog) en **Board** (alle dagen
  als kolommen naast elkaar, Trello-stijl). Op het bord kun je taken tussen dagen
  **slepen** (desktop).
- **Snel toevoegen**: onderaan elke lijst of kolom zit een invoerveldje — typen,
  Enter, klaar.
- **Doorschuiven**: onafgemaakte taken van eerdere dagen geven een waarschuwing
  bovenaan met één knop om ze naar vandaag te verplaatsen.
- **Nieuwe taak**: knop **+ DIRECTIVE** rechtsonder.
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
