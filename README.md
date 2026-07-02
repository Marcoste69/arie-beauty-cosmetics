# Arie Beauty Cosmetics – Website

Statische One-Page-Website. Kein Build-Schritt, kein Framework, kein
JavaScript — `index.html` einfach im Browser öffnen oder auf einen
beliebigen Static-Host hochladen (Netlify, Vercel, GitHub Pages, IONOS, …).

Ein-Seiten-Layout statt 4-5 Unterseiten, weil das für ein kleines Studio
mit klarem "Jetzt anrufen"-Ziel schneller zum Termin führt. Auf Wunsch
lässt sich das später in Unterseiten aufteilen.

## Struktur
- `index.html` — komplette Seite (Hero, Über uns, Leistungen, Bewertungen,
  Galerie, Öffnungszeiten & Anfahrt, Footer)
- `css/style.css` — Styles (mobile-first, warme Nude-/Roségold-Palette)
- `images/` — siehe `images/README.md` für benötigte Fotos

## Vor dem Live-Schalten unbedingt prüfen

1. **Adresse bestätigen.** Das Briefing nennt „Löckherstraße 30/1", der
   Flyer im Chat zeigt „Löckherstraße 2". Im Code steht aktuell
   „Löckherstraße 30/1" (Briefing-Angabe). Adresse taucht an 4 Stellen in
   `index.html` auf — Footer, Anfahrt-Sektion, Google-Maps-Embed-Link,
   Schema.org-Block (`<script type="application/ld+json">`) — bei
   Korrektur bitte an allen 4 Stellen ändern.
2. **Öffnungszeiten ergänzen.** Bisher nur bekannt: „schließt 17:00 Uhr"
   (Freitag). Volle Wochenzeiten fehlen — suche in `index.html` nach
   `auf Anfrage` in der Öffnungszeiten-Tabelle und trage die echten Zeiten
   von der Facebook-Seite ein. Danach auch die
   `openingHoursSpecification` im Schema.org-Block ergänzen (aktuell
   bewusst weggelassen, siehe Kommentar dort).
3. **Fotos ablegen.** Siehe `images/README.md`. Sobald die Dateien im
   Ordner liegen, Galerie-Anzahl in `index.html` ggf. anpassen, falls
   weniger als 6 Fotos verfügbar sind.
4. **Preise.** Aktuell überall „auf Anfrage“, da keine Preisliste vorlag.
   Falls gewünscht, echte Preise in `index.html` in den jeweiligen
   `.service-card`-Blöcken ergänzen.

✅ Bewertungen sind bereits erledigt — 3 echte Google-Rezensionen
(Belle Desire, Uyun Resch, Petra Mursteiner) sind im Bewertungen-Bereich
eingetragen.

## Domain & Hosting

Noch nicht konfiguriert. Sobald eine Domain feststeht: `og:url` und `url`
im Schema.org-Block in `index.html` ergänzen (aktuell mit TODO-Kommentar
markiert).
