# Lexploris – Erreichbarkeit

Dieses Repository prüft alle 30 Minuten von außen, ob [www.lexploris.com](https://www.lexploris.com) erreichbar ist
(`/api/health`: Seite, Datenbank, Herzschlag des Workers). Schlägt eine Prüfung fehl, schickt GitHub eine
E-Mail an den Betreiber.

Es ist öffentlich, damit die Prüfung keine Actions-Minuten des privaten Lexploris-Repositorys verbraucht.
Es enthält keine Geheimnisse und keinen Code von Lexploris, nur die beiden Workflows:

- `erreichbarkeit.yml`: die Prüfung (alle 30 Minuten, Testalarm von Hand möglich)
- `lebenszeichen.yml`: wöchentlicher Eintrag, damit GitHub die geplanten Workflows nicht nach 60 Tagen abschaltet

Betrieb, SLOs und Runbooks stehen im (privaten) Repository von Lexploris unter `docs/betrieb/`.
