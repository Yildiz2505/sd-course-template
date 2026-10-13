# SD Learn 3.0

Centrale Markdown + HTML-lesopmaak voor Software Developer, MBO College Amstelland.

## Starten

Publiceer via GitHub **Settings → Pages → Deploy from a branch → main → /(root)**. De voorbeeldpagina staat daarna doorgaans op https://yildiz2505.github.io/sd-course-template/.

Lokaal testen: `python3 -m http.server 8000` en open http://localhost:8000. Via `file://` wordt Markdown vaak geblokkeerd.

## Nieuwe les

1. Kopieer `templates/lesson.md` naar `courses/react/les-02.md`.
2. Vul de les in.
3. Voeg aan de `lessons`-array in `js/app.js` toe: `{title:"Les 2 – JSX",path:"courses/react/les-02.md"}`.
4. Commit en push.

Ook beschikbaar: `templates/knowledgecheck.md` en `templates/project.md`.

## Centrale opmaak hergebruiken

Gebruik in andere websites:

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Yildiz2505/sd-course-template@main/css/style.css">
```

De andere website moet de bijbehorende HTML-klassen gebruiken. Alleen CSS toont nog geen Markdown. Gebruik bij productie liever een vaste release/tag dan `@main` voor gecontroleerde wijzigingen. In deze versie is `js/app.js` nog per cursus configureerbaar.

## Functies

Responsive menu, inhoudsopgave, donker/licht thema, kopieerknop voor code, TIP/WARNING/NOTE, print/PDF en React-voorbeeldles.

## Beperkingen

Statische website, geen Laravel of database. Nog geen persoonlijke voortgang, zoekfunctie of syntax-highlighting. Marked en DOMPurify worden vanaf jsDelivr geladen; voor offline gebruik moet je die bibliotheken lokaal opslaan.
