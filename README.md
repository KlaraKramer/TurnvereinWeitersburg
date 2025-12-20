# Anleitung: Neuen Artikel zur Homepage hinzufügen

## Übersicht:
 * Ziel: Pflege einen neuen Artikel ein, formatiere ihn korrekt, und lade ihn hoch.

## Artikel einfügen:
 1. Denke dir eine ID zur Identifizierung des Artikels aus (muss einmalig sein), und merke sie dir.
    Die ID darf nur aus Kleinbuchstaben und Zahlen bestehen. Leerzeichen sind nicht erlaubt!
    * Beispiel: turnweihnachtsfeier2025
 2. [index.html](https://github.com/KlaraKramer/TurnvereinWeitersburg/blob/main/index.html):<br>
    a. Kopiere den grünen Beispielartikel, der ca. in Zeile 270 beginnt. Füge deine Kopie direkt unter dem       
        Beispielartikel ein, und entferne die zweite Zeile (< !--) und das Ende der vorletzten Zeile (-->)
    b. Füge deine ID in das "NEWID" Feld ein.
    c. Füge deinen Titel in das TITEL Feld ein.
    d. Füge dein Datum im Format '3. Januar 2026' in das DATUM Feld ein.
    e. Füge den Artikeltext in das ARTIKEL TEXT Feld ein, und erstelle ggf sinnvolle Zeilenumbrüche mit < br> (kein Leerzeichen).
 3. [index.html](https://github.com/KlaraKramer/TurnvereinWeitersburg/blob/main/index.html):<br>
    a. Füge den Namen deines Bildes in "IMAGE.IMG" ein, und wähle "picRight" oder "picLeft" aus, je nachdem auf welcher Seite das letzte Bild sich befindet.
    b. Wenn das Bild hochkant ist, setze "width:222px". Für Bilder im Queerformat kannst du es auf "width:333px" lassen.
    c. Füge eine kurze Beschreibung des Bildinhalts in das "ALTTEXT" Feld ein. Maximum 1 Satz.
    d. Wenn du keine Bildunterschrift brauchst, lösche die < figcaption> Zeile.
 4. [index.html](https://github.com/KlaraKramer/TurnvereinWeitersburg/blob/main/index.html):<br>
 

## Vorschau & Testen
 * Lokal starten: Klicke in deiner Ordnerstruktur auf index.html um die Datei im Browser zu öffnen.

## Build & Deployment
 * Commit:
 *   - Branch benennen z. B. feature/add-article-mein-artikel
 *   - Commit-Nachricht kurz und aussagekräftig: "Add article: Mein Artikel"
 * - Pull-Request:
 *   - Beschreibe Inhalt, evtl. Screenshots und Testanweisungen.
 *   - Verlinke relevante Issue-Nummern.
 * - CI/CD baut die Seite und deployed die Änderungen automatisch nach Merge (je nach Projekt).

## PR-Checklist (Kurz)
 * - [ ] Frontmatter vollständig und korrekt (title, date, summary, draft=false).
 * - [ ] Bilder vorhanden und optimiert; heroAlt gesetzt.
 * - [ ] Lokale Vorschau geprüft (Design, Format, Links).
 * - [ ] Linter/Tests erfolgreich.
 * - [ ] PR-Beschreibung und ggf. Übersetzungen ergänzt.

## Hinweise
 * - Project-spezifische Konventionen (Pfad, Felder, Build-Befehle) können abweichen — prüfe die README oder CONTRIBUTING.md des Repositories für projektspezifische Regeln.
 * - Bei Unsicherheit: Erzeuge eine Draft-PR und bitte eine Code-Review von einem Maintainer.