# Änderungen 2016

## 6.0.180 (28.10.2016)

### MAGELLAN

* korrigiert: `Personen > Daten > Strasse`: Speichern von 100 Zeichen, anstatt 30 Zeichen.
* korrigiert: Für alle Kollegiumsrechte (Kollegium 1-5) wird der Tutor unter ```Auswahl > Schüler``` gezeigt.
+ geändert: Beim Übertrag des Lehrerunterrichts von DAVINCI nach MAGELLAN werden alle Unterrichtsarten berücksichtigt.
+ Neu: Neues Modul "MAGELLAN Abitur" für Auslandsschulen, Sonderversion von MAGELLAN zur ausschließlichen Nutzung der Verordnungen DRP und DIAP.

#### Statistik
##### RLP-BBS-Bewegungsdaten
* korrigiert: YBildungsgang: Der Schülerbildungsgang wird vor dem Klassenbildungsgang berücksichtigt.

##### RLP-BBS-Neuanlagedaten
* korrigiert:  Plausibilität STALA 12850
* korrigiert: Plausibilität STALA-14400
* korrigiert: Ausspielen der leeren Vorbildungsdaten für Schüler die in den Bildungsgang 8610081 gewechselt sind, zurückgenommen. Lt. Aussage des Amtes Mussfelder.
* korrigiert: Ausspielen der leeren Neuzugangs- und Vorbildungsdaten für Schüler die in den Bildungsgang 8610081 gewechselt sind
* korrigiert: Plausibilität STALA-27150-1, Berücksichtigung der BVJ Schlüssel.
* korrigiert: Ausspielen der Ausbildungsberufe für Y-Bildungsgänge 8101050 und 8101060 \\(BVJ\\) verhindert.
* geändert: Das Amt hat die Plausibilitäten 29020 und 29430 um Zugang mit Schulform 990 erweitert.
* korrigiert: Plausibilität STALA-29275
* korrigiert: Ausspielen der Ausbildungsberufe für Y-Bildungsgänge 8101050 und 8101060 \(BVJ\) verhindert.
* korrigiert: STALA 25930-2 Schulform: Bei angegebenem Bildungsgang \(8204\*\) sind nur die Klassenstufen 1-2 zulässig, Klassenstufe war jedoch korrekt
* korrigiert: STUEBER -20-2 wird das BVJ - Sprachförderung nicht berücksichtigt 
* geändert: Das Amt hat die Plausibilitäten 29020 und 29430 um Zugang mit Schulform 990 erweitert.
* korrigiert: Plausibilität STALA-29275
* korrigiert: Plausibilität STALA-27150-1: Berücksichtigung der BVJ Bildungsgänge
* korrigiert: Plausibilitäten STALA-39720-2 STALA-39720-6 entfernt, da veraltet.
* korrigiert: Plausibilität STALA-37600\/MORGEN-170, berücksichtigt jetzt BVJ-S
* korrigiert: Plausibilität STUEBER-20-2, berücksichtigt jetzt BVJ-S
* korrigiert: Plausibilität STUEBER-23, berücksichtigt jetzt BVJ-S

##### RLP-BBS-Lehrerdaten
* korrigiert: Lehrer, die nach dem letzten Statistiktermin an Ihre Schule wechselten und vor dem aktuellen Statistiktermin Ihre Schule verlassen haben, werden statistisch nicht an Ihrer Schule ausgewertet, sollen also nicht in Ihrer Lehrer.xml erscheinen. Sie werden statistisch an der Herkunftschule als Abgang und an der neuen Schule als Zugang geführt.
* korrigiert: Ausspielen des Feldes "DienstHerr"
* korrigiert: Ausspielen der SchulFormStufe für BVJ im Zusammenhang mit Förderschul-Lehrkraft Schlüssel 73.
* korrigiert: Fehlende Schlüssel in der Importdatei der Lehrer Beschäftigungsverhältnisse korrigiert. Importdatei heisst jetzt 00\_Beschaeftverh.keys und enthält alle Schlüssel, da diese sowohl für ABS als auch BBS gelten.
* korrigiert: Plausibilität STALA-5850-1
* korrigiert: Ausspielen der SchulFormStufe für BVJ-S Schlüssel 83 berücksichtigt
* korrigiert: Ausspielen der SchulFormStufe für BVJ-S Schlüssel 83. Erweiterte Korrektur!
* korrigiert: Plausibilität STALA-5850-1 
* korrigiert: Ausspielen der SchulFormStufe für BVJ-S Schlüssel 83 berücksichtigt

##### RLP-ABS-Neuanlagedaten
* geändert: Die 2.Fremdsprache wird ausgelesen wenn, die Klassenstufe größer/gleich 6 ist, die Schulart  20 (Realschule), 21 (Realschule Plus) oder  40 (IGS) und der Fremdsprachenstatus 6 (Wahlpflicht) **oder 2 (Wahlfach (fakultativ))** ist. Bitte beachten Sie in der Dokumentation auch den Abschnitt "ABS: Wann wird die 2.Fremdsprache ausgegeben?". 
* korrigiert: In der Bewegungsdatei wurden nicht die Abiturnoten der G8-Abiturienten ausgegeben, bitte tauschen Sie die lokale MAGELLAN.exe aus.
* korrigiert: Plausibilität STALA-14400

##### RLP-ABS-Bewegungsdaten
* korrigiert:Für einen weiteren Fall wird die 2.Fremdsprache mit ausgegeben, bitte tauschen Sie die lokale MAGELLAN.exe aus




### MAGELLAN-ADMINISTRATOR

* korrigiert: Fehler beim Löschen der Magellan-Datenbank behoben. 

