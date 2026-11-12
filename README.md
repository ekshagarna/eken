# Eken
Installationsbar webbapp (PWA) för Samsung/Android.

## Starta och installera
1. Lägg mappen på valfri HTTPS-webbplats, t.ex. GitHub Pages, OneDrive/SharePoint-webb eller egen webbserver.
2. Öppna `index.html` via webbplatsens adress i Samsung Internet eller Chrome.
3. Välj **Installera app** eller **Lägg till på startskärmen**.

För lokal provkörning på dator: kör `python -m http.server 8080` i mappen och öppna http://localhost:8080.

## Data och fakturaregister
- Data sparas lokalt i mobilen.
- Exporten använder semikolonseparerad UTF-8 CSV med samma 12 första kolumner som flikarna Tid EMP/Tid EMB/Tid Övrigt, plus resekolumner.
- CSV kan delas till OneDrive, Outlook eller Teams genom mobilens Dela-meny.
- JSON används för full säkerhetskopia och återställning.

## Säkerhet
Lokal lagring är inte en central backup. Exportera JSON regelbundet. För automatisk OneDrive-synk behövs en Microsoft Entra-appregistrering och MSAL-konfiguration.

Visual in this file was generated with Microsoft Copilot.
