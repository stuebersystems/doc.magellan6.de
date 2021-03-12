
# Änderungen 2017

## LEGENDE

Abkürzung | Bedeutung
----------|----------
FIX | Korrektur bestehender Funktionalität
NEW | Neue Funktionalität
CHANGE | Änderung des Ablaufs, Verarbeitung oder Bedienung





> #### primary::Aktuelle Hinweise
>
> * SERIENDRUCK: Einige Kunden erhielten beim Aufruf des Seriendruck eine Fehlermeldung "Makrospeicher konnte nicht geöffnet werden". Diese Meldung resultiert aus Sicherheitseinstellungen in Word. Bitte lesen Sie dazu diesen [Artikel](https://doc.magellan6-kb.stueber.de/seriendruck/makrospeicher.html).
> * RUNTIME-ERROR: Einige Benutzer, die von älteren Versionen umsteigen, können MAGELLAN im Anschluss nicht starten. Meist ist die Ursache, dass eine der Dateien, die beim Programmstart geladen werden, beschädigt ist.
> Sie finden hier eine [Anleitung](https://doc.magellan6.stueber.de/installation/probleme-beim-update.html#meldung-runtime-error-) um dieses Problem zu beheben.

---

## 6.5.15 - 668 \(15.12.2017\)

### MAGELLAN

* FIX: \#1022324 - `Verzeichnisse > Zeugnisbeurteilungen`: Neuer Datensatz direkt editierbar
* FIX: \#1022324 - `Schüler > Zeugnis > Fächer > Sammellöschung`: Inkrementelle Suche in der Auswahl der Schüler
* FIX: \#1022324 - `Schüler > Zeugnis > Details > Sammelzuweisung`: Die Sortierung der Lehrer zur Auswahl der Tutoren und des Prüfungsvorsitzenden wurden umgedreht, es werden aktive Lehrer zuerst angezeigt
* FIX: \#1022311 - NRW: für die Keys-Datei "BS_Bildungsgänge" wurden die weiblichen Bezeichnungen ergänzt
* FIX: \#1022324 - `Schüler > Zeugnis > Details > Sammelzuweisung`: Die Sortierung der Tutoren umgedreht, es werden aktive Lehrer zuerst angezeigt
* FIX: \#1022311 - NRW: für die Keys-Datei "BS\_Bildungsgänge" wurden die weiblichen Bezeichnungen ergänzt
* FIX: \#1022445 - `Bewerber > Bearbeiten > Import > aus SchuelerOnline`: Für Bildungsgänge werden '/' in '-' gewandelt.
* FIX: Querverweise auf andere Ansichten werden jetzt nach dem Wechsel korrekt im Grid markiert \(Blaue Zeile\)
* FIX: \#1022664 - Wird von `Betriebe > Auszubildenden` aus der Zeitraum gewechselt, wird der Betrieb beibehalten

### MAGELLAN Administrator

* FIX: Aktualisieren der Medienkataloge beim Vergeben von Benutzerrechten, beim Wechsel des Mandanten, wenn mehrere Mandanten vorhanden sind.



### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: "Zuweisen von Zeugnisbemerkungen.dws" - Meldung behoben
* FIX: Abiturskript Niedersachsen NIE-APO-G9-2016.dws - Optimierung für Sportprofil angepasst
* FIX: Synchronisiere ABI.dws \( [Vorabdownload hier](https://my.hidrive.com/lnk/JiSJChxf) \)
* FIX: DE-DIAP-2015: Markierung und Summierung der Halbjahresergebnisse \( [Vorabdownload hier](https://my.hidrive.com/lnk/UcypCHSD)\)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* NEW: DAS-ZZ \(Q-Phase\)\(Anlage 1\)\(RiLi 1.6\).rpt
* NEW: DAS-GY \(Klasse 11-12\).rpt
* NEW: DAS-GS \(Klasse 1-2\).rpt
* NEW: DAS-GS-GY \(Klasse 3-10\).rpt
* NEW: DAS-GY-ABI (Anlage 7).rpt
* NEW: DAS-Ergebnisliste Abitur (Anlage 8)(§39_2).rpt (Übersicht der Ergebnisse der Deutschen Internationalen Abiturprüfung der einzelnen Prüflinge (s. §39(2)))
* UPDATE: MVP-GY \(Studienbuch - Seite 1\)\(Anlage 22\).rpt
* UPDATE: MVP-GY \(Studienbuch - Seite 2\)\(Anlage 22\).rpt
* UPDATE: Klassenlehrerliste.rpt


## 6.5.14 - 668 \(08.11.2017\)

> #### warning::Wichtig!
>
>** Ab dieser Version verlangt Magellan die Firebird Version 2.5.7**. Diese Version schließt eine Sicherheitslücke, die in allen vorangegangenen 2.5.x Versionen enthalten ist. Als Bonus erhält man Fehlerkorrekturen und Geschwindigkeitsverbesserungen des Firebird Systems.
> **Bitte folgen Sie der** [**Anleitung**](https://doc.magellan6.stueber.de/installation/firebird-aktualisieren.html#update-von-firebird-255-auf-257)!

### MAGELLAN

* FIX: `Hilfe > Systeminfo...` Vergleich der Pfade zur Anzeige der Unterschiede korrigiert
* UPDATE: Min. Voraussetzung Firebird 2.5.7
* FIX: Farbige Anzeige beim Vergleich der Pfade aus der Registry und den Angaben der Verbindung `MAGELLAN Administrator > Serververwaltung > Verbindungen verwalten` korrigiert

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* UPDATE: NIE-APO-G9-2016 \(Fachhochschulreife, Punkteberechnung optimiert\)

* [Download hier](https://my.hidrive.com/lnk/K2yJCLxy)
* [Anleitung: Landesanpassungen - Berechnungsskripte - NIE-APO-G9-2016](https://doc.la.stueber.de/nie-apo-g9-2016.html)

* FIX: Synchronisiere ABI.dws - Setzen des aktuellen Halbjahres zur Erfassung von Wiederholern

* ERWEITERT: "Synchronisiere Gemeinden.dws" - Dieses Skript führen Sie über das Modul `MAGELLAN Administrator > Datenbankpflege > Datenbank überprüfen > Gemeinden synchronisieren` aus. Dabei werden für Schüler, Lehrer und Betrieb die Felder PLZ, Ort und Ortsteil geprüft und ggfs. mit passenden Gemeindekennziffern aus dem Verzeichnis `Postleitzahlen`verbunden.

## 6.5.13 - 668 \(26.10.2017\)

> #### warning::Wichtig!
>
> **Änderungen für die Statistikschnittstellen 2017/18** stellen wir vorab zum Download zur Verfügung, anschließend veröffentlichte MAGELLAN-Ausgaben beinhalten diese Änderungen. Was geändert wurde dokumentieren wir an folgenden Stellen für Sie:
>
> * [** Änderungsliste RLP**](https://doc.ls.stueber.de/rheinland-pfalz/changelog.html)
> * [** Änderungsliste NRW**](https://doc.ls.stueber.de/nordrhein-westfalen/changelog.html)
>
> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](http://doc.magellan6.stueber.de/installation/serviceupdates.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](http://doc.magellan6.stueber.de/installation/troubleshootingupdate.html).

### MAGELLAN

* FIX: Problem bei der Eingabe unter `Schüler/Bewerber > Merkmale > B1-B4` behoben.

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: Synchronisiere Abi.dws:
* werden Fachdaten \(Fach, Unterrichtsart, Fachstatus, Note...\) für einen Wiederholer synchronisiert, werden vor dem Einfügen der zuletzt erworbenen Daten, die zuerst erworbenen Daten gelöscht. Verkehrte Einträge durch eine neue Kurswahl des Schülers in der Wiederholung werden vermieden.
* Trimester: wiederholt ein Schüler in der Klassenstufe 12 \(Noten für 12.1, 12.2\), wird das Trimester 12.3 beim Synchronisieren ignoriert, die alten Trimestereinträge der 12.1 und 12.2 werden gelöscht und die wiederholten Trimester \(12.1 und 12.2\) eingefügt.

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE: BAW-BG-ABI \(DIN A4 doppelseitig 2015\).rpt \(Ausgabe Sport als 5. PF eingebaut - ist Sport 5 PF, dann muss unter "Mündlich" der fachpraktische Punktwert und unter "Mündlich 2" der mündliche Punktwert der Prüfung eingetragen werden\)

## 6.5.12 - 667 \(16.10.2017\)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](http://doc.magellan6.stueber.de/installation/serviceupdates.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](http://doc.magellan6.stueber.de/installation/troubleshootingupdate.html).

### MAGELLAN

> #### warning::Wichtig!
>
> **Änderungen für die Statistikschnittstellen Rheinland-Pfalz und Nordrhein-Westfalen 2017/18** stellen wir vorab zum Download zur Verfügung, anschließend veröffentlichte MAGELLAN-Ausgaben beinhalten diese Änderungen. Was geändert wurde dokumentieren wir an folgenden Stellen für Sie:
>
> * [** Änderungsliste RLP**](https://doc.ls.stueber.de/rheinland-pfalz/changelog.html)
> * [** Änderungsliste NRW**](https://doc.ls.stueber.de/nordrhein-westfalen/changelog.html)

* FIX: `Extras > Schüler einschulen` und `Extras > Schüler wechseln` es stehen wieder "Fachtafeln" zur Auswahl
* FIX: Schülersuche mittels Suchfunktion - wählt man in der Ergebnisliste `Gehe zu Schüler` werden nun wieder alle Daten in den Registerkarten für den gewählten Schüler angezeigt
* FIX: Menü "Schüler" `Bearbeiten|Sammelzuweisung` - es stehen wieder definierte Merkmale zur Auswahl
* FIX: Menü "Lehrer \| Soll-Berechnung" - die Dauer beim Erfassen \(über `Editieren`\) von Soll-Schlüsseln wird wieder korrekt in die Ansicht übergeben
* FIX: Auswahllisten "Schüler", "Bewerber", "Personen", "Lehrer", "Schulen" und "Betriebe" sowie den Berliner Masken - Excel-Export übergibt die Spalte "Status" wieder als Text "Aktiv", "Neu" oder "Ausgeschult"
* FIX: Sammelzuweisung von Zeugnisbemerkungen
* FIX: Menü `Datenbank|Kennwort ändern`
* FIX: angezeigter Pfad unter `Hilfe|Systeminfo` konnte per WindowsExplorer nicht gewählt werden
* FIX: Speicherhaken wird wieder aktiv
* FIX: `Magellan|Bewerber|Gruppieren nach B-Merkmalen:` nie gefüllte und geleerte Felder wurden getrennt
* NEW: `Schüler > Merkmale > B1 - B4` Zeichengröße von 15 auf 100 erweitert.
* NEW: `Schüler > Statistik > T1 - T4` Zeichengröße von 15 auf 100 erweitert.
* FIX: `Extras > Statistik` bei der Prüfung wird in den Meldungen auch der Name der Plausibilitätsdatei mit ausgegeben. Diese Änderung ist nicht wichtig beim Erstellen der Statistik, hiermit können aber die entstandenen Meldungen besser in Excel sortiert werden.

### MAGELLAN Administrator

* FIX: Mehrfache Lizenzabfrage führte unter Windows Server 2003 zu einem Fehler beim Starten.
* FIX: Import von Mediendaten

### MAGELLAN Bibliothek

* FIX: Problem beim Übernehmen von neuen Ausleihern \(Meldung PLZ\) behoben

### MAGELLAN Skripteditor

* NEW: Icons erneuert
* NEW: Neue Editor-Komponente, die Probleme mit der Einrückung lösen soll
* NEW: Überarbeiteter Aufruf für Kompilieren und Ausführen; Kompilieren mit STRG+F7 / Ausführen mit F5
* NEW: Überarbeitete Suche- und Ersetzen Funktion; Suche mit STRG-F / Rückwärts-Suche mit SHIFT-F3 / Vorwärts-Suche mit F3
* FIX: Fehler beim Ausführen von Skripten Datenbankbefehlen im Skripteditor behoben \(WaitCursor\)

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: RLP-Statistik LehrerNeuanlage BBS 2017.xml \(STALA 5180\)
* FIX: RLP-SchuelerNeuanlage BBS 2017.xml \(STALA-29275\)
* FIX: RLP-Statistik LehrerNeuanlage BBS 2017.xml \(Massenmeldung STALA 5180 korrigiert\)
* FIX: RLP-SchuelerNeuanlage BBS 2017.xml \(STALA-29275 "Höchster Abschluss ABS: Bei angegebener Zugangsschulform \(826\) sind als Höchster Abschluss ABS nur 7 oder 19 zulässig." \)
* FIX: RLP-SchuelerNeuanlage BBS 2017.xml \(STALA 24000-2\)
* FIX: RLP-Statistik SchuelerNeuanlage ABS 2017.xml \(STALA-13100 Schlüssel in Meldung aktualisiert\)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* NEW: Klassenlehrerliste mit Räumen \(Variante 2\).rpt
* NEW: Betriebe mit Auszubildenden \(Nur aktuellste Laufbahn\).rpt
* NEW: Schülerpersonalblatt \(aktive Schüler mit Eltern und Vorbildung\).rpt - Nur noch aktive Schüler
* NEW: Schülerpersonalblatt \(nur mit Eltern und Vorbildung\).rpt - Alle Schüler
* FIX:
* Schülerliste \(Förderung\).rpt
* Schülerliste \(mit Sorgeberechtigten\).rpt

## 6.5.11 - 666 \(30.08.2017\)

### MAGELLAN

* NEW: \[Schüler &gt; Daten1 &gt; Ausbildung\] Die Information wurde um das Bildungsgangkürzel und das Berufskürzel ergänzt. Darstellung: `(AusbildungVon-AusbildungBis) - Ausbildungsbetrieb - BildungsgangKürzel (BerufsKürzel)`
* NEW: \[Schüler &gt; Daten1 &gt; Praxis\] Für Praxiseinträge ohne Praxisbetrieb wird ein Hinweis ausgegeben
* erweitert: `MAGELLAN > Hilfe > Systeminformationen` erweitert für die Anzeige von Windows 10
* FIX: Seriendruck mit Office 2000
* CHANGE: `Schüler > Fehlzeiten > Fehlstunden` \(Dezimalzahlen können eingegeben werden\)
* erweitert: `Statistik > RLP > BBS`: die Schulformstufenberechnung wurde erweitert
Für BVJs mit Inklusionsschülern müssen im Gliederungsplan 2017 die verfügbaren Stunden wie folgt differenziert werden:
Der Unterricht in einem BVJ mit Inklusionsschülern \(Bildungsgang 8101060\) wird im Tag "Verfuegbar" mit zwei unterschiedlichen SchulFomStufen gemeldet.
Der Unterricht in Sprachförderung \(DAZ = Deutsch als Zusatzsprache, Fach mit Schlüssel 6\) wird mit SchulFormStufe 83 gemeldet.
Der übrige Unterricht wird mit der SchulFormStufe 59 \(BVJ-Vollzeit\) gemeldet.
* FIX: `Statistik > RLP` : Prüfen der Plausibilitäten
* erweitert: Für Extras &gt; Statistik wird das bei der Installation ausgewählte Bundesland vorbesetzt. Das Bundesland kann im Modul MAGELLAN ADMINISTRATOR unter `Datenbankpflege > Bundesland auswählen` geändert werden.
* erweitert: die im Assistenten unter `Extras > Statistik` ausgewählten Optionen werden gespeichert.
* CHANGE: die im Assistenten unter `Extras > Statistik` ausgewählte Aktion für die erste Nutzung auf `Datenprüfung + Statistikdateien` erstellen vorbesetzt
* FIX: \[Statistik NRW ABS\] Problem beim Erzeugen der Statistikdatei behoben

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: Importiere SDTF, Exportiere SDTF
* FIX: BAW-APO-BGY-2010-G9.dws \( Deutsch als 4. und 5. Prüfungsfach\)
* FIX: RLP-Statistik LehrerNeuanlage BBS 2017.xml
* FIX: RLP-Statistik SchuelerBewegung ABS 2017.xml
* FIX: RLP-Statistik SchuelerBewegung BBS 2017.xml
* FIX: RLP-Statistik SchuelerNeuanlage ABS 2017.xml
* FIX: RLP-Statistik SchuelerNeuanlage BBS 2017.xml

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: Kursliste Namen.rpt

## 6.5.10 - 666 \(09.08.2017\)

> #### warning::Wichtig
>
> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Bitte denken Sie daran, nach der Anpassung der Datenstruktur die Zugriffsrechte der Benutzer wieder zu synchronisieren. Sie finden die Funktion im Modul MAGELLAN ADMINISTRATOR unter `Datenbankpflege > Datenbank überprüfen > Zugriffsrechte synchronisieren`.

### MAGELLAN

> #### warning::Wichtig!
>
> **Änderungen für die Statistikschnittstelle Rheinland-Pfalz 2017/18** stellen wir vorab zum Download zur Verfügung, bitte lesen Sie dazu [die Änderungsliste](https://doc.ls.stueber.de/rheinland-pfalz/changelog.html)!

* Hinweis: Seriendruck: Einige Kunden erhielten beim Aufruf des Seriendruck eine Fehlermeldung "Makrospeicher konnte nicht geöffnet werden". Diese Meldung resultiert aus Sicherheitseinstellungen in Word. Bitte lesen Sie dazu diesen [Artikel](https://doc.magellan6-kb.stueber.de/seriendruck/makrospeicher.html).

* CHANGE: Kontextmenü unter `Menü Schüler (Bewerber...) > Drucken > Berichte/Zeugnisse` verfügbar

* CHANGE: MagSDTFdaV5Sync.exe/MagSDTFSync.exe \(Hinzufügen von Verbindungsparametern fürs aktuelle Skripting-Mechanismus\)

* FIX: Löschen von Klassen und Klassenzeiträumen

* FIX: `Bewerber > Daten > Bearbeiten > Bewerbungsdaten > Details Hauptfächer`: Noteneingabe

* FIX: Extras &gt; Optionen &gt; Bewerberverfahren \(Karte wird korrekt gefüllt\)

* CHANGE: `Schüler > Zeugnis > Details > Fehlzeitenfelder` \(Verhalten bei der Eingabe und beim Leeren der Felder geändert\)

* CHANGE: Alle Auswahllisten: Wenn man auf einer der Datenkarten zum nächsten Datensatz wechselt, während die Datensätze in der Auswahlliste gruppiert sind, werden programmintern die Gruppierungen geöffnet, um die korrekte Datensatzreihenfolge je nach Sortierung in der Auswahlliste zu gewähren. Wechseln Sie zurück in die Auswahlliste, werden alle Gruppierungen geschlossen.

### MAGELLAN ADMINISTRATOR

* FIX: bei der Neuanlage eines Benutzers wird das Magellan Passwort auf Wunsch als MyMagellan Passwort übernommen.

> #### warning::Wichtig!
>
> Bitte verwenden Sie auch die parallel veröffentlichte Ausgabe von [MyMAGELLAN](https://download.stueber.de/bin/de/magellan/v6/mymagellan6.msi). Die Änderungen finden Sie in unserer [MyMAGELLAN-Dokumentation](https://doc.mymagellan6.stueber.de/changelog.html).

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: BAW-APO-BGY-2010-G9.dws \(Sport als 5.PF\)
* FIX: BAW-APO-BGY-2010-G9.dws \(Sonderfall für die Berechnung der Prüfung in Englisch\)

* FIX: BER-FW-APO-2017.js

* FIX: BER-FW-APO-2011.js

* FIX:Exportiere daVinci5 SDTF.dws \(Export aus MAGELLAN nach DAVINCI5\)

* FIX:Importiere daVinci5 SDTF.dws \(Import von MAGELLAN nach DAVINCI5\)

* CHANGE: Schüler fortschreiben.dws \(Wird ein Schüler fortgeschrieben und für die Klasse existiert bereits der neue Klassenzeitraum, wird dieser nicht mehr aktualisiert\)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* erweitert: DAS-JZ \(5-12\).rpt \(personalisierte Platzhalter für Bemerkungen erweitert\)
* erweitert: DAS-HJZ-JZ \(3-12\).rpt \(personalisierte Platzhalter für Bemerkungen erweitert\)
* Hinweis: Für eigene Berichte finden Sie [hier eine Anleitung](https://doc.magellan6-kb.stueber.de/cr-zeugnisbemerkungen-personalisieren.html) zum Einfügen von Platzhaltern in Berichte.

| Platzhalter in der Bemerkung | füllt der Bericht mit folgendem Wert |
| --- | --- |
| `<<Vorname>>` | Vorname des Schülers \(Beispiel: Hans\) |
| `<<VornameV>>` | Vorname, Vorname2 \(Beispiel: Hans Herbert\) |
| `<<Nachname>>` | Nachname des Schülers \(Beispiel: Müller\) |
| `<<NachnameV>>` | Zusatz und Nachname des Schülers \(Beispiel: von Müller\) |
| `<<Name>>` | Vorname, Vorname2, Namenszusatz und Nachname des Schülers \(Beispiel: Hans Herbert von Müller\) |
| `<<Er_Sie>>` | Er/Sie \(je nach Geschlecht des Schülers\) |
| `<<er_sie>>` | er/sie \(je nach Geschlecht des Schülers\) |
| `<<Seine_Ihre>>` | Seine/Ihre \(je nach Geschlecht des Schülers\) |
| `<<seine_ihre>>` | seine/ihre \(je nach Geschlecht des Schülers\) |
| `<<Ihm_Ihr>>` | Ihm/Ihr \(je nach Geschlecht des Schülers\) |
| `<<ihm_ihr>>` | ihm/ihr \(je nach Geschlecht des Schülers\) |
| `<<Seinen_Ihren>>` | Seinen/Ihren \(je nach Geschlecht des Schülers\) |
| `<<seinen_ihren>>` | seinen/ihren \(je nach Geschlecht des Schülers\) |
| `<<DerSchueler_DieSchuelerin>>` | Der Schüler/Die Schülerin \(je nach Geschlecht des Schülers\) |
| `<<derSchueler_dieSchuelerin>>` | der Schüler/die Schülerin \(je nach Geschlecht des Schülers\) |
| `<<DemSchueler_DerSchuelerin>>` | Dem Schüler/Der Schülerin \(je nach Geschlecht des Schülers\) |
| `<<demSchueler_derSchuelerin>>` | dem Schüler/der Schülerin \(je nach Geschlecht des Schülers\) |

## 6.5.9 - 665 \(28.07.2017\)

### MAGELLAN

* CHANGE: `Extras > Schüler rückversetzen` nur noch mit sysdba-Anmeldung sichtbar
* NEW: wird die Netzwerkanbindung zwischen MAGELLAN und der Datenbank unterbrochen, wird die Verbindung automatisch ohne Zwischenmeldung wieder aufgenommen
* FIX: einen Schüler und dessen Kopie \(Feld IDIntern mit der ID des originalen Schülers gefüllt\) beim "Schüler Einschulen" zusammenführen
* FIX: Sammellöschung korrigiert \(MAGELLAN.exe und Skript "Loeschen von SchuelerFaechern.dws"\)
* FIX: `Schüler > Zeugnis` zeigt als Startkarte die Unterkarte `Fächer`.
* FIX: `Betriebe > Bearbeiten > Organisieren > Betriebe zusammenführen`\(Mandantenfehlermeldung beim Löschen des zweiten Betriebs\)
* FIX: Beim Aufruf der Menüs per Tastenkombination werden die Markierungen in der Menüleiste korrekt aktualisiert
* FIX: gewählte Fenstergröße der Seitenvorschau wird gespeichert
* FIX: \(Berliner Masken\) Schüler &gt; Zeugnis &gt; Zeugnis \(Schaltflächen aktiviert\)

![&quot;Editieren&quot;, &quot;Löschen&quot;, &quot;Alles löschen&quot; werden beim Zuweisen einer Zeugnisbemerkung oder eines Zeungisformulars aktiviert](/images/liesmich/6.5.9.00.png)

### MAGELLAN BIBLIOTHEK

* FIX: zur Übernahme angezeigte Schüler im Assistenten unter `Schüler > Neu (rotes Plus)` korrigiert
* FIX: Schülersumme im Assistenten unter `Schüler > Neu (rotes Plus)` korrigiert
* NEW: Anzeige der zur Übernahme in die Bibliothek möglichen Ausleiher beschleunigt

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: Exportiere Fachwahl Schueler.dws \(`Abitur > Bearbeiten > Fachwahl exportieren > SDTF oder Untis`\)
* FIX: "DE-DIAP-2015.dws" \(Vorschlagsautomatik, Berechnen des 4. und 5. Prüfungsfachs\)
* FIX: Loeschen von SchuelerFaechern.dws
* CHANGE: "Benutzerrechte zuweisen" und "Synchronisiere Zugriffsrechte" berücksichtigen den Menüpunkt "Mittelstufe". Aktuell gibt es noch keine Abstufung der Rechte.

## 6.5.8 - 665 \(10.07.2017\)

### MAGELLAN

* NEW: Nordrhein-Westfalen Statistikmodul 2017. Beachten Sie bitte die aktualisierten [Schlüsselverzeichnisse](https://doc.ls.stueber.de/schluesselverzeichnisse.html).
Bitte lesen Sie die aktualisierte [Statistikdokumentation für NRW](https://doc.ls.stueber.de/nordrhein-westfalen/abs+bbs.html).
* CHANGE: Funktion `Schüler > Bearbeiten > Passfoto > Passfoto aus Digitalquelle...` überarbeitet
* CHANGE: Funktion `Schüler > Auswahlliste> Rechtsklick > Dokumente > aus Digitalquelle...` überarbeitet
* CHANGE: Im Assistenten fürs `Schüler versetzen` wird die `Weiter`-Schaltfläche erst aktiv, wenn für die Fachtafel die Auswahl korrekt ist \(Häkchen gesetzt und Fachtafel gewählt **oder** Häkchen nicht gesetzt\)
* CHANGE: `Schüler > Abitur > Qualifikation` gewählte Zeile wird blau hinterlegt

![Schaltfläche &quot;Weiter&quot; wird erst bei korrekter Eingabe aktiv](/images/liesmich/6.5.8.00.png)

* CHANGE: Lizenzeinstellung für "MAGELLAN Abitur" überprüft

### MAGELLAN Skripteditor

* FIX: "Object factory for class is missing"

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: BER-Statistik Abitur 2015.xml
* FIX: Synchronisiere BBS.dws
* NEW: Menü `Mittelstufe`mit in die Skripte `Benutzerrechte zuweisen.dws` und `Synchronisiere Zugriffsrechte.dws` integriert
* FIX: DE-DIAP-2015.dws

## 6.5.7 - 665 \(27.06.2017\)

> #### warning::Wichtig
>
> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Bitte denken Sie daran, nach der Anpassung der Datenstruktur die Zugriffsrechte der Benutzer wieder zu synchronisieren. Sie finden die Funktion im Modul MAGELLAN ADMINISTRATOR unter `Datenbankpflege > Datenbank überprüfen > Zugriffsrechte synchronisieren`.

### HINWEIS für angepasste Skriptdateien

Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert.
Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier:
[https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

### MAGELLAN

* NEW: Rheinland-Pfalz Statistikmodul 2017. Beachten Sie bitte die aktualisierten [Schlüsselverzeichnisse](https://doc.ls.stueber.de/schluesselverzeichnisse.html). Die aktualisierte [Statistikdokumentation](https://doc.ls.stueber.de/rheinland-pfalz/abs+bbs.html)
für RLP finden Sie hier.
* FIX: `Abitur > Prüfungen` Die Verzeichnisliste hinter den Eingabefeldern \(z.b. mdl. Note\) klappt bei der Eingabe nicht mehr auf
* FIX: Bei Gruppierungen wurden für den ersten Schüler in einigen Situationen keine Daten in Bericht geladen
* FIX: beim Erfassen von Ausbildungsdaten für Schüler nacheinander, wird der Ausbilderkontakt korrekt aktualisiert.
* FIX: Beschriftung im Assistenten unter `Bewerber > Import > SchülerOnline`
* FIX: Ergebnis der Prüfung aus SchülerOnline kann vollständig nach Excel übergeben werden
* FIX: Bewerber-Doublettenprüfung: Wechsel zum Schüler/Bewerber korrigiert
* FIX: Zeitraumüberschneidungsprüfung unter `Verzeichnisse > Zeiträume` erweitert
* FIX: Das Bewerber-Seriendruckfeld «Sorgebe\_Anrede» gab im Worddokument den verkehrten Wert aus, also z.B. statt "Familie" die Ziffer 8.
* FIX: Accessaufruf aus MAGELLAN \(neu Alt+A\) wieder eingebunden
* FIX: Speichern der Umbenennung unter `Schüler > Zeugnis > Fächer und Leistungen`
* FIX: Speichern der Umbenennung unter `Schüler > Abitur > Qualifikation/Prüfung/Fachwahl`
* FIX: Speichern der Umbenennung unter `Mittelstufe > Prüfung`
* FIX: Speichern der Umbenennung unter `Berufsschule > Matrix`
* CHANGE: die Anmeldefenster für MAGELLAN und den MAGELLAN Administrator sind unterschiedlich bezeichnet
* FIX: `Berufschule > Drucken > Zeugnisse > Drucken und Export nach PDF`
* FIX: Unter Fachtafel-Fächer bleibt der Bearbeitenbutton auch beim Anlegen mehrerer Fächer aktiv!
* NEW: Für das Bundesland Saarland gibt es das neue Modul MAGELLAN MITTELSTUFE. Dieses dient der automatischen Berechnung der Abschlüsse an Gemeinschaftsschulen nach dem Besuch der Klassenstufe 9. Bitte beachten Sie die entsprechende [Anleitung](https://doc.la.stueber.de/mittelstufe.html).

### MAGELLAN-ADMINISTRATOR

* FIX: Unter "Datensicherung" wurden die Punkte Sicherung und Wiederherstellung überarbeitet
* CHANGE: Bitte beachten Sie auch die dazu passende Dokumentation für die [Sicherung der Datenbank](https://doc.magellan6.stueber.de/admin/db-connection.html#sicherungskopie-erstellen) und die [Wiederherstellung der Datenbank aus einer Sicherungskopie](https://doc.magellan6.stueber.de/admin/db-connection.html#sicherungskopie-wiederherstellen).

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).

* NEW: "SAR-VO-GEM-2015.dws" für die automatischen Berechnung der Abschlüsse an Gemeinschaftsschulen nach dem Besuch der Klassenstufe 9
* FIX: "SHL-APO-2015.dws" Aktualisierung für MAGELLAN 6.5.x/Berechnung korrigiert
* FIX: "BER-APO-KO-2011" Aktualisierung für MAGELLAN 6.5.x
* FIX: "SAR-APO-2017.dws"
* FIX: "SAR-APO-BGY-2017.dws"
* FIX: "RLP-APO-2014" Aktualisierung für MAGELLAN 6.5.x
* FIX: "BER-FW-APO-2011" Kursprüfung G8/G9
* FIX: "BER-FW-APO-2017" Kursprüfung G8/G9
* FIX: "RLP-APO-BGY-2010"
* FIX: "NRW-AS-APO-BK-1999" Aktualisierung für MAGELLAN 6.5.x und inhaltliche Änderungen.
Bitte beachten Sie die
[Anleitung](https://doc.la.stueber.de/durchschnitt_abschluss/nrw-as-apo-bk-1999.html)
und die [Änderungshinweise](https://doc.la.stueber.de/durchschnitt_abschluss/nrw-as-apo-bk-1999/anderungen.html) zu diesem Skript.
* FIX: "Synchronisiere BBS.dws"
* FIX: "BER-APO-2011 / BER-APO-2017" Summenberechnung für die Fachstatus 1PFBLL bis 4PFBLL
* FIX: "BBS Faecher kopieren.dws"

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: SAR-GEMS-Verhaltenszeugnis.rpt \(Druckeroptionen geändert, Druckberechtigung erweitert\)
* FIX: SAR-GEMS-AS \(Klasse 9-10\).rpt \(Druckeroptionen geändert, Satz für Abschluss korrigiert - Kultusministerkonferenz, Druckberechtigung erweitert\)
* FIX: SAR-GEMS-AZ \(Klasse 5-10\).rpt \(Druckeroptionen geändert, Druckberechtigung erweitert\)
* FIX: BER-GY \(Abi-18a - Mitteilungen zu den schriftlichen und mündlichen Prüfungen\)\(03.12\).rpt
* FIX: BER-GY \(abi\_4\_berechnungsbogen\)\(09.12\)
* FIX: DAS-JZ \(5-12\).rpt \(Ausgabe Vor- und Nachname Schüler\)

## 6.5.6 - 664 \(09.06.2017\)

### MAGELLAN

* FIX: Fehlermeldung beim Start von MAGELLAN behoben, wenn das Datum im Format dd/mm/yyyy dargestellt wird.

![Meldung korrigiert](/images/liesmich/6.5.6.date.png)

* NEW: Neue Beispielvorlage für den Seriendruck aus dem Schülermenü an den Ausbilder des Schülers \(Brief an Ausbilder des Schülers \(Ausbildungsbetrieb\).dotx\). Bitte beachten Sie auch die Abschnitte [Seriendruck an den aktuellen Betrieb oder den Ausbilder des Schülers](https://doc.magellan6.stueber.de/howto/seriendruck.html#an-den-aktuellen-betrieb-oder-den-ausbilder-des-schülers) und [Seriendruck: Ausbilder per Mail anschreiben?](https://doc.magellan6.stueber.de/howto/seriendruck.html#den-ausbilder-per-mail-anschreiben).
* FIX: Anzeige der Fahrstrecken unter `Schüler > Daten4 > Fahrstrecken`
* CHANGE: \[Berlin\] Abiturdatenstatistikschnittstelle für 2017 angepasst. Bitte beachten Sie unsere [Dokumentation](https://doc.magellan6.stueber.de/bundeslaender/berlin/stat.abidaten.html)!
* FIX: Problem beim Auslösen von Berechnungen aus `Schüler > Zeugnis > Leistungen > Durchschnitt` behoben.
* FIX: Problem beim Auslösen von Simulationen aus `Abitur > Qualifikation > Simulation...` behoben.
* FIX: Filterung beim Drucken von Zeugnisformularen \(`Schüler > Drucken > Zeugnisformulare`\)

### Importe

* FIX: \[NRW\] BS\_Bildungsgaenge.keys

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).

* FIX: \[NRW-APO-BK-2012.dws\] Problem beim Ausführen des Skripts behoben
* FIX: \[BAW-APO-BGY-2010-G9.dws\] Problem beim Ausführen des Skripts behoben
* FIX: \[RLP-APO-BGY-2014\] Problem beim Ausführen des Skripts behoben
* FIX: \[BER-APO-2011\] Problem beim Ausführen des Skripts behoben
* FIX: \[BER-APO-2017\] Problem beim Ausführen des Skripts behoben
* FIX: \[SAC-APO-BGY-2017\] Korrektur beim Einbringen der Fremdsprachen
* FIX: \[NRW-AS-APO-BK-1999\]

### MAGELLAN-ADMINISTRATOR

* CHANGE: Problem in der Ausleihe behoben \(Barcodescanner und Ausleihe/Rückgabe/Verlängerung, verkehrtes Buch markiert\)

### MAGELLAN-Bibliothek

* FIX: Beim Scannen in der Ausleihe wurde in einigen Situationen nicht das gescannte, sondern das erste Buch in der Liste markiert.
* FIX: Mehrere neue Bücher für einen Ausleiher scannen \(Ausleiher scannen, Exemplare scannen, Aktion ausführen\) und im Anschluss eins der soeben ausgeliehenen Bücher zurückgeben: als Ergebnis wird oben rechts in den Feldern nicht das gescannte Buch, sondern ein anderes gezeigt.
* FIX: Ein Exemplar ist überzogen und taucht daher in der Liste der Mahnungen auf. Es wird gemahnt. Anschließend in die Ausleihe wechseln und das Exemplar scannen: die Liste und die Ausleiherinfos bleiben leer, nur oben rechts taucht Info auf, die Aktion erfolgt aber nicht.

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE: BER-GY \(abi\_4\_berechnungsbogen\)\(09.12\).rpt

## 6.5.5 - 664 \(29.05.2017\)

### MAGELLAN

* FIX: Problem beim Starten von MAGELLAN unter Windows Server 2003

## 6.5.4 - 664 \(24.05.2017\)

### MAGELLAN

* FIX: in einigen Konstellationen ergab sich ein Runtime-Error beim Programmstart, die Ursache ist behoben
* FIX: `Seriendruck > Schüler > an Schüler > Klassenkürzel`: im parallel abgelegten Worddokument wurde nicht das korrekte Klassenkürzel gespeichert
* FIX: `Menü "Abitur" > Drucken "Prüfungslisten Drucken"`
* FIX: Benutzer der Rechtegruppen Kollegium2-Kollegium5 können wieder Daten auf der Laufbahnkarte ändern
* FIX: Beim Verwenden der Seriendruckfunktion wird die WinWord-Anwendung korrekt geöffnet und geschlossen
* FIX: Spaltenreihenfolge unter `Schüler > Zeugnis > Fächer` und unter `Schüler > Zeugnis > Leistungen` wird wieder gespeichert
* FIX: Fehlermeldung beim Start von MAGELLAN behoben, wenn 12-stündiges Zeitsystem \(AM + PM\) statt 24-stündiges Zeitsystem verwendet wird.

![Meldung korrigiert](/images/liesmich/6.5.4.time.png)

### MAGELLAN-ADMINISTRATOR

* CHANGE: Aufruf "Kopiere Empfehlungen" unter `Datenbankpflege > Datenbank überprüfen` entfernt
* FIX: MAGELLAN-Importformat an neue Komponenten angepasst
* FIX: Fehlermeldung beim Start von MAGELLAN behoben, wenn 12-stündiges Zeitsystem \(AM + PM\) statt 24-stündiges Zeitsystem verwendet wird.

### MAGELLAN-Bibliothek

* FIX: Testmeldung beim Scannen entfernt

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).

* FIX: DE-DIAP-2005.dws
* FIX: SAC-APO-BGY-2017.dws
* FIX: NRW-AS-APO-BK-1999.dws \(DateTime Meldung\)

* FIX: Synchronisiere Generatoren.dws

* FIX: Synchronisiere Zugriffsrechte.dws

* FIX: Synchronisieren Gemeindekennziffern.dws
* FIX: Korrigiere KlassenZeiträume.dws
* FIX: Entfernen von Unterstrichen im Schülernamen.dws
* FIX: Benutzerrechte zuweisen.dws

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* MVP-BS-AS-AZ.rpt
* MVP-BS-AS-AZ\_Sonstige.rpt
* SAR-GEMS-AS \(Klasse 9-10\).rpt
* Dienstbezeichnung 2. Klassenlehrer aktualisiert, neue Sternchen-Bemerkungen \(\*\) - aktualisiert
* Bemerkungsfelder für Fächer, die nach einem individuellen Förderplan unterrichtet werden, aktualisiert \(\*,\*\* **, **\*\*\*\)
* Ein Handout zu den Zeugnisformularen Klassenstufen 5-10 \(Gymnasium\) ist auf dem BSCW-Server [http://bscw.saarland.de](http://bscw.saarland.de) abgelegt.
* SAR-GEMS-Verhaltenszeugnis.rpt
* Dienstbezeichnung 2. Klassenlehrer aktualisiert
* Ein Handout zu den Zeugnisformularen Klassenstufen 5-10 \(Gymnasium\) ist auf dem BSCW-Server [http://bscw.saarland.de](http://bscw.saarland.de) abgelegt.
* SAR-GEMS-AZ \(Klasse 5-10\).rpt
* Dienstbezeichnung 2. Klassenlehrer aktualisiert
* Ein Handout zu den Zeugnisformularen Klassenstufen 5-10 \(Gymnasium\) ist auf dem BSCW-Server [http://bscw.saarland.de](http://bscw.saarland.de) abgelegt.

## 6.5.3 - 664 \(11.05.2017\)

### MAGELLAN

* NEW: \[Berlin\] Abiturdatenstatistikschnittstelle für 2017 angepasst. Bitte beachten Sie unsere [Dokumentation](https://doc.magellan6.stueber.de/bundeslaender/berlin/stat.abidaten.html)!
* FIX: Schülername wird wieder eingeblendet auf der Karte `Familie`
* FIX: Beim Seriendruck vom Schülermenü an den Sorgeberechtigten wird das Feld `Sorge_Anrede` wieder korrekt umgesetzt
* FIX: Anfrage einer Testlizenz über den Willkommensassistenten
* FIX: Fehlermeldung beim Seriendruck nach Word \(mehrere Menüs\) ohne Aktivierung der Dokumentenablageoption \(unter `Extras > Optionen > Dokumente > Word-Seriendruck`\)
* FIX: im Menü `Abitur`wird die Spalte `Klasse`in der Auswahlliste gefüllt

### Skripte

Eine Anleitung für alle unsere Skripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).

* FIX: SAC-APO-BGY-2011.dws

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* NEW: DAS-GY-ABI 2017 \(Version 2\).rpt
* NEU - Ausgabe Sprachniveaus
* bitte tragen Sie in unter "Daten 3\|Fremdsprachenfolge" im Feld "Referenz" das Referenzniveau der Fremdsprache ein. Grundlage bildet das Verzeichnis\|weitere Schlüsselverzeichnisse\|Sprachreferenzen
* NEW: DAS-GY-ABI-Reifepruefung 2017.rpt
* NEU - Ausgabe Sprachniveaus
* bitte tragen Sie in unter "Daten 3\|Fremdsprachenfolge" im Feld "Referenz" das Referenzniveau der Fremdsprache ein. Grundlage bildet das Verzeichnis\|weitere Schlüsselverzeichnisse\|Sprachreferenzen"
* NEW: SAC-BG-ABI \(E.01.06\)\(2017\).rpt \(Fremdsprachenniveaus werden unter Zeugnisbemerkungen ausgegeben.Tragen Sie im Menü „Abitur“ unter „Zeugnis“ im Feld „Zeugnisbemerkungen“ den entsprechenden Text ein\)

## 6.5.2 - 664 \(09.05.2017\)

### MAGELLAN

* FIX: Fehler beim Drucken im Netzwerk behoben.
* FIX: `Bewerber > Ausbildung > aktuelle Ausbildung` kann wieder eingestellt werden
* FIX: Meldung beim Drucken aus dem Modul `Abitur`

### Skripte

Eine Anleitung für alle unsere Skripte finden Sie in der Dokumentation \[MAGELLAN Landesanpassungen\].\([https://doc.la.stueber.de/](https://doc.la.stueber.de/)\)

* FIX: SAC-APO-BGY-2014.dws und SAC-APO-BGY-2017.dws
* NEW: [SAR-APO-2017.dws](https://doc.la.stueber.de/Skripte/SAR-APO-2017.html) gemäß Änderung der GOS-VO vom 02.05.2017
* NEW: [DE-DIAP-2015.dws](https://doc.la.stueber.de/de-diap-2015.html) gemäß dem neuen DIAP 2015

## 6.5.1 - 664 \(05.05.2017\)

* [Anleitung zum Einspielen eines Serviceupdate.](installation/update.md)
* [Probleme beim Einspielen des Updates?](installation/probleme-beim-update.md)

> #### warning::Wichtig
>
> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten.

### MAGELLAN

* NEW: für nicht eingeschulte Schüler \(Vagabunden\) werden die Karten `Schüler > Laufbahn`und `Schüler > Zeugnis`deaktiviert

![Deaktivierte Karten für nicht eingeschulte Schüler ](/images/liesmich/6.5.01.png)

* FIX: MagSDTFSync.exe wählt die korrekte MAGELLAN.evm \(lokal oder per MAGELLAN.paths\)
* NEW: Seriendruckschnittstelle zu Office 2016 wird unterstützt
* NEW: Prüfung unter `Verzeichnisse > Zeiträume > Von/Bis`:
* Prüfung auf mögliche Überschneidungen mit bereits erfassten Zeiträumen
* `Von` muss kleiner als `Bis`sein
* Vor dem Speichern wird geprüft, ob `Von`und `Bis` gefüllt sind
* Prüfung wird aktiviert beim Ändern einer Zeile
* NEW: unter `Schüler > Zeugnis > Fächer` sind Mehrfachmarkierungen möglich
* NEW: unter `Verzeichnisse` und unter `Verzeichnisse > Weitere Verzeichnisse`:
* Mehrfachmarkierung von Zeilen möglich \(mehrere Zeilen können zeitgleich gelöscht werden, Zeilenauswahl für den Excelexport möglich\)
* eine neue Zeile kann über die Tastenkombinaton STRG+N angelegt werden
* Schlüsselverzeichnisse sind beim Aufruf generell zur Bearbeitung gesperrt, damit können Sie die inkrementelle Suche in den Listen nutzen \(Feld anklicken, gesuchten Wert eintippen, Markierung wechselt zur ersten Übereinstimmung. Zur nächsten Übereinstimmung wechseln Sie mit STRG und den Pfeiltasten \(auf und ab\)\)
* Bestehende Werte können mit Klick auf die neue Schaltfläche `Bearbeiten` geändert werden
* wenn eine neue Zeile übers Plus oder STRG+N erzeugt wurde, ist der Bearbeitungsmodus automatisch aktiv
![Über die Schaltfläche gelangen Sie in den Editiermodus des Verzeichnisses](/images/liesmich/6.5.02.png)

* NEW: neue Menü-Navigationsleiste \(bessere Erkennbarkeit des gewählten Menüpunktes\)

* FIX: Problem bei veränderter Spaltenanordnung in den Assistenten behoben

* CHANGE: unter `Extras > Optionen > SMS-Nachrichten` kann Länderkennung jetzt maximal 3-stellig erfasst werden.

![Die Länderkennung kann auch dreistellig erfasst werden](/images/liesmich/6.5.00.png)

* CHANGE: alle Benutzerhandbuchverweise gehen auf unsere Onlinedokumentationen

### Import/Export

* CHANGE:\[MVP\] SIP-Schnittstelle überarbeitet \(`MAGELLAN > Extras > Export > SIP...`\). Die Dokumentation der Landesstatistiken finden Sie [hier](https://doc.ls.stueber.de/mecklenburg-vorpommern/sip.html).
* CHANGE:\[MVP\] Schlüsselimportdateien aktualisiert, bitte importieren Sie die Schlüsselverzeichnisse im MAGELLAN ADMINISTRATOR unter `Datenimporte > Schlüsselverzeichnisse importieren`.
* FIX: \[NRW\] Beim Import bereits bestehender Schüler wurde ein Problem beim Abgleich der Sorgeberechtigten behoben. Bitte beachten Sie unsere Dokumentation für den [Abgleich mit SchülerOnline](https://doc.magellan6.stueber.de/bundeslaender/nrw/schueleronline.html).

### MAGELLAN-Importkonverter

* erweitert: Der MAGELLAN-Importkonverter kürzt die Staatsangehörigkeiten der Sorgeberechtigten aus IBIS ab \(Beispiel: 000~~=DEU~~, also aus 000=DEU wird 000, beibehalten wird alles vor dem Zeichen "="\)

### Skripte

* aktualisiert: \[MVP\] Prüfskripte für SIP \(MVP-SIP 2017\_BBS.xml, MVP-SIP 2017\_ABS.xml\)
* CHANGE: [RLP-APO-2014](https://doc.la.stueber.de/skripte_rlp-apo-2014.html) Wenn für einen Sportleistungskurs die praktischen Anteile nicht vollständig erbracht werden konnten, markieren Sie die Fachzeile in der Spalte `Merkmal`bitte mit dem Eintrag "ST"\(Sporttheorie\). Das Fach wird von der Automatik mit dem Fachstatus 3.PF markiert und nur einfach bewertet. Bitte beachten Sie die [Dokumentation für die Spalte "Merkmal"](https://doc.la.stueber.de/skripte_rlp-apo-2014.html#merkmal).
* NEW: SAC-APO-BGY-2017: [Bitte beachten Sie Dokumentation des Skriptes](https://doc.la.stueber.de/skripte_SAC-APO-BGY-2017.html)!
* NEW: BER-APO-2017: [Bitte beachten Sie die Dokumentation!](https://doc.magellan6.stueber.de/bundeslaender/berlin/oberstufe/ber-apo-2017.html)
* NEW: BER-APO-FW-2017: [Bitte beachten Sie die Dokumentation!](https://doc.magellan6.stueber.de/bundeslaender/berlin/oberstufe/ber-fw-apo-2017.html)
* NEW: BER-APO-KO-2017: [Bitte beachten Sie die Dokumentation!](https://doc.magellan6.stueber.de/bundeslaender/berlin/oberstufe/ber-apo-ko-2017.html)

### MAGELLAN-ADMINISTRATOR

* CHANGE: ungenutzte Punkte wurden ausgeblendet \(Datenexport, Unterkarte im Datenbankverbindung prüfen, einige Punkte unter Datenbankpflege &gt; Datenbank überprüfen\)

* NEW: Prüfung bei der Übernahme eines Lehrers aus MAGELLAN als Benutzer auf unerwünschte Zeichen im Kürzel

* NEW: beim Anlegen eines Benutzers ist der Account aktiv gesetzt

* NEW: Unter `Benutzerverwaltung > Benutzerliste > Benutzer editieren > Rechte` sind die ergänzenden Rechtefelder mit den niedrigsten Rechten vorbesetzt \(Beispiel: Verzeichnisse editieren ist voreingestellt als `nicht editierbar`\)

* NEW: eine neue Datenbankverbindung kann angelegt werden, während MAGELLAN parallel geöffnet ist

* NEW: Verbindungsname wird in der Statusleiste mit eingeblendet

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* SAR-GEMS-AS \(Klasse 9-10\).rpt
* SAC-BF-AZ \(B.03.04\).rpt
* SAC-FS-HJZ \(C.01.03\).rpt
* SAC-BG \(Punktekreditkarte-2010\).rpt
* Schuelerliste mit Barcode \(nach Klassen gruppiert\).rpt \(nun alphabetisch sortiert nach Schülernamen\)
* Schülerpersonalblatt incl. Schuleintritt und -austritt \(mit Vorbildung\).rpt
* Klassenlehrerliste mit Räumen.rpt
* Bewerber gruppiert nach Bewerberstatus.rpt \(alle Bewerberstatus nachgetragen, optimiert\)

## 6.0.182 - 663 \(15.03.2017\)

### MAGELLAN

* NEW: optionale Adressänderungen für Familienmitglieder, bitte beachten Sie unsere Dokumentation
["Adressanpassungen bei Familienmitgliedern"](https://doc.magellan6.stueber.de/howto/schueler.html#adressanpassungen-bei-familienmitgliedern). Geprüft und optional geändert werden die Felder:
* Straße
* Gebiet
* Ergänzung
* PLZ
* Ort
* Ortsteil
* Land

Diese Prüfung erfolgt bei Adressänderung für Schüler, Bewerber, Personen, Lehrer und Sorgeberechtigte, wenn Verweise auf Familienmitglieder über die Familienkarte eines Schülers oder Bewerbers bestehen.

* NEW: In der Liste der optional mit anzupassenden Familienmitglieder gibt es die Spalten "Verhältnis", dass das beim Schüler eingetragene Verhältnis zeigt, der Wert ist also immer aus Schülersicht. Zusätzlich wird in der Spalte "Ansicht" gezeigt, aus welcher MAGELLAN-Ansicht \(Schüler/Bewerber, Lehrer, Person, Sorgeberechtigte\) das Familienmitglied stammt.

![neu sind die Spalten &quot;Verhältnis&quot; und &quot;Ansicht&quot;](/images/liesmich/6.0.182.01.png)

* CHANGE: Unter `Schüler > Familie` wird in Klammern hinter dem, dem Schüler zugewiesenen Datensatz, die Ansicht aus der derjenige stammt wie folgt dargestellt:

![Hinter dem zugewiesenene Familienangehörigen, Sorgeberechtigtem oder Ansprechpartner wird gezeigt aus welcher Ansicht die Daten stammen](/images/liesmich/6.0.182.00.png)

### Skripte

Eine Anleitung für die Nutzung von Skripten finden Sie in der Dokumentation ["Landesanpassungen"](https://doc.la.stueber.de/).

* CHANGE:
 * MVP-APO-2010.dws: Wird das Fach "Musik" oder "Kunst" nicht unterríchtet, so wird es nicht ausgewertet.
 * Importiere SDTF: Korrektur für den Import des Lehrerunterrichtes pro Klasse aus Untis
 * RLP-APO-2014:
  * Wenn für das Fach Religion ein Kurs nicht durchgehend besucht wurde, sondern halbjahresweise aufgeteilt \(kat,ev,ethik\), wird jetzt korrekt markiert und gerechnet
  * Für einige Pflichtfächer wurde das Ergebnis der 13 nicht korrekt zum Einbringen markiert
  * Einbringungspflicht bei mehr als einem Fach der selben Kategorie korrigiert
  * Markierung für § 10 Absatz \(2\) Unterpunkt f.\) wurde korrigiert \(... in einer zweiten Fremdsprache oder in einer zweiten Naturwissenschaft oder in Informatik oder bei beruflichen Gymnasien in Informationsverarbeitung\)
  * Markierung für § 10 Absatz \(5\) wurde korrigiert \(Ist im neunjährigen Bildungsgang und im beruflichen Gymnasium innerhalb der Pflichtstundenzahl kein künstlerisches Fach durchgehend belegt worden, so sind die Kurse im künstlerischen Fach aus den Halbjahren 12/1 und 12/2 einzubringen. Wird dieses Fach in der Jahrgangsstufe 13 fortgeführt, so kann auch dieser Kurs, bei beruflichen Gymnasien können diese Kurse, eingebracht werden.\)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* NEW:
 * MVP-BS-AS-AZ\_Sonstige.rpt \(Zeugnis für Schüler, deren Fächer nicht in Lernbereiche unterteilt werden\)
 * SAC-FS-AZ \(C.01.06\).rpt
* CHANGE:
 * Kursliste Namen.rpt \(Auswahlfilter überarbeitet + nur aktive nicht gewechselte Schüler\)
 * Kursliste \(Zensurerfassung nach Lehrer gruppiert\).rpt \(Sortierung nach Nachnamen des Schülers\)
 * SAR-GEMS-AZ \(Klasse 5-10\).rpt
 * SAR-GEMS-HJZ-JZ \(Klasse 5-10\).rpt
 * RLP-GY-HJZ \(11-13\).rpt \(Spaltenbreite für Ausgabe Note und Punkte verändert\)
 * MVP-BS-AS-AZ.rpt \(Zeugnis für Schüler, deren Fächer in Lernbereiche unterteilt werden \(Berufsbezogener und Berufsübergreifender Lernbereich sowie Berufsbezogene Fremdsprache\)
* MVP-FG-AZ \(Vorstufe DINA4\).rpt

## 6.0.181 - 663 \(13.01.2017\)

* [Anleitung zum Einspielen eines Serviceupdate.](installation/update.md)
* [Probleme beim Einspielen des Updates?](installation/probleme-beim-update.md)

> #### warning::Wichtig
>
> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten.

### MAGELLAN

* NEW:\(Saarland\) Ansicht `Abitur > Registerkarte "Qualifikation`: Neue Registerkarten `Anmeldung` und `Rücktritt`. Auf der Registerkarte `Anmeldung` gibt es das neue Optionsfeld `Abitur angemeldet`.
* NEW: \(Saarland\) Ansicht `Abitur > Registerkarte Prüfung`: Neues Feld `Prüfungsstatus` mit den Werten `Nicht zum schriftlichen Abitur zugelassen`, `Nicht zum mündlichen Abitur zugelassen` und `Mündliche Abitur nicht bestanden`.
* NEW: \(Saarland\) Ansicht `Abitur > Auswahlliste`: Neue Spalten `Prüfungsstatus` und `Abitur angemeldet`.
* NEW: \(Saarland\) Ansicht `Schüler > Auswahl bzw. Daten 1`: Neues Feld `Stadtbezirk`.
* NEW:\(Saarland\) Ansicht `Bewerber > Auswahl bzw. Daten 1`: Neues Feld `Stadtbezirk`.
* NEW: `Extras > Statistik`: Neues Schnittstelle für die Landesstatistik im Saarland. Eine Dokumentation zur Schnittstelle finden Sie unter [http://doc.la.stueber.de](http://doc.la.stueber.de) im Abschnitt für das Saarland.
* NEW: unter Extras &gt; Optionen gibt es die neue Karte Mandanten. Bitte beachten Sie die [Dokumentation](https://doc.magellan6.stueber.de/admin/preferences.html#extras--optionen--mandanten)!
* NEW: unter Extras gibt es die neue Funktion `In Mandanten GUIDs abgleichen...`. Damit können zwischen als gleich erkannten Lehrern, Personen oder Sorgeberechtigten die GUIDs in bestehenden Datenbanken abgeglichen werden.
* NEW: Optional können mit gleichen GUIDs versehene Lehrer, Personen oder Sorgeberechtigte gleichzeitig geändert oder gelöscht werden. Beim Anlegen können Stammdaten aus anderen Mandanten für als gleich erkannter Lehrer, Sorgeberechtigter oder Personen übernommen werden. Bitte beachten Sie die [Dokumentation](https://doc.magellan6.stueber.de/admin/mehrmandantenloesung.html)!

* FIX: Versand von SMS an ungültige Mobilnummern korrigiert. Die ungültigen Mobilnummern werden beim Versand übersprungen und dies wird entsprechend im SMS-Protokoll ausgewiesen.

* FIX: Standardinstallationspfad für Datenordner bei der Server- und Einzelplatzinstallation \(Beispiel Windows10\): `C:\Users\Public\Documents\Stueber Systems\Magellan 6`

* FIX: Problem beim Anlegen von Bewerbern und Schülern behoben \(Anlegen von Schülern oder Bewerbern, Stammdaten eingeben, Ausbildung eingeben, speichern, Stammdaten fehlen\).

### Skripte

Eine Anleitung für die Nutzung von Skripten finden Sie in der Dokumentation [Landesanpassungen](https://doc.la.stueber.de/).

* CHANGE: Importiere SDTF.dws: Beim Übertrag des Lehrerunterrichts von DAVINCI nach MAGELLAN werden alle Unterrichtsarten berücksichtigt.

* CHANGE: Nordrhein-Westfalen Abiturskript für Allgemeinbildende Schulen NRW-APO-2102.dws

* NEW: neue Fachwahlskripte \(Gymnasium und Wirtschaftsgymnasium\) für Hessen, für die Anleitung klicken Sie bitte auf die Links:

* [HES-FW-APO-BGY-2015.js](https://doc.la.stueber.de/fachwahl/hes-fw-apo-bgy-2015js.html)
* [HES-FW-APO-2015.js](https://doc.la.stueber.de/fachwahl/hes-fw-apo-2015js.html)

* NEW: neues Abiturberechnungsskript für Wirtschaftsgymnasien in Hessen, für die Anleitung klicken Sie bitte auf die Links:

* [HES-APO-BGY-2015.dws](https://doc.la.stueber.de/hes-apo-bgy-2015.html)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE:

* Rentenbescheid.rpt
* Medienliste \(Inventur\).rpt
* Kursliste \(Zensurerfassung nach Lehrer gruppiert\).rpt
* SAR-GEMS-AZ \(Klasse 5-10\).rpt
* SAC-BG-HJZ \(E.01.01\).rpt
* SAC-FO-HJI \(D.01.01\)\(Fachpraktischer Unterricht\).rpt \(hier wird nun auch der Fachpraktische Unterricht mit ausgegeben\)




