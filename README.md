# mitglied.bcerfurt.de

Formulare und Anleitungen für die Mitglieder des BC Erfurt e.V.

| Adresse | Inhalt |
| --- | --- |
| `/` | Übersicht |
| `/mitgliedsantrag/` | Aufnahmeantrag |
| `/schiedsrichterkosten/` | Erstattung Schiedsrichterkosten |
| `/fahrtkosten/` | Erstattung Fahrtkosten |
| `/sonstige-kosten/` | Erstattung sonstiger Auslagen |
| `/anleitungen/` | alle vier Anleitungen zum Lesen |
| `/pdf/` | dieselben Anleitungen als PDF |

Die drei Dateien `kostenerstattung*.html` im Wurzelverzeichnis sind Weiterleitungen
auf die neuen Adressen. Sie stehen in den bereits gedruckten Anleitungen und in
älteren QR-Codes – bitte nicht löschen.

## Formulare

Jedes Formular ist eine einzelne HTML-Datei ohne externe Abhängigkeiten. Verarbeitet
werden die Eingaben von einem Google-Apps-Script-Backend; dessen `/exec`-Adresse steht
als `PROXY` bzw. `PROXY_URL` oben im jeweiligen Formular. Die Backends liegen im
privaten Repo, da sie Zugangsschlüssel enthalten.

## Anleitungen ändern

Die Seiten unter `/anleitungen/` und die PDFs werden aus einer gemeinsamen Quelle
erzeugt, damit beide denselben Stand haben. Wer den Text ändert, baut beide neu –
sonst widersprechen sich PDF und Website.

## Hosting

GitHub Pages, Custom Domain über die Datei `CNAME`. Damit die Domain greift, muss
`mitglied` im DNS als CNAME auf `bcerfurt.github.io` zeigen.
