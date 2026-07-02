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
2. **Fotos ablegen.** Siehe `images/README.md`. Sobald die Dateien im
   Ordner liegen, Galerie-Anzahl in `index.html` ggf. anpassen, falls
   weniger als 6 Fotos verfügbar sind.
3. **Preise.** Aktuell überall „auf Anfrage“, da keine Preisliste vorlag.
   Falls gewünscht, echte Preise in `index.html` in den jeweiligen
   `.service-card`-Blöcken ergänzen.

✅ Bewertungen erledigt — 3 echte Google-Rezensionen (Belle Desire, Uyun
Resch, Petra Mursteiner) sind im Bewertungen-Bereich eingetragen.

✅ Öffnungszeiten erledigt — täglich 08:00–18:00, Termin auf Anfrage
(Hinweis im Anfahrt-Bereich + `openingHoursSpecification` im
Schema.org-Block gesetzt).

## Domain & Hosting

Noch nicht konfiguriert. Sobald eine Domain feststeht: `og:url` und `url`
im Schema.org-Block in `index.html` ergänzen (aktuell mit TODO-Kommentar
markiert).
