# Anleitung: Neuen Artikel zur Homepage hinzufügen

### Übersicht:
 * Ziel: Pflege einen neuen Artikel ein, formatiere ihn korrekt, und lade ihn hoch.

### Artikel einfügen:
 1. Denke dir eine ID zur Identifizierung des Artikels aus (muss einmalig sein), und merke sie dir.
    Die ID darf nur aus Kleinbuchstaben und Zahlen bestehen. Verwende das aktuelle Jahr. Leerzeichen sind nicht erlaubt!
    * Beispiel: kikofe2026
 2. [index.html](https://github.com/KlaraKramer/TurnvereinWeitersburg/blob/main/index.html):<br>
    a. Kopiere den grünen Beispielartikel, der ca. in Zeile 270 beginnt. Füge deine Kopie direkt unter dem       
        Beispielartikel ein, und entferne die zweite Zeile (< !--) und das Ende der vorletzten Zeile (-->)<br>
    b. Füge deine ID in das "NEWID" Feld ein.<br>
    c. Füge deinen Titel in das TITEL Feld ein.<br>
    d. Füge dein Datum im Format '3. Januar 2026' in das DATUM Feld ein.<br>
    e. Füge den Artikeltext in das ARTIKEL TEXT Feld ein, und erstelle ggf sinnvolle Zeilenumbrüche mit < br> (kein Leerzeichen).<br>
 3. [index.html](https://github.com/KlaraKramer/TurnvereinWeitersburg/blob/main/index.html):<br>
    a. Füge den Namen deines Bildes in "IMAGE.IMG" ein, und wähle "picRight" oder "picLeft" aus, je nachdem auf welcher Seite das letzte Bild sich befindet.<br>
    b. Wenn das Bild hochkant ist, setze "width:222px". Für Bilder im Queerformat kannst du es auf "width:333px" lassen.<br>
    c. Füge eine kurze Beschreibung des Bildinhalts in das "ALTTEXT" Feld ein. Maximum 1 Satz.<br>
    d. Wenn du keine Bildunterschrift brauchst, lösche die < figcaption> Zeile.<br>
    e. Wenn du eine Bildunterschrift einfügen möchtest, schreibe sie zwischen die < figcaption> und </ figcaption> Tags. Verwende sinnvolle Zeilenumbrüche mit < br> (kein Leerzeichen).<br>
 4. [index.html](https://github.com/KlaraKramer/TurnvereinWeitersburg/blob/main/index.html):<br>
    Unter "Übersicht aktueller Artikel:" (ca. Zeile 150), lege einen neuen Link an:<br>
    a. Kopiere die oberste mit < li> beginnende Zeile.<br>
    b. Füge deine ID nach dem # ein.<br>
        * Beispiel: #kikofe2026<br>
    c. Ersetze den weißen Text durch deine Artikelüberschrift.<br>
 5. [style/index.css](https://github.com/KlaraKramer/TurnvereinWeitersburg/blob/main/style/index.css):<br>
    a. Scrolle ans Ende der Datei und kopiere den letzten dreizeiligen Block (von # bis }).<br>
    b. Ersetze die ID (beginnt hinter dem #) durch deine ID.<br>
        * Beispiel: #kikofe2026<br>

### Vorschau & Testen
 * Lokal starten: Klicke in deiner Ordnerstruktur auf index.html um die Datei im Browser zu öffnen.
 * Öffne die Übersicht über aktuelle Artikel für das aktuelle Jahr, indem du auf den roten Knopf klickst.
 * Ist deine Artikelüberschrift da? Dann klicke auf sie.
 * Wirst du zu deinem Artikel geleitet? Dann überprüfe, dass alles gut aussieht.

<!--
### Build & Deployment
 * Commit:
 *   - Branch benennen z. B. feature/add-article-mein-artikel
 *   - Commit-Nachricht kurz und aussagekräftig: "Add article: Mein Artikel"
 * - Pull-Request:
 *   - Beschreibe Inhalt, evtl. Screenshots und Testanweisungen.
 *   - Verlinke relevante Issue-Nummern.
 * - CI/CD baut die Seite und deployed die Änderungen automatisch nach Merge (je nach Projekt).

### PR-Checklist (Kurz)
 * - [ ] Frontmatter vollständig und korrekt (title, date, summary, draft=false).
 * - [ ] Bilder vorhanden und optimiert; heroAlt gesetzt.
 * - [ ] Lokale Vorschau geprüft (Design, Format, Links).
 * - [ ] Linter/Tests erfolgreich.
 * - [ ] PR-Beschreibung und ggf. Übersetzungen ergänzt.

### Hinweise
 * - Project-spezifische Konventionen (Pfad, Felder, Build-Befehle) können abweichen — prüfe die README oder CONTRIBUTING.md des Repositories für projektspezifische Regeln.
 * - Bei Unsicherheit: Erzeuge eine Draft-PR und bitte eine Code-Review von einem Maintainer.
 -->