### Berichte (neu oder geändert)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* geändert:

  * SHL-GY-AS \(Klasse 5-10\)\(G9\).rpt
  * SHL-GY-AS \(Klasse 5-10\)\(G8\).rpt
  * SHL-GY-HJZ \(Profil\).rpt
  * Noch nicht zurueckgegebene Exemplare pro Schueler \(nach Klassen gruppiert\).rpt durch

    * Offene Ausleihvorgänge \(nach Klassen gruppiert\).rpt
    * Offene Ausleihvorgänge \(nach Schüler gruppiert\).rpt

  * Bescheinigung zur Rentenversicherung \(V0510 - 30.09.2014\).rpt



* neu: 
  * Klassenliste mit Arbeitsgemeinschaften \(max. 2\).rpt

## 6.0.179 662 (16.08.2016)

### MAGELLAN

* geändert: Anzeige der Landesstatistik 2016 unter `Hilfe > Lizenz`
* korrigiert: Eingabe einer neuen Fahrroute unter Daten4
* geändert: Umbenennung des Spaltenkopfes unter `Verzeichnisse > Fahrschüler > Verkehrslinien`. "Operator \(Adressen\)" statt "Operator".
* korrigiert: beim Wechsel des "Jahrgangs" \(`Abitur > Qualifikation > Jahrgang`\) werden 10 Zeichen des Wertes aus dem Verzeichnis "Abschlussjahrgänge" geprüft.
* korrigiert: Bei der Sammelzuweisung unter `Schüler > Laufbahn` kann mit der Sammelzuweisung auch das Abschlussdatum2 gesetzt werden.
* Korrigiert: Aus dem Menü Berufsschule klappt wieder Drucken > Zeugnis/Berichte > Exportieren nach PDF/Drucken und Exportieren nach PDF.

