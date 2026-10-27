# japaknees

QuizCards: eine Japanisch-Lern-App in einer einzigen Datei (`index.html`), ohne Server und ohne Anmeldung. Alle Daten bleiben im Browser (localStorage).

## Der Weg
Die Startseite ist der **Weg**: 47 Einheiten in 8 Abschnitten, von den ersten Kana bis JLPT N5 (Einheiten 1–23) und N4 (24–40), dazu der Abschnitt „Praxis und Alltag“ (41–47: Datum und Zählwörter, Kleidung, Geld und Reisen, Notfälle, Ausgehen, Kultur, Büro).
- kurze Lektionen mit festem Ablauf: Wörter, Grammatik, Dialog, Checkpoint
- Prüfungen am Ende jedes Abschnitts (bestanden ab 80 %)
- Tagesziel und Serie
- Schriftschalter: Auto (mit Romaji-Hilfe), nur Romaji oder nur Kana
- Hörübungen lassen sich mit „Kann gerade nicht hören“ für eine Stunde pausieren
- Zusatz zu den Einheiten: Kanji-Gruppen und Lesegeschichten

## Weitere Bereiche
- **Wiederholen und Üben:** fällige Karten (Leitner-System), freies Üben nach Einheit, Wortliste
- **Schreibübung:** gelernte Wörter oder eigene Listen auf dem Canvas schreiben
- **Nachschlagen:** Wörterbuch über alle Wörter und Kanji, Verbformen-Tabelle, Aussprache (Branch `claude/nachschlagen`)
- **Kanji, Grammatik (zum Nachschlagen), Lesegeschichten, Chats, Spiele, eigene Sets**
- „Level-Modus (alt)“ und „Lernpfad (alt)“ bleiben als alte Ansichten erhalten

## Prüfung der Inhalte
Im Browser-Konsolenfenster prüft `checkCurriculum()`, ob in keiner Lektion ein Wort vorkommt, das noch nicht gelehrt wurde. Ein leeres Ergebnis (`[]`) bedeutet: alles in Ordnung.
