# Kettlebell-Einführung

Interaktive Seite mit Übersicht, Ablaufplan und Sprechzettel für die erste Kettlebell-Einführung. Reine statische Seite, kein Build nötig.

## Struktur

```
index.html        Inhalt (Texte, Übungen, Ablaufplan)
assets/style.css  Aussehen (Farben ganz oben unter :root)
assets/app.js     Tabs, Abhaken, Theme-Umschalter
vercel.json       Vercel-Konfiguration
```

## Auf Vercel deployen

1. Repo auf GitHub anlegen und diese Dateien hochladen (oder pushen).
2. Auf vercel.com einloggen, **Add New → Project**, das Repo auswählen.
3. **Framework Preset: Other.** Build Command und Output Directory leer lassen.
4. **Deploy** drücken. Danach hast du eine feste URL.

Ab dann gilt: Jeder Commit auf `main` deployt automatisch neu.

## Aufs iPad

Die Vercel-URL in Safari öffnen, dann **Teilen → Zum Home-Bildschirm**. Die Seite startet danach wie eine App.

## Anpassen

- Texte, Übungen, Zeiten: `index.html`. Jede Übung ist ein `<details class="ex">`, jeder Ablaufblock ein `<div class="block" data-block>`.
- Farben und Schrift: `assets/style.css`, die Variablen stehen oben unter `:root` (hell) und in den Dunkel-Blöcken.
- Verhalten: `assets/app.js`.

Zum Testen lokal einfach `index.html` im Browser öffnen.

## Hinweis zum Inhalt

Intro, Swing, Clean, Squat und Press stammen aus den Erklärvideos „Meet the Kettlebell 2.0“. Warm-up, Zeiten und Gewichtsempfehlung sind eigene Ergänzungen.