###Statistik
* Neu:   Nordrhein-Westfalen Statistikmodul ABS und BBS 2016. Beachten Sie bitte die aktualisierten Schlüsselverzeichnisse und die Anleitung:  [Landesstatistik NRW](http://doc.ls.stueber.de/nrw/nordrhein-westfalen_-_abs_und_bbs.html) 
* Neu:   Schleswig-Holstein Statistikmodul 2016. Beachten Sie bitte die aktualisierten Schlüsselverzeichnisse und die Anleitung: [Landesstatistik SHL](http://doc.ls.stueber.de/shl/schleswig-holstein.html)  

### MAGELLAN-ADMINISTRATOR
* Neu: SHL => ```Unter Datenbankpflege > Datenbank überprüfen``` gibt es eine neue Funktion zum Korrigieren des Fächerverzeichnisses für die Statistik in SHL. Bitte beachten Sie dazu den Abschnitt ["Verzeichnis Fächer (ABS/BBS) korrigieren"](http://doc.ls.stueber.de/shl/schleswig-holstein.html#Verzeichnis Fächer ABS/BBS korrigieren) in der Anleitung.

### Importe
* Neu: Schlüsselkataloge für allgemeinbildende Schulen in NRW:  
  * AS_Herkunftsarten.keys
  * AS_KlassenMerkmale.keys

### Berichte (neu oder geändert)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* geändert: Schüler-Abschlussbericht\(Schulabgänger\).rpt 


## 6.0.178 662 (12.07.2016)

### MAGELLAN

* Neu: Rheinland-Pfalz Statistikmodul 2016. Beachten Sie bitte die aktualisierten Schlüsselverzeichnisse. [Die Statistikdokumentation für RLP finden Sie hier.](http://doc.ls.stueber.de/rlp/rheinland-pfalz_-_abs_und_bbs.html)

### MAGELLAN-Administrator

* Korrigiert: Umschalten des Mandanten im Dialogfenster "Benutzer bearbeiten" wirkt sich jetzt auf die Anzeige der Medienkataloge Registerkarte "Rechte" aus.
  
### Skripte

Eine Dokumentation aller Skripte finden Sie unter [http://doc.la.stueber.de](http://doc.la.stueber.de)

* Korrigiert: [NRW-APO-2012](http://doc.la.stueber.de/skripte_nrw-apo-2012.html) 
* Korrigiert: [NRW-APO-BK-2012](http://doc.la.stueber.de/skripte_nrw-apo-bk-2012.html)

### Importe

* Geändert: Für das Saarland wurden die Kürzel auch als Schlüsselwerte in der Datei BS_Faecher.keys ergänzt.
> Bitte beachten Sie vor dem Import der Datei BS_Faecher.keys (enthält die Lernfelder) die [**Anleitung**](http://doc.magellan6.stueber.de/more/saarland_lernfelder_importieren.html).
* Neu: Für Nordrhein-Westfalen (ABS) stehen die Dateien AS_Fachgruppen.keys und AS_Fachniveaus.keys zur Verfügung

### Berichte (neu oder geändert)

+ Neu: Zeugnis "NRW-GES-JZ-HJZ (5-9.1_10.1).rpt"
+ Neu: Zeugnis "NRW-GY-JZ-HJZ (5-9).rpt"
+ Neu: Zeugnis "NRW-GES-AS (A3, 10.2).rpt"
* Geändert: Klassenliste (Schüler mit Verhaltens- oder Mitarbeitsnoten blanko).rpt (Feldhöhe Fach erweitert)
+ Neu: Saarland -> wir veröffentlichen vom saarländischen Ministerium für Bildung und Kultur bereitgestellte Berichte:
  + Zeugnisse unter: Drucken > Zeugnisse > Saarland > Ministerium:
     * SAR-BS-AGZ Lernfeld MBK.rpt
     * SAR-BS-AS-Lernfeld A3 MBK.rpt
     * SAR-BS-HJZ-Lernfeld MBK.rpt
     * Anleitung: MBK - Zeugniserstellung nach dem Lernfeldkonzept mit MAGELLAN.pdf
  + Klassenberichte unter: Drucken > Berichte > Saarland > Ministerium:
     * SAR-Klassen-Notenliste Abgeschlossene Lernfelder MBK.rpt
     * SAR-Klassen-Notenliste Halbjahr Lernfeld MBK.rpt
    
## 6.0.177 662 (15.06.2016)
 
### MAGELLAN

* Neu: Unter "Verzeichnisse|Fächer" gibt es die neue Kategorien "Pädagogik" und "Literatur".
* Korrigiert: Ansicht "Schüler|Laufbahn|Allgemein: Fehlende Felder sind wieder eingeblendet.

### MAGELLAN-Administrator

* Geändert: Der Import des Schlüsselverzeichnisses Fächer wurde um die Felder "Zeugnismerkmal" und "Bezeichnung2" erweitert.

### Skripte
Eine Dokumentation der Skripte finden Sie unter [http://doc.la.stueber.de](http://doc.la.stueber.de)

* Korrigiert: [DE-DIAP-2005.dws](http://doc.la.stueber.de/skripte_de-diap-2005.html), Fehler behoben
* Korrigiert: [DE-DRP-2005.dws](http://doc.la.stueber.de/skripte_de-drp-2005.html), Fehler behoben  
* Korrigiert: [SAR-APO-2007.dws](http://doc.la.stueber.de/skripte_sar-apo-2007.html), Fehler behoben  
* Korrigiert: [RLP-APO-BGY-2014.dws](http://doc.la.stueber.de/skripte_rlp-apo-bgy-2014.html) 
  * beliebige Kurse der 2.Fremdsprache können eingebracht werden
  * bitte markieren Sie die 2.Fremdsprache mit Fachstatus "Freiw"
  * BWL oder VWL muss nicht eingebracht werden
* Korrigiert: Importiere SDTF.dws.

### Importe
* Neu: Für das Saarland stehen die Dateien BS_Faecher.keys und BS_Berufe.keys zur Verfügung. 
> Bitte beachten Sie vor dem Import der Datei BS_Faecher.keys (enthält die Lernfelder) die [**Anleitung**](http://doc.magellan6.stueber.de/more/saarland_lernfelder_importieren.html).

### Berichte (neu oder geändert)

+ Erweitert: Bewerberpersonalblatt.rpt enthält jetzt die Ausgabe des Praxisbetriebes.
+ Neu: SAR-BS-AS-Lernfeld MBK A3.rpt (erstellt vom Ministerium für Bildung und Kultur Saarland)
+ Neu: SAR-BS-HJZ-Lernfeld MBK.rpt(erstellt vom Ministerium für Bildung und Kultur Saarland)
+ Neu: SAR-Klassen-Notenliste Abgeschlossene Lernfelder MBK.rpt(erstellt vom Ministerium für Bildung und Kultur Saarland)
+ Neu: SAR-Klassen-Notenliste Halbjahr Lernfeld MBK .rpt
+ Neu: Etiketten (Dymo 99010, 28x89).rpt
+ Neu: Etiketten (Dymo 99012, 36x89).rpt
+ Neu: Zeugnis "BAW-BG-AS.rpt"
+ Neu: Zeugnis "BAW-BG-AS (Variante mit Endnote Gesamt).rpt"
+ Neue Fassung: "BER-GY-JZ (Schul Z 250)(02.15).rpt"
+ Angepasst: "Unfallanzeige.rpt" und "Unfallanzeige (mit Erläuterungen).rpt" entsprechend der Änderungen in Magellan wird hier der erste Familienangehörige angezeigt, der den Haken "Sorgerecht" hat oder, wenn keiner mit Haken vorhanden, dann der erste mit Benachrichtigung "immer".
+ Korrigiert: Zeugnis "BER-Schul Z 303 (05.16).rpt", Anzeige personalisierter Zeugnisbemerkungen möglich
+ Neue Fassung: Aufgrund von Ablehnungen bei Ämtern wurde der Schülerbericht "Rentenbescheid.rpt" auf die aktuelle Vorlage V0510 der Deutschen Rentenversichung umgesetzt und nennt sich jetzt "Bescheinigung zur Rentenversicherung (V0510 - 30.09.2014).rpt"

## 6.0.176 662 (26.05.2016)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](http://doc.magellan6.stueber.de/installation/serviceupdates.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](http://doc.magellan6.stueber.de/installation/troubleshootingupdate.html).

### Datenstruktur

 * Neu: Felder "Fremdsprache1Referenz" ... "Fremdsprache4Referenz" in Tabelle "Schueler"
 * Neu: Schlüsseltabelle "Sprachreferenzen"
 
### MAGELLAN

* Neu: "Verzeichnisse|Weitere Schlüsselverzeichnisse: Neues Schlüsselverzeichnis "Sprachreferenzen" für möglichen Kompetenzen nach dem Gemeinsamen europäischen Referenzrahmen für Sprachen (GeR).   
* Neu: Ansicht "Schüler"/"Bewerber": Auf der Registerkarte "Daten 3" kann man jetzt für die Fremdsprache unter "Referenz" die Sprachreferenz aus dem neuen Schlüsselverzeichnis "Sprachreferenzen" eintragen.
* Neu: Berliner Masken: Ansicht "Schüler/in"/"Bewerber/in": Auf der Registerkarte "Sekundarstufe I" bzw. "Sekundarstufe II" kann man jetzt für die Fremdsprache unter "Referenz" die Sprachreferenz aus dem neuen Schlüsselverzeichnis "Sprachreferenzen" eintragen.
* Neu: für die Berliner Masken wurde in der Sammelzuweisung die Sprachreferenz für "SekI" und "SekII" ergänzt.
* Neu: Ansicht "Abitur"|Auswahl: Neue Spalte "Verordnung" zur Anzeige der jeweiligen Verordnung des Schülers.

### MAGELLAN-Administrator

* Aktualisiert: Spalte "Muendlich" zum Import der Schueler_Fachdaten.csv hinzugefügt.
* Neu: unter Importe|Deutschland und für alle Bundesländer gibt es als importierbare Schlüsseldatei "00_Sprachreferenzen.keys"

### Skripte

Eine Dokumentation aller Skripte finden Sie unter [http://doc.la.stueber.de](http://doc.la.stueber.de)
+ Korrigiert: DAS-DRP-2005.dws, Fehler behoben
+ Aktualisiert: BER-APO-KO-2011.dws, Gesamtnote für die besondere Lernleistung wird berechnet 
+ Korrigiert: RLP-APO-2014.dws, Fehler behoben

### Berichte (neu oder geändert)

+ BER-Schul Z 301 (05.16).rpt
+ BER-Schul Z 303 (05.16).rpt
+ BER-Schul Z 306 (05.16).rpt
+ BER-Schul Z 324 (03.16).rpt
+ Etiketten (Dymo 99012, 89x36).rpt
+ Klassenliste Schüler-Notenmatrix (Querformat-Durchschnitt, sortiert).rpt
+ Klassenliste Schüler-Notenmatrix (Querformat-Durchschnitt, unsortiert).rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 2).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-GY-ABI (2010-G8-G9)A4.rpt
+ RLP-GY-JZ JG 10 (G8).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ Kursliste Namen.rpt
+ Neu: Schülerliste (Klasse, Geburtsdaten, Adresse, Telefon, sortiert nach Schüler).rpt
+ Umbenannt:Schülerliste (Klasse, Geburtsdaten, Adresse, Telefon, sortiert nach Klasse).rpt

### 6.0.175 661 (04.05.2016)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Datenstruktur

* Neu: Felder "RuecktrittNachZulassung" und "RuecktrittFolgenlos" in Tabelle "SchuelerABI"

### MAGELLAN

+ Neu: "Ansicht Abitur|Qualifikation": Neue Felder "Rücktritt nach Zulassung" und "Rücktritt folgenlos".
+ Neu: Beim Drucken von Berichten wird im Dialogfenster zur Auswahl der Berichte die Spaltenbreite automatisch an den längsten Berichtsnamen angepasst.
+ Korrigiert: Berliner Masken für Schüler/Bewerber: Fehler bei Neuanlage eines Schülers/Bewerbers mit Ausbildungsbetrieb behoben.
+ Neu: Berlin: Die Abiturschnittstelle 2016 steht jetzt zur Verfügung. Beachten Sie dazu auch die aktualisierte Dokumentation für Berlin im Dokument [Magellan Berlin](ftp://ftp.stueber.de/pub/doc/de/schulverwaltung/dokumentation/Magellan6Berlin.pdf).
+ Korrigiert: Seriendruck an Sorgeberechtigten=> Sorgebe_Anrede wird wieder korrekt übergeben


### MyMAGELLAN-Center

+ Korrigiert: Fehler beim Import behoben.

### MAGELLAN BIBLIOTHEK

+ Neu: Ansicht "Ausleihe": Anzeige der aktuellen Vorgänge eines Ausleihers, auch wenn dieser inaktiv oder die Ausleiherlaubnis erloschen ist. 
 
### Skripte

+ Korrigiert: DAS-DRP-2005.dws, Fehler bei der Berechnung der Prüfungssumme behoben

### Berichte (neu oder geändert)

+ Offene Medienvorgänge (bis zum heutigen Tag).rpt: Dieser Bericht listet alle offenen Medienvorgänge auf, dessen Ausleihedatum vor dem Druckdatum liegen. Es werden Informationen zum Medium, Exemplar und Ausleiher ausgegeben.
 
## 6.0.174 660 (14.04.2016)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Datenstruktur

* Neu: Felder "UpdateTry" und "UpdateError" in Tabelle "Version"

### Magellan

* Neu: Datenstrukturupdates können nur noch ausgeführt werden, wenn die Mindestanforderungen an die Strukturupdates gegeben sind. Diese sind zum aktuellen Zeitpunkt:
    * Firebird-Version: 2.5.2.X
    * ODS-Version der Magellan-Datenbank: 11.2
    * Nur ein Benutzer an der Magellan-Datenbank angemeldet
    * Nur als Benutzer "SYSDBA" angemeldet        
* Die Funktionalität wurde um eine Prüfung aller Mindestvoraussetzungen erweitert. Im Falle, dass diese nicht übereinstimmen, erhalten Sie eine detaillierte Meldung zur weiteren Vorgehensweise. Zudem ist das angebotene Sichern der Magellan-Datenbank vor dem Strukturupdate jetzt zwingend erforderlich ist (zuvor optional).
+ Korrigiert: Registerkarte "Bewerber|Sorgeberechtigte" umbenannt in "Bewerber|Familie"
+ Korrigiert: Anlegen eines neuen Schüler und direkt Anlegen eines neuen 
    Sorgeberechtigten führte zu Fehler, da der neue Schüler in der 
    konkurrierenden Datenmenge noch nicht erkannt wurde.
+ Verbessert: Ein Fehler der beim Bewerber, anlegen/bearbeiten von Ausbildungen 
    "Operation bei geschlossener Datenmenge" kann nicht richtig nachvollzogen 
    werden. Es wurden einige Verbesserungen eingeführt, die das Problem evtl. 
    beheben (Status: Unter Beobachtung).
+ Neu: Für NRW: Unter "Verzeichnisse|Fachtafeln" gibt es 
    - für Fachtafeln das neue Feld "Mündlich" pro Fach
    - für Fachwahltafeln die neuen Felder "E1 Mündlich", "E2 Mündlich", "Q1 Mündlich",
    "Q2 Mündlich","Q3 Mündlich" und "Q4 Mündlich".
+ Neu: Für NRW: Unter "Ansicht Schueler|Zeugnisse|Fächer" gibt es das neue Feld "Mündlich" pro Fach.
    Damit kann man festhalten, ob das Fach nur mündlich benotet wird.
+ Neu: Für NRW: Unter "Ansicht Abitur|Qualifikation" gibt es die neuen Felder "E1 Mündlich", 
    "E2 Mündlich", "Q1 Mündlich", "Q2 Mündlich","Q3 Mündlich" und "Q4 Mündlich" pro Fach.
    Damit kann man festhalten, ob das Fach mündlich benotet wird.
+ Neu: Für NRW: Unter "Ansicht Abitur|Fachwahlen" gibt es die neuen Felder "E1 Mündlich", 
    "E2 Mündlich", "Q1 Mündlich", "Q2 Mündlich","Q3 Mündlich" und "Q4 Mündlich" pro Fach.
    Damit kann man festhalten, ob das Fach in den einzelnen Halbjahren mündlich belegt wird.
+ Neu: Unter "Ansicht Schüler|Zeugnis|Details" gibt es das neue Feld "Zeugnisdatum 2"
+ Korrigiert: "Ansicht Sorgeberechtigte|Arbeitgeber": Fehler bei der Anzeige behoben.
+ Neu: Neue Vorlagen für den Seriendruck: 
	* Brief an Praxisbetrieb des Schülers.dot
	* Brief an Praxisbetrieb des Bewerbers.dot
       
### Magellan-Bibliothek

+ Korrigiert: Ansicht "Schueler|Daten", Anzeige der Schüler-Stammdaten in 
    vergangenen Zeiträumen
+ Korrigiert: Aktualisierung der offenen Nachschlage-Datenmengen, wenn 
    Schlüsselverzeichnisse geändert werden.      
+ Korrigiert: Der Exemplarstatus wird jetzt nicht mehr aus dem Statusfeld der 
    Tabelle MedienExemplare gelesen, sondern direkt aus den vorhandenen 
    Ausleihvorängen berechnet. Damit kann es nicht mehr vorkommen, dass 
    abgeschlossene Ausleihvorgänge im Exemplarstatus noch als ausgeliehen 
    dargestellt werden und ggf. bereits sich noch in befindliche Vorgängen 
    als frei dargestellt sind.

### MyMagellan-Center

+ Neu: Sie können jetzt einstellen, ob die Felder "Unterrichtstage" und "Versäumnisse" sichtbar 
  und editierbar sind.
+ Neu: Sie können jetzt einstellen, ob die Felder "Zusatz Note 1" ... "Zusatz Note 9",
  "Vornote" und "Beurteilung" sichtbar und editierbar sind.
+ Neu: Beim Verteilen der Dateien wird bei der Auswahl der sichtbaren Spalten jetzt auch der Originalname der Spalte zusätzlich mit angezeigt

### Skripte

+ korrigiert: SAR-APO-2007.dws
+ neu: SHL-APO-2015.dws
+ neu: DAS-DRP-2005.dws, Skript zur Berechnung der Reifeprüfung an Deutschen Auslandsschulen
+ neu: RLP-APO-G8-2014.dws (bitte unter  Verzeichnisse|Verordnungen einrichten und in der Spalte Typ G8 eintragen)

### Berichte (neu oder geändert)

+ BAW (Notenkonferenzliste).rpt
+ Aktive Ausleihvorgaenge pro Schueler (nach Klassen gruppiert).rpt
+ BAW (Notenkonferenzliste).rpt
+ BER-GY (abi_4_berechnungsbogen)(09.12).rpt
+ Kursliste (Zensurerfassung nach Lehrer gruppiert).rpt
+ MVP-FOS-AS-AZ.rpt
+ Quittung (Leihvertrag Taschenrechner).rpt
+ SAR-FHReife (Nachweis).rpt
+ SHL-GY-ABI (2011).rpt
+ DAS-GY-ABI-Reifepruefung.rpt
+ RLP-GY-Punktekreditkarte-2012.rpt (überarbeitet, klappt für G8 und G9 [Verzeichnisse|Verordnungen|Spalte "Typ" bitte G8 eintragen oder für G9 leer lassen])
  
## 6.0.173 659 (11.03.2016)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Datenstruktur

+ Neu: Felder "Lehrer", "Person", "Geschwister","Familiennr", "Sorgerecht" in Tabelle "SchuelerSorgebe" hinzugefügt
+ Neu: Ansicht "SchuelerFamilie" über die Tabellen "Schueler", "Personen", "Lehrer" und "Sorgebe"      
+ Neu: Tabellen "TransportationMethods", "TransportationRoutes", "TransportationStops", "TransportationLines", "StudentRoutes", "StudentTransportation"
+ Neu: Tabellen "MedizinArten", "MedizinKategorien", "SchuelerMedizinDaten",      "SchuelerMedizinAkten", "LehrerMedizinDaten", "LehrerMedizinAkten", "PersonenMedizinDaten", "PersonenMedizinAkten"
+ Neu: Ansichten "MedizinDaten", "MedizinAkten"
+ Neu: Tabellen "Schulgeldarten", "SchuelerSchulgeld"

### Magellan

+ Korrigiert: Anlegen eines Sorgeberechtigten aus der Ansicht Schüler|Sorgeberechtigten 
+ Korrigiert: Anzeige des verkehrten Klassenleiters beim Aufruf eines Schülers aus der Auswahlliste behoben 
  (Datensatz einfach anklicken, Auswahl Daten1 mit linker Maustaste)
+ Korrigiert: Zugriffsverletzung beim Aufruf der Bewerberliste
+ Neu: Unter "Verzeichnisse|Medizin" gibt es die neuen Schüsselverzeichnisse "Medizinarten" und
  "Medizinkategorien". Diese werden auf der neuen Registerkarte "Medizin" verwendet
+ Neu: Unter den Ansichten "Schüler", "Bewerber", "Lehrer", "Personen" gibt es eine neue 
  Registerkarte "Medizin" zur Erfassung medizischer Stammdaten und einer medizinischen Akte. 
+ Neu: "Extras|Optionen|Register Ein-/Ausblenden" - Über die neuen Optionsfelder 
  - "Register "Medizin" in  Ansicht "Schüler" bzw. "Bewerber" ausblenden" 
  - "Register "Medizin" in  Ansicht "Lehrer" bzw. "Bewerber" ausblenden" 
  - "Register "Medizin" in  Ansicht "Personen" ausblenden" 
  können Sie die Registerkarte "Medizin" in den Ansichten "Schüler", "Bewerber", "Lehrer"
  bzw "Personen" ein- oder ausblenden. 
+ Neu: Unter den Ansichten "Schüler" bzw. "Bewerber" gibt es eine neue 
  Registerkarte "Schulgeld" zur Erfassung der Schulgelder. 
+ Neu: "Extras|Optionen|Register Ein-/Ausblenden" - Über das neue Optionsfeld 
  "Register "Schulgeld" in  Ansicht "Schüler" bzw. "Bewerber" ausblenden" 
  können Sie die Registerkarte "Schulgeld" in den Ansichten "Schüler" bzw. "Bewerber" ein- oder ausblenden.     
+ Änderung: In den Ansichten "Schüler" bzw. "Bewerber" ist die Registerkarte "Sorgeberechtigte" 
  in "Familie" umbenannt worden. Neben Sorgeberechtigten kann man dort jetzt auch Geschwisterkinder,
  Lehrer oder Personen als Mitglieder der Familie zuordnen.
+ Neu: In den Ansichten "Schüler" bzw. "Bewerber" gibt es auf der Registerkarte "Familie" zusätzlich
  die Felder "Familiennummer" und "Sorgerecht"
+ Neu: In den Ansichten "Schüler" bzw. "Bewerber" kann man auf der Registerkarte "Familie" zusätzlich
  unter "Verhältnis" 10 weitere Verhältnisse auswählen. Diese Verhältnisse können unter
  "Verzeichnisse|Bezeichnungen anpassen" unter "Ansicht Schüler/Bewerber" iun den Zeilen 
  "Verhältnis 1" ... "Verhältnis 10" frei definiert werden. 
+ Neu: Unter "Verzeichnisse|Fahrschüler" gibt es die neuen Schüsselverzeichnisse "Verkehrslinien", 
  "Fahrstrecken und Haltestellen" und "Verkehrsmittel". Diese werden in der Ansicht "Schüler" auf 
  der Registerkarte "Daten 4" verwendet.
+ Neu: Unter den "Ansichten Schüler|Daten 4" gibt unter dem Bereich "Fahrtstrecken" die neuen Felder
  "Hinweg" und "Rückweg". 

### Statistik 

+ MVP-SIP: Korrektur der Ausgabe der Knoten "SchulartId" bei Schüler und Klassen
+ MVP-SIP: Wichtige Ergänzungen im Landesstatistiken.pdf für die 
  Fremdsprachen Von und Bis Felder
  
### Importformat

+ sorgebe.import.csv: Geburtsland für den Import der Sorgeberechtigten ergänzt.  

### Berichte (neu oder geändert)

+ BAW (Notenkonferenzliste).rpt
+ Bewerber nach Herkunftsschulen und Klassen.rpt
+ Klassenliste (Klassenlehrer mit Foto).rpt
+ Klassenliste Schüler-Notenmatrix (Querformat-Durchschnitt).rpt
+ MVP-FG-ABI (2015).rpt
+ MVP-FOS-AS-AZ.rpt
+ SAC-BS-AS (A.02.05).rpt
+ SAC-FS-AS mit FHR (C.01.14).rpt
+ Schülerausweis ohne Photo.rpt
+ SHL-GY-AZ (A3).rpt

### 6.0.172 658 (29.02.2016)

#### Magellan

+ Korrigiert: Fehler beim Aufruf der Ansichten "Schüler" und "Abitur" am 29.02.2016 behoben.
+ Korrigiert: "Benutzerrechte zuweisen" - Schreibfehler führte zum Abbruch des Skriptes

#### Skripte

+ Neu: DE-DIAP-2005.dws für Auslandsschulen. Beinhaltet die Berechnung gemäß der Deutschen Internationalen
       Abiturprüfung an Auslandsschulen. Ersetzt das bisherige Skript DE-APO-2015.dws.

### 6.0.171 658 (08.02.2016)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

#### Magellan

+ Korrigiert: im Seriendruck werden Schattenkopien unterdrückt
+ Neu: Unter Schüler|Zeugnis|Leistungen gibt es das Feld Vornote
+ Neu: "Ansicht Betriebe|Kontakte" - Für jeden Kontakt kann jetzt auch die Mobilnummer festgehalten werden
+ Neu: "Ansicht Sorgeberechtigte" - Neue Registerkarte "Arbeitgeber" zum Festhalten des Arbeitgebers des
  Sorgeberechtigten inkl. seiner Abteilung und Position.
+ Neu: "Ansicht Sorgeberechtigte|Auswahl" - hier können Sie zusätzliche die Spalten mit den Inhalten der 
  neuen Registerkarte "Arbeitgeber" einblenden lassen.
+ Neu: Beim Seriendruck an Sorgeberechtigte können zusätzlich die Felder der neue Registerkarte 
  "Arbeitgeber" verwendet werden. 
+ Neu: "Extras|Optionen|Register Ein-/Ausblenden" - Über das Optionsfeld "Register "Arbeitgeber" in 
  Ansicht "Sorgeberechtigte" ausblenden" können Sie das Register "Arbeitgeber" in der Ansicht "Sorgeberechtigte"
  ein- oder ausblenden.
+ Neu: "Ansicht Schüler|Bearbeiten|Fehlzeiten": Die Anzahl der Fehlstunden werden jetzt als Kommazahl gespeichert.
+ Neu: "Extras|Gruppen benachrichtigen": Jetzt können Sie auch Mitteilungen an die Schüler oder Sorgeberechtigte eines 
  Verkehrsmittels, was der Schüler nutzt, senden.
+ Neu: Beim Drucken über Crystal Reports aus den Ansichten "Schüler|Bewerber|Klassen|Lehrer|Mandanten|Personen|Sorgebrechtigte|Betriebe|
  Schulen|Adressen" kann man jetzt optional über "Export nach PDF" die Berichte nach PDF exportieren, ohne die Berichte zu drucken. 
  Dies steht nur dann zur Verfügung, wenn unter "Extras|Optionen|Registerkarte Dokumente|Registerkarte Crystal Reports" die jeweiligen 
  Dokumentenordner aktiviert worden sind.
+ Korrigiert: Allgemein: Anzeige des Klassenleiters unter "Ansicht Schüler|Daten 1" nach Wechsel aus anderem Menü
+ Korrigiert: Berlin: Anzeige des Klassenleiters in der "Ansicht Schüler" unter Grundstufe, Berufsbildung, SekI, SekII
+ Korrigiert: Berlin: auf der Karte Berufsbildung wechselt man per Doppelklick auf den Ausbildungsdatensatz ins Betriebemenü

#### Magellan-Administrator
+ Neu: Importformat|Import der Sorgeberechtigten um Felder "Staatsangeh1", "Staatsangeh2", 
  "Muttersprache", "Verkehrssprache" erweitert  
    
#### Skripte:
+ Korrigiert: "Synchronisiere Zugriffsrechte" und "Benutzerrechte zuweisen" wurden ergänzt um die Rechte für die Verzeichnisse 
  Staaten, Gebiete und Gebietsarten   
+ Korrigiert: RLP-APO-2014.dws: Wenn Religion und Ethik belegt wurden und eingebracht werden sollen, wird immer auch der Q4-Kurs berücksichtigt.    

### 6.0.170 657 (19.01.2016)

#### Magellan: 
+ Korrigiert: "Ansicht Schüler/Bewerber|Ausbildung" - Fehler bei der Suche nach Betrieben behoben.
+ Korrigiert: "Extras|Gruppen benachrichtigen": Fehler beim Versenden von E-Mails behoben.
+ Geändert: "Extras|Optionen|Registerkarte E-Mail": Bei der Anwahl des Optionsfeldes 
  "SSL/TSL-verschlüsselte Verbindung" müssen Sie jetzt zusätzlich angeben, ob diese Verschlüsselung expizit 
  oder implizit ist.
+ Geändert: "Ansicht Schüler|Daten 1" - Das Feld "Ausbildung" dient jetzt nur noch zur Anzeige des aktuellen 
  Ausbildungbetriebes. Die Einstellung des aktuellen Ausbildungsbetriebes erfolgt jetzt neu auf der 
  Registerkarte "Ansicht Schüler|Ausbildung". Angezeigt wird jetzt der Name 1 und Name 2 des Ausbildungsbetriebes.
+ Neu: "Ansicht Schüler|Daten 1" - Das Feld "Praxis" zeigt jetzt dem Feld "Ausbildung" den aktuellen
  Praxisbetrieb der Ausbildung an, der unter auf der Registerkarte "Ansicht Schüler|Ausbildung" ausgewählt
  wurde.
+ Geändert: "Ansicht Bewerber|Daten 1" - Das Feld "Ausbildung" dient jetzt nur noch zur Anzeige des aktuellen 
  Ausbildungbetriebes. Die Einstellung des aktuellen Ausbildungsbetriebes erfolgt jetzt neu auf der 
  Registerkarte "Ansicht Bewerber|Ausbildung". Angezeigt wird jetzt der Name 1 und Name 2 des Ausbildungsbetriebes.
+ Geändert: "Ansicht Schüler/Bewerber|Ausbildung" - Die Anzeige in der lsite der Ausbildungsbetriebe wurde 
  überarbeitet und jetzt übersichtlicher aufgebaut. Zusätzlich ermöglicht das Feld "Ausbildung" die Auswahl des 
  aktuellen Ausbildungsbetriebes drirekt auf der Registerkarte. 
  Zu jedem aktuell ausgewählten Ausbildungsbetrieb wird auch im Feld "Praxis" der Praxisbetrieb angezeigt 
+ Neu: "Ansicht Schüler/Bewerber|Ausbildung|Hinzufügen/Editieren": Im Dialogfenster "Ausbildung hinzufügen" bzw. 
  "Ausbildung editieren" kann jetzt über die Optionfeld "Als neue Ausbildung übernehmen" die aktuelle Eintragung
  direkt als aktuelle Ausbildung übernommen werden.
+ Neu: "Ansicht Schüler/Bewerber|Ausbildung|Hinzufügen/Editieren": Im Dialogfenster "Ausbildung hinzufügen" bzw. 
  "Ausbildung editieren" kann jetzt bei der Auswahl eine Ausbilder Kontakts bzw. Praxis Kontakts ein solcher 
  bestehender Kontkat per Doppelklick schneller ausgewählt werden.
+ Neu: "Ansicht Betriebe|Auszubildende": Neue zusätzliche Spalte "Betriebsart" gibt an, ob der zugeordnete 
  Betrieb ein Ausbldungs-, Praxis oder Praktikumsbetrieb ist.
+ Neu: "Extras|Gruppen benachrichtigen": Jetzt können Sie auch Mitteilungen an Bewerber senden.
+ Neu: Aus Schüler/Bewerber|Seriendruck an den Betrieb des Schülers können auch Praxisbetriebe angeschrieben werden.
+ Neu: Unter Betriebe|Auszubildende werden auch die Auszubildenden für den Praxisbetrieb gezeigt. 
+ Neu: Unter Betriebe|Auszubildende|Betriebsart werden die Werte Praxisbetrieb, Ausbildungsbetrieb, Praxis- und Ausbildungsbetrieb pro Auszubildenden gezeigt

#### Berichte (neu oder geändert):
+ Auslandsschulen: DAS (Zwischenzeugnis).rpt
+ BAW-BG-Abi (Ergebnisliste).rpt
+ Betriebe (Ausbilderkontakte).rpt
+ Klassenliste Schüler-Notenmatrix (mit Fehltagen).rpt
+ SAC-BS-HJI (A.01.02).rpt


### 6.0.169 657 (12.01.2016)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

#### Magellan: 
+ Korrigiert: "Ansicht Schüler", Fehler beim Seriendruck behoben.
+ Korrigiert: "Ansicht Schüler|Daten 1", Fehler bei der Anzeige des Klassenleiters
+ Korrigiert: "Ansicht Abitur|Prüfung", Fehler im Dialogfenster "Schriftliche Prüfungsnoten" behoben
+ Korrigiert: Berliner Masken: Ansicht "Schüler/Bewerber": Fehler bei Anzeige des Bezirks behoben.
+ Korrigiert: "Ansicht Schüler" - Geschwindigkeitsverbesserung beim Aufruf für:
    - das Dialogfenster für den Seriendruck
    - das Dialogfenster für das Drucken von Berichten
    - das Dialogfenster für das Drucken von Zeugnissen
+ Neu: Die Verhältnisse zwischen Schülern/Bewerbern und Sorgeberechtigten ist um die Verhältnisse "Verhältnis1" ... "Verhältnis10" 
  erweitert worden. Diese zusätzlichen Verhältnisse können unter "Verzeichnisse|Bezeichnungen anpassen" individuell in der Datenbank 
  angepasst werden. 
+ Neu: Unter "Ansicht Lehrer|Daten 2" gibt es jetzt die neuen Felder "Vertrag von", "Vertrag bis" und "Beschäftigungsart"
+ Neu: Unter "Ansicht Lehrer|Daten 3" kann man bei den Lehrämtern jetzt zusätzlich die Felder "Jahrgang von", "Jahrgang bis" und 
  "Bemerkung" eintragen.  
+ Geändert: die Berichtevorschaufenster zeigen Berichte mit der Endung *.RPT/*.rpt an    
+ Neu: Für Auslandsschulen: In den Ansichten Schüler/Bewerber/Lehrer/Sorgeberechtigte/Personen gibt es eine neue Registerkarte
  "Zusatz" mit Angaben zur Heimatadresse, Rechnungsadresse1, Rechnungsadresse2, Bankkonto1, Bankkonto2,
  Visumsverwaltung. Unter "Extras|Optionen|Ein-/Ausblenden" kann jeweils pro Ansicht eingestellt werden, ob die neue 
  Registerkarte "Zusatz" sichtbar sein soll oder nicht.  
+ Neu: Für Auslandsschulen: In den Ansichten Schüler/Bewerber/Lehrer/Sorgeberechtigte/Personen können in der Auswahlliste 
  zusätzlich die Felder "Pass gültig bis" und "Visum Ablauf am" eingeblendet werden.  
+ Neu: Für Auslandsschulen: Beim Seriendruck an Schüler/Bewerber/Lehrer/Sorgeberechtigte/Personen können zusätzlich die Felder
  der Heimatadresse verwendet werden. 
+ Neu: Unter "Verzeichnisse|Weitere Schlüsselverzeichnisse" gibt es die neuen Schlüsselverzeichnisse "Sponsoren" und "Beschäftigungsarten".    
+ Neu: Für Auslandsschulen: Unter Ansicht "Betriebe" gibt es das neue Feld "Sponsor" in der Auswahlliste und auf der Registerkarte "Daten 1".

#### MyMagellanCenter:

+ Korrigiert: Daten einsammeln: Für Tutoren werden jetzt auch in MyMagellan eingetragene Zeugnisbemerkungen der Schüler korrekt nach 
  Magellan übertragen.

#### Statistik 

+ MVP-SIP: Korrektur der Ausgabe des Knotens "SchulartId"

#### Berichte (neu oder geändert):

+ Mandant (Berufe und Fachrichtungen).rpt
+ SAC-BG-HJZ (E.01.03).rpt
