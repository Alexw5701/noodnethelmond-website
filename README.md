# NoodNet Helmond — website

Websiteconcept voor https://www.noodnethelmond.nl — pilot Mierlo-Hout (oktober 2026).

## Inhoud

- `index.html` — startpagina
- `hoe-werkt-het.html` — uitleg PMR446 en NoodNet
- `buurtpunten.html` — concept buurtpunten
- `over-noodnet.html` — achtergrond
- `nieuws.html` — pilotnieuws / conceptteksten
- `meedoen.html` — vrijwilligers (nog GEEN formulier)
- `styles.css`, `script.js` — vormgeving en menu
- `CNAME` — GitHub Pages domein `www.noodnethelmond.nl`
- `.nojekyll` — serveer statische website zonder Jekyll-verwerking

## Publiceren via GitHub (geen betaald hostingpakket nodig)

1. Gebruik je GitHub-account **Alexw5701**. Bekijk https://github.com/Alexw5701.
2. Maak via https://github.com/new een **public** repository `noodnethelmond-website` (zonder gevoelige gegevens). De URL wordt https://github.com/Alexw5701/noodnethelmond-website zodra je hem hebt aangemaakt.
3. Upload **de losse bestanden uit dit pakket**, rechtstreeks naar de hoofdmap van de repository (NIET het .zip-bestand als één bestand).
4. Open **Settings > Pages** van die repository. Kies **Deploy from a branch**, daarna `main` en `/(root)`, en klik **Save**.
5. Voer onder **Custom domain** `www.noodnethelmond.nl` in en klik **Save**.
6. Voeg bij Mijndomein in de DNS voor `noodnethelmond.nl` de GitHub Pages A-records toe voor de hoofddomeinnaam en de www-CNAME naar **alexw5701.github.io**. Zie onderstaande DNS-tabel.
7. Wacht op DNS-/certificaatverwerking en activeer **Enforce HTTPS** zodra beschikbaar.

### DNS bij Mijndomein

| Naam | Type | Waarde |
|---|---|---|
| `@` (hoofddomein) | A | `185.199.108.153` |
| `@` | A | `185.199.109.153` |
| `@` | A | `185.199.110.153` |
| `@` | A | `185.199.111.153` |
| `www` | CNAME | `alexw5701.github.io` |

Let op: Bij Mijndomein kan `@` automatisch worden omgezet naar de volle domeinnaam. Verwijder **alleen strijdige** bestaande A/AAAA/CNAME records voor `@` en `www` en **laat MX/TXT (e-mail) en andere subdomeinen staan**. Als je e-mail gebruikt via een dienst met aparte DNS-records, mogen die niet worden verwijderd. Stel eerst het eigen domein in bij GitHub, en pas daarna de DNS aan.

### Beveiliging: domein eerst verifiëren

GitHub adviseert verificatie via de profielinstellingen **Settings > Pages > Add a domain** en een unieke TXT-verificatiecode die GitHub genereert. Gebruik uitsluitend die code; verzin geen TXT-record. Dit voorkomt domain takeover. Behoud het TXT-record.

### Nog af te ronden voor publiek gebruik

- Controleer alle inhoud en het onderscheid burgerinitiatief versus gemeentelijk noodsteunpunt.
- Voeg nog geen buurtpuntadressen toe zonder toestemming.
- Maak eerst afspraken over wie aanmeldingen ontvangt, bewaartermijnen en privacyinformatie voordat een formulier live gaat.
- De website stelt niet voor dat NoodNet een gegarandeerde hulpdienst is; contacteer bij acuut gevaar de reguliere hulpdiensten.

Bronnen:
- https://docs.github.com/en/pages/quickstart
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
- https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/verifying-your-custom-domain-for-github-pages
- https://mijndomein.zendesk.com/hc/nl/articles/200416102-DNS-records
