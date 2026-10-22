# NoodNet Helmond — websiteversie 2.0

**Domein:** https://www.noodnethelmond.nl  
**GitHub-account:** `Alexw5701`  
**Repository:** https://github.com/Alexw5701/noodnethelmond-website  
**Versiedatum:** 22 oktober 2026

## Wat zit er in deze versie?

Zes volledig uitgewerkte hoofdonderdelen:

1. `index.html` — homepage met visie, schematische werking en pilotstatus.
2. `hoe-werkt-het.html` — werking PMR446, stappen, beperkingen en veelgestelde vragen.
3. `buurtpunten.html` — functie, selectie en status van kandidaat-buurtpunten, zonder adressen te verzinnen.
4. `over-noodnet.html` — achtergrond en verschil met gemeentelijk noodsteunpunt De Geseldonk.
5. `nieuws.html` — bewonersavond, testavond en geplande oefening; geen onbevestigde testresultaten.
6. `meedoen.html` — manieren waarop bewoners kunnen helpen en heldere uitleg over aanmelden.

Andere bestanden:

- `styles.css` — responsive vormgeving, donkerblauw/geel.
- `script.js` — mobiel menu met toetsenbordbediening.
- `favicon.svg` — herkenbaar webpictogram.
- `404.html` — pagina niet gevonden.
- `robots.txt` en `sitemap.xml` — basis voor vindbaarheid.
- `CNAME` — **bevat www.noodnethelmond.nl; niet verwijderen of veranderen.**
- `.nojekyll` — laat GitHub Pages de statische bestanden ongewijzigd publiceren.

## Publicatie: bestaande GitHub-website bijwerken

Je hoeft **geen nieuwe repository** aan te maken en je hoeft de DNS bij Mijndomein **niet opnieuw** in te stellen.

1. Ga naar https://github.com/Alexw5701/noodnethelmond-website.
2. Bewaar eventueel eerst een kopie van de huidige bestanden (oude versie) als je die wilt kunnen terugzetten. GitHub bewaart ook eerdere versies via de geschiedenis van de repository.
3. Pak het ZIP-bestand van versie 2.0 uit op je computer.
4. In GitHub, op het tabblad **Code**, kies **Add file / Voeg een bestand toe > Upload files / Bestanden uploaden**.
5. Sleep of selecteer **de losse bestanden** uit de uitgepakte map, rechtstreeks in de hoofdmap van de repository. **Upload niet alleen het ZIP-bestand.**
6. Dezelfde bestandsnamen worden bijgewerkt. Nieuwe bestanden (`favicon.svg`, `404.html`, `sitemap.xml`, `robots.txt`) worden toegevoegd. Vergeet ook `styles.css` en `script.js` niet: zonder deze bestanden ziet de website er niet goed uit.
7. Klik onderaan **Commit changes / Wijzigingen vastleggen**.
8. GitHub Pages publiceert de nieuwe versie via de bestaande instelling `main` / `(root)`.
9. Bezoek https://www.noodnethelmond.nl en vernieuw eventueel met `Ctrl + F5` om oude cache te omzeilen.

**Let op:** bestand `spelen.html` uit een eerdere versie kan in de repository zijn achtergebleven. Deze versie linkt niet naar `spelen.html`. Dit oude bestand kun je later afzonderlijk verwijderen als het niet gebruikt wordt.

### Als HTTPS nog niet beschikbaar is

De nieuwe bestanden hebben geen invloed op DNS, CNAME of het TLS-certificaat. GitHub geeft bij **Settings > Pages** aan of het certificaat klaar is. Schakel **Enforce HTTPS / HTTPS afdwingen** in zodra dat kan. Ga bij certificaatproblemen niet willekeurig DNS-records aanpassen.

## Belangrijke redactionele keuzes

- **Dit is een burgerinitiatief in pilotfase, geen werkend meldnetwerk of hulpdienst.** De site mag niet het beeld oproepen dat 24/7 hulp beschikbaar is.
- NoodNet en het door de gemeente onderzochte noodsteunpunt bij De Geseldonk zijn **verschillende trajecten**. De teksten claimen geen formele koppeling.
- De datum **12 november 2026** staat als *gepland* in de tekst; controleer dat voordat je het publiek als uitnodiging presenteert.
- Over de **PMR446-test op 19 oktober** zijn geen aantoonbare technische scores of betrouwbaarheidsclaims gepubliceerd. De site beschrijft daarom alleen dat er getest is.
- Locaties van buurtpunten worden nog niet vermeld. Publiceer privé-adressen alleen na instemming, een test en duidelijke inzetafspraken.
- Er staat **geen aanmeldformulier en geen verzonnen contactadres** op de site. Voor een toekomstig formulier zijn verantwoordelijke, ontvangstadres, doel, bewaartermijn en privacyinformatie nodig.
- **Deze website werkt mogelijk niet tijdens een grote storing.** Bewoners moeten belangrijke informatie ook offline beschikbaar hebben.
- De website bevat geen trackers, advertenties, remote fonts, cookies, externe scripts of externe afbeeldingen. Uitgaande links openen externe sites pas nadat een bezoeker klikt.

## Inhoud bijwerken

- **Nieuwsbericht aanpassen:** open `nieuws.html`; pas de tekst binnen het juiste artikel aan. Wijzig bij een nieuwe publicatie ook de datum in de kop.
- **Buurtpuntlocatie toevoegen:** pas `buurtpunten.html` pas aan na bevestigde locatie, toestemming en bereiktest. Vermeld ook of de locatie alleen bij aanwezigheid van de vrijwilliger actief is.
- **Aanmeldroute toevoegen:** wijzig `meedoen.html` zodra er een veilige externe formulierdienst of bevestigd e-mailadres is, met passende privacyinformatie. Plaats geen API-sleutels of aanmeldgegevens in de openbare GitHub-repository.
- **Kleuren of vormgeving aanpassen:** `styles.css`, bovenaan onder `:root`.
- **Menu aanpassen:** wijzig de navigatie in elk HTML-bestand, of gebruik een code-editor om dit automatisch op alle pagina's te vervangen.
- **Teksten actueel houden:** werk bij belangrijke wijzigingen `sitemap.xml` en de tekst `Bijgewerkt` in de footer bij.

## Inhoudelijke naslag

- https://www.denkvooruit.nl/informatieboekje
- https://www.rdi.nl/onderwerpen/vergunningen-en-registraties/portofoons-en-mobilofoons
- https://www.helmond.nl/1/nieuws/2026/oktober/denk-vooruit-bus-zaterdag-17-oktober-in-helmond
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Publicatiecontrole

- [ ] Zes pagina's openen via het navigatiemenu.
- [ ] Website goed op computer én telefoon.
- [ ] `www.noodnethelmond.nl` werkt met HTTPS wanneer het certificaat beschikbaar is.
- [ ] Datum van geplande activiteit klopt nog.
- [ ] Geen onbevestigde buurtpuntadressen of valse contactgegevens gepubliceerd.
- [ ] Hulpdienstwaarschuwing blijft zichtbaar.
