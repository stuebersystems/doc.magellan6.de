# Änderungen 2015

## 6.0.168 656 (21.12.2015)

### Magellan

Berlin => Problem in den Berliner Masken behoben

## 6.0.167 656 (18.12.2015)

### Magellan

* Verhalten der Speicherhäkchen im Schülermenü (Laufbahn, Zeugnis) korrigiert
* Berlin|Berufsbildung|Ausbildung z.Z -> auch Ausbildungen ohne Betrieb können als aktuelle Ausbildung gewählt werden

### Berichte (neu oder geändert)

+ Kursliste (Zensurerfassung nach Lehrer gruppiert).rpt
+ SAC-BG-HJZ (E.01.01).rpt
+ SAC-BG-HJZ (E.01.03).rpt
+ SAC-BG-HJZ (E.01.04).rpt
+ SAC-BG-JZ (E.01.02).rpt

## 6.0.166 656 (18.12.2015)

> DIESES UPDATE SETZT VORAUS, DASS IHRE DATENBANK UNTER FIREBIRD 2.5.2 GESICHERT UND WIEDERHERGESTELLT WURDE!

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Korrigiert: Ansicht "Bewerber", Weiterschalten zum nächsten Bewerber
+ Korrigiert: Ansicht "Adressen", Weiterschalten zur nächsten Adresse

### Berichte (neu oder geändert)

+ Kursliste (Zensurerfassung nach Lehrer gruppiert).rpt
+ SAC-BG-HJZ (E.01.03).rpt

## 6.0.165 655 (08.12.2015)

### Magellan:
+ Korrigiert: auf der Laufbahnkarte kann zwischen Allgemein und Abschluss gewechselt werden
+ Korrigiert: Schüler|Daten1 Klassenleiter und Klasse wird eingeblendet
+ Korrigiert: Berlin: Wechsel aus der Karte Grundstufe (SekI, SekII, BBS) per Doppelklick auf einen Sorgeberechtigten ins Menü Sorgeberechtigten 

### MyMagellanCenter:
+ Korrigiert: Statussymbol wird gezeigt

### Magellan-Administrator:
+ Korrigiert: Problem beim Neuanlegen eines Benutzers behoben
+ Korrigiert: Eingabe des Passworts für MyMagellan geändert

## 6.0.164 655 (07.12.2015)

### Magellan:
+ Korrigiert: Ansicht Schüler|Zeugnis beim Blättern über die Pfeiltasten werden auch die Inhalte beim Schüler (Fächer) aktualisiert
+ Korrigiert: Ansicht Schüler: Geschwindigkeitsproblem beim Wechsel zum nächsten Schüler behoben.
+ Neu: Sammelzuweisung Laufbahndaten Schüler: Das Feld Entscheidung kann neu zugewiesen  werden.
+ Korrigiert: Sammelzuweisung Details Schüler: die Anpassungen der Bezeichnungen Fehltage, davon unentschuldigt, Fehlstunden, davon unteschuldigt werden 
  jetzt auch hier korrekt angezeigt.

### Berichte (neu oder geändert):
+ Kursliste (Zensurerfassung nach Lehrer gruppiert).rpt
+ Schülerliste (Förderung).rpt

## 6.0.163 655 (02.12.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan:
+ Geändert: Ansicht "Schüler": Verbesserte Geschwindigkeit beim Aufruf der Ansicht
+ Neu: Verzeichnisse|Weitere Schlüsselverzeichnisse: Neue Schlüsselverzeichnisse "Gebiete", "Gebietsarten" und "Staaten".
  Die Werte aus "Gebietsarten" und "Staaten" können als weitere Spezifikation im Schlüsselverzeichnis "Gebiete" für die Felder "Gebietsart" und "Land" verwendet werden.
+ Neu: Ansichten "Schüler"/"Bewerber"/"Lehrer"/"Personen"/"Sorgeberechtigte": Adressangaben erweitert um die Felder "Ergänzung" (= Adressergänzung) und "Gebiet" (=Wohngebiet).
  In das Feld "Gebiet" kann der Wert getippt oder aus dem Verzeichnis ausgewählt werden. Das Verzeichnis können Sie unter Verzeichnisse|Weitere Schlüsselverzeichnisse|Gebiete erweitert.
+ Neu: Unter "Extras|Optionen|Ein-/Ausblenden" können Sie unter "Feld Gebiet bei Adressen von Schülern, Bewerbern, Lehrern, Personen und Sorgebrechtigte ausblenden" einstellen, 
  ob das neue Feld "Gebiet" bei der Adresseingabe angezeigt wird.
+ Neu: Ansichten "Lehrer"/"Personen": Bei der Namensangabe kann jetzt auch der "Namenszusatz" und der "2. Vorname" analog zu den Schülern eingegeben werden.
+ Neu: Ansichten "Sorgeberechtigte": Bei der Namensangabe kann jetzt auch der "2. Vorname" analog zu den Schülern eingegeben werden.
+ Neu: Für NRW: Ansichten "Schüler"/"Bewerber": Neues Feld "Daten 1|Geburtskreis".
+ Neu: Für Auslandsschulen: Ansichten "Lehrer"/"Personen"/"Sorgeberechtigte": Neue Felder "Staatsangehörigkeit 1", "Staatsangehörigkeit 2", "Muttersprache" und "Verkehrssprache".
+ Geändert: auf eine lokal abgelegte Magellan.UpdateInfo-Datei (standardmäßig auf unserem Server) müssen die Windows-Nutzer nur noch Leserechte haben
+ Korrigiert: Fehler bei der Übernahme von Adressänderungen von Schülern auf die Adresse der Sorgeberechtigten
+ Korrigiert: Anzeige der Mädchen und Jungen in der Statusleiste im Klassenmenü
+ Korrigiert: Problem beim Druck von Zeugnissen und gleichzeitigen PDF-Export behoben 

### Statistik:
+ SHL-ABS: Übergabe Unterrichtsart in die SA-Datei erweitert 
+ RLP-ABS: Zugänge aus Förderschulen wurden verkehrt immer als Neuzugang erkannt, jetzt wird der Schlüssel der Herkunftsart (70, 71-77) 
  und ZugangAm (zwischen dem letzten und dem aktuellen Stichtag der Statistik) geprüft
+ RLP-BBS: Lehrerabgänge werden in den LehrerNeuanlage übergeben, wenn der Lehrer inaktiv ist, ein Abgangsdatum zwischen der letzten 
  und dieser Statistik hat und einen Abgangsgrund

### Skripte:                                
+ SHL-Statistik DATEA 2015.xml (EA3700; EA2700; EA6400; EA9300; EA1900; EA9000)
+ SHL-Statistik DATSA 2015.xml (SA1700; SA1820)
+ SHL-Statistik DATLE 2015.xml (LE1210)
+ RLP-Statistik SchuelerBewegung ABS 2015.xml (STALA-36020)
+ RLP-Statistik SchuelerBewegung BBS 2015.xml (STALA-39750-1 - STALA-39750-5)
+ RLP-Statistik SchuelerNeuanlage ABS: Korrektur der Kursnr. Berechnung für GKs mind. Kursnr. 1

### Magellan-Bibliothek:
+ Korrigiert: Aktualisierung des Medienkataloges beim Wechsel zwischen Mandanten. 
  Dies führte zu einer irreführenden Fehlermeldung beim Anlegen von "MedienExemplaren". 
  Exemplare wurden aufgrund des falschen Kataloges nicht angelegt.
  
### Berichte: neu oder geändert
+ SAC-BVJ-AS ohne HS (A.01.09).rpt
+ SAC-BVJ-AS mit HS (A.01.08).rpt
+ SAC-BV-HJI (A.01.01).rpt
+ SAC-BS-JZ (nach Anlage 5).rpt
+ Klassenübersicht (Schülersumme nach Ausbildungsort).rpt
+ Quittung (Leihvertrag Taschenrechner).rpt
+ SAC-BG-AZ (E.01.05).rpt
+ SAC-BG-HJZ (E.01.04).rpt
+ SAC-BG-HJZ (E.01.03).rpt
+ SAC-BG-HJZ (E.01.01).rpt
+ Kursliste (Zensurerfassung nach Lehrer gruppiert).rpt
+ SAC-BF-HJI (B.03.01).rpt
+ MVP-GY (Studienbuch - Seite 2).rpt
+ SAC-BS-JZ (A.02.01).rpt
+ SAC-BS-JZ (A.02.01) 2spaltig.rpt
+ SAC-BS-HJZ (1 seitig).rpt
+ SAC-BS-HJI (A.01.04).rpt
+ SAC-BS-HJI (A.01.02).rpt
+ SAC-BS-Bescheinigung (F.01.01).rpt
+ SAC-BS-Bescheinigung  über erreichten Leistungen.rpt
+ SAC-BS-AZ (nach Anlage 8).rpt
+ SAC-BS-AZ (A.02.04).rpt
+ SAC-BS-AZ (A.02.04) 2spaltig.rpt
+ SAC-BS-AZ (A.02.03).rpt
+ SAC-BS-AZ (A.02.02).rpt
+ SAC-BS-AZ (2 seitig).rpt
+ SAC-BS-AS (Vorbereitungsklasse) (A.01.06).rpt
+ SAC-BS-AS (nach Anlage 6 einspaltig)2.rpt
+ SAC-BS-AS (nach Anlage 6 einspaltig).rpt
+ SAC-BG-HJZ (2010).rpt
+ SAC-BG-HJZ (2008)2.rpt
+ SAC-BG-ABI (E.01.06).rpt
+ SAC-BF-ZAS (B.04.04).rpt
+ SAC-BF-JZ (B.07.02).rpt
+ MVP-FG-ABI (2013).rpt
+ MVP-GY (Studienbuch - Seite 1).rpt
+ MVP-FO-JZ.rpt
+ MVP-FO-Fhreife.rpt
+ MVP-FO-AZ.rpt
+ MVP-FO-AZ (Variante 2 DINA4).rpt
+ MVP-FO-AZ (Variante 2 DINA3).rpt
+ MVP-FO-AS .rpt
+ MVP-FG-FHReife (Bescheinigung 2013).rpt
+ MVP-FG-AZ  (Vorstufe DINA4).rpt
+ MVP-FG-AZ  (Qualifikationsphase DINA4).rpt
+ MVP-FG-AZ.rpt
+ MVP-FG-AZ (Qualifikationsphase).rpt
+ MVP-FG-ABI.rpt
+ MVP-FG-ABI (2015).rpt
+ MVP-FG-ABI (2006).rpt
+ MVP-FG (Bescheinigung über den schulischen Teil).rpt
+ MVP-Empfangsbescheinigung.rpt
+ MVP-BVJ-HJZ.rpt
+ MVP-BVJ-AZ.rpt
+ MVP-BS-JZ.rpt
+ MVP-BS-JZ (Variante 2).rpt
+ MVP-BS-HJZ.rpt
+ MVP-BS-AZ.rpt
+ MVP-BS-AS (Variante 3).rpt
+ MVP-BS-AS (Variante 2).rpt
+ MVP-BS-AS (Variante 1).rpt
+ MVP-BS (Prüfungsakte).rpt
+ SAC-BS-AS (A.02.06).rpt
+ SAC-BS-AS (A.02.05).rpt
+ SAC-BS-AS (A.02.05) 2spaltig.rpt
+ SAC-BS-AS (A.01.07).rpt
+ SAC-BS-AS (A.01.06).rpt
+ SAC-BGJ-JZ (nach Anlage 3).rpt
+ SAC-BGJ-HJI.rpt
+ SAC-BGJ-AS ohne HS (A.01.11).rpt
+ SAC-BGJ-AS mit HS (A.01.10).rpt
+ SAC-BG-HJZ (2008).rpt
+ SAC-BG-AZ.rpt
+ SAC-BG-ABI.rpt
+ SAC-BG-ABI (E.01.09).rpt
+ SAC-BG-ABI (E.01.08).rpt
+ SAC-BG-ABI (E.01.08)(SF).rpt
+ SAC-BG-ABI (2010).rpt
+ SAC-BF-JZ (B.04.02).rpt
+ SAC-BF-JZ (B.03.02).rpt
+ SAC-BF-HJZ (nach Anlage 9).rpt
+ SAC-BF-HJZ (B.07.03).rpt
+ SAC-BF-HJZ (B.04.03).rpt
+ SAC-BF-HJZ (B.02.01).rpt
+ SAC-BF-HJI (B.05.01).rpt
+ SAC-BF-HJI (B.04.01).rpt
+ SAC-BF-HJI (B.02.01).rpt
+ SAC-BF-HJI (B.01.01).rpt
+ SAC-BF-AZ (B.03.04).rpt
+ SAC-BF-AZ (B.01.02).rpt
+ SAC-BF-AS (B.07.05).rpt
+ SAC-BF-AS (B.04.06).rpt
+ SAC-BF-AS (B.03.05).rpt
+ SAC-BF-AS (B.01.03).rpt
+ Schülerliste (Abi Statusanzeige).rpt
+ Schüler (Anzeige Schulpflichtverletzung).rpt
+ Klassenliste (Betriebe mit Auszubildenden nach Gemeinden).rpt
+ HES-AS-HJZ (Blindenschule 5-10).rpt
+ Schülerliste (Fehlzeiten nach Schüler gruppiert).rpt
+ Schülerliste (Fehlzeiten nach Klasse gruppiert).rpt
+ Schüler (Anzahl Schüler je Herkunftsschulen).rpt
+ Schulbescheinigung (mit Klasse und Ausbildungsdauer).rpt
+ Zeugnisliste nach Schülerfächern (DIN A4 nur aktive Schueler und Fachkuerzel).rpt
+ Klassenliste inkl. ausgeschulter Schüler.rpt
+ Klassenliste (welche Bewerber sind Wiederholer).rpt
+ Unfallanzeige (in Word ausfüllbar).rpt
+ Schulzeitenbescheinigung (in Word ausfüllbar).rpt
+ Schülerliste (mit Sorgeberechtigten).rpt
+ Schülerliste (mit Sorgeberechtigten französisch).rpt
+ Schülerliste (mit Sorgeberechtigten deutsch).rpt
+ Schüler (Bescheinigung-Laufbahn).rpt
+ Schulbescheinigung (SHL - in Word ausfüllbar).rpt
+ Anmeldeschein (weiterführende Schulen).rpt
+ Schülerliste (gruppiert nach Berufen mit Wohnort).rpt
+ Klassenliste (Durchnittsnoten Abitur).rpt
+ MVP-Schullastenausgleich-Vollzeit (nicht im Landkreis Mecklenburgische Seenplatte).rpt

## 6.0.162 654 (25.09.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan:
+ Neu: Unter Verzeichnisse|"Bezeichnungen anpassen" kann die folgende Feldbezeichnungen in der Ansicht 
  Schüler geändert werden: Zeugnis|Details|Versäumnisse
+ Korrigiert: in der Vorschauliste der Seriendruckdokumente im Seriendruckassistenten werden die Schattenkopien der Worddateien ausgeblendet.  
+ RLP-BBS: Erhebungsdatum in der Magellan.exe für Berufsbildende Schulen geändert
+ Neu: Die Feldlänge unter Schüler|Daten4|Fördernummer wurde auf 20 Zeichen erhöht.
+ Korrigiert: Klasse|Daten|Beeinträchtigung und sonderpäd. Förderung: die Schwerpunktfelder zeigen die eingetragenen Kürzel an
+ Neu: neues Feld "Zeugnisdatum2" unter Schüler|Zeugnis|Details

### Statistiken:
+ BRA: Landesstatistik 2015/2016 veröffentlicht
  - Aktuelle Schnittstelle
  - Neue Schlüsselverzeichnisse 
 
+ SHL: Landesstatistik 2015/2016 veröffentlicht
  - Aktuelle Schnittstelle
  - Neue Schlüsselverzeichnisse
  - Neue Skripte  

### Importe:
+ Berlin: Folgende Schlüsselimportdateien wurden erneuert/korrigiert vom Berliner Senat zur Verfügung gestellt:
  - BS_Berufsfelder.keys      (für Berufsbildende Schulen)
  - BS_Berufe.keys            (für Berufsbildende Schulen)
  - 00_Amtsbez.keys           (für Berufsbildende und Allgemeinbildende Schulen)
  Bitte importieren Sie die Dateien über den Magellan-Administrator|Datenimporte|Schlüsselverzeichnisse importieren.

### Skripte:
+ RLP-Statistik SchuelerBewegung BBS 2015 Plausibilitäten korrigiert (u.a. STALA-39730-1; STALA-37610)
+ RLP-Statistik SchuelerNeuanlage ABS 2015 Plausibilitäten korrigiert (STALA-12050;STALA-12500-2;STALA-16260-1...STALA-16260-8; STUEBER-14)
+ RLP-Statistik SchuelerNeuanlage BBS 2015 Plausibilitäten korrigiert
+ RLP-Statistik LehrerNeuanlage BBS 2015 Plausibilitäten korrigiert

+ NRW-Statistik: Fehlendes Schlüsselverzeichnis Abschlussarten (für ABI.TXT benötigt) hinzugefügt
+ NRW-Statistik: Import der NRW-Schulen um Schulnummern für Schlüssel mit Schulen anderer Bundesländer erweitert 
+ NRW-Statistik: Dokumentation verbessert: Voraussetzungen für alle Statistikdateien
+ NRW-Statistik: Dokumentation korrigiert: LSFachklasse wird aus 
  Schüler|Daten 2|Höchster Abschluss BBS|Bildungsgang ausgelesen
+ NRW-Statistik SIM.TXT: Auslesen der Ausbildung im Vorjahreszeitraum auf das gesamte Vorjahres Schuljahr erweitert
+ NRW-Statistik SIM.TXT: Auslesen der Gliederung und Fachklassen aus dem Vorjahreszeitraum korrigiert
+ NRW-Statistik SIM.TXT: Auslesen der Verkehrssprache korrigiert
+ NRW-Statistik SIM.TXT: Auslesen von zugezogen aus InDeutschlandSeit korrigiert
+ NRW-Statistik ABI.TXT: Auslesen der Abiturschüler, wenn nicht im Abiturmodul verwaltet, korrigiert

### Berichte (neu oder geändert)
+ SAR-GY-AZ (Zulassung Abitur).rpt
+ Abi (Gesamtschnitt nach Punktzahl sortiert).rpt
+ Betriebe nach Standort gruppiert.rpt
+ Betriebe nach Branchen gruppiert.rpt
+ Klassenübersicht (Schülersumme nach Ausbildungsort).rpt
+ Kursliste Namen.rpt
+ MVP-FG-AZ.rpt
+ MVP-FG-AZ (Qualifikationsphase).rpt
+ MVP-FG-FHReife (Bescheinigung 2013).rpt
+ MVP-GY (Studienbuch - Seite 2).rpt
+ MVP-GY (Studienbuch - Seite 1).rpt
+ MVP-FG-ABI (2015).rpt
+ Anmeldeschein (weiterführende Schulen).rpt
+ HES-AS-HJZ (Blindenschule 5-10).rpt
+ Klassenliste (Betriebe mit Auszubildenden nach Gemeinden).rpt
+ Klassenliste (Durchnittsnoten Abitur).rpt
+ Klassenliste (welche Bewerber sind Wiederholer).rpt
+ Klassenliste inkl. ausgeschulter Schüler.rpt
+ Klassenübersicht (Schülersumme nach Ausbildungsort).rpt
+ Kursliste (Zensurerfassung nach Lehrer gruppiert).rpt
+ MVP-BS (Prüfungsakte).rpt
+ MVP-BS-AS (Variante 1).rpt
+ MVP-BS-AS (Variante 2).rpt
+ MVP-BS-AS (Variante 3).rpt
+ MVP-BS-AZ.rpt
+ MVP-BS-HJZ.rpt
+ MVP-BS-JZ (Variante 2).rpt
+ MVP-BS-JZ.rpt
+ MVP-BVJ-AZ.rpt
+ MVP-BVJ-HJZ.rpt
+ MVP-Empfangsbescheinigung.rpt
+ MVP-FG (Bescheinigung über den schulischen Teil).rpt
+ MVP-FG-ABI (2006).rpt
+ MVP-FG-ABI (2013).rpt
+ MVP-FG-ABI (2015).rpt
+ MVP-FG-ABI.rpt
+ MVP-FG-AZ  (Qualifikationsphase DINA4).rpt
+ MVP-FG-AZ  (Vorstufe DINA4).rpt
+ MVP-FG-AZ (Qualifikationsphase).rpt
+ MVP-FG-AZ.rpt
+ MVP-FG-FHReife (Bescheinigung 2013).rpt
+ MVP-FO-AS .rpt
+ MVP-FO-AZ (Variante 2 DINA3).rpt
+ MVP-FO-AZ (Variante 2 DINA4).rpt
+ MVP-FO-AZ.rpt
+ MVP-FO-Fhreife.rpt
+ MVP-FO-JZ.rpt
+ MVP-GY (Studienbuch - Seite 1).rpt
+ MVP-GY (Studienbuch - Seite 2).rpt
+ MVP-Schullastenausgleich-Vollzeit (nicht im Landkreis Mecklenburgische Seenplatte).rpt
+ Quittung (Leihvertrag Taschenrechner).rpt
+ SAC-BF-AS (B.01.03).rpt
+ SAC-BF-AS (B.03.05).rpt
+ SAC-BF-AS (B.04.06).rpt
+ SAC-BF-AS (B.07.05).rpt
+ SAC-BF-AZ (B.01.02).rpt
+ SAC-BF-AZ (B.03.04).rpt
+ SAC-BF-HJI (B.01.01).rpt
+ SAC-BF-HJI (B.02.01).rpt
+ SAC-BF-HJI (B.03.01).rpt
+ SAC-BF-HJI (B.04.01).rpt
+ SAC-BF-HJI (B.05.01).rpt
+ SAC-BF-HJZ (B.02.01).rpt
+ SAC-BF-HJZ (B.04.03).rpt
+ SAC-BF-HJZ (B.07.03).rpt
+ SAC-BF-HJZ (nach Anlage 9).rpt
+ SAC-BF-JZ (B.03.02).rpt
+ SAC-BF-JZ (B.04.02).rpt
+ SAC-BF-JZ (B.07.02).rpt
+ SAC-BF-ZAS (B.04.04).rpt
+ SAC-BG-ABI (2010).rpt
+ SAC-BG-ABI (E.01.06).rpt
+ SAC-BG-ABI (E.01.08)(SF).rpt
+ SAC-BG-ABI (E.01.08).rpt
+ SAC-BG-ABI (E.01.09).rpt
+ SAC-BG-ABI.rpt
+ SAC-BG-AZ (E.01.05).rpt
+ SAC-BG-AZ.rpt
+ SAC-BG-HJZ (2008).rpt
+ SAC-BG-HJZ (2008)2.rpt
+ SAC-BG-HJZ (2010).rpt
+ SAC-BG-HJZ (E.01.01).rpt
+ SAC-BG-HJZ (E.01.03).rpt
+ SAC-BG-HJZ (E.01.04).rpt
+ SAC-BGJ-AS mit HS (A.01.10).rpt
+ SAC-BGJ-AS ohne HS (A.01.11).rpt
+ SAC-BGJ-HJI.rpt
+ SAC-BGJ-JZ (nach Anlage 3).rpt
+ SAC-BS-AS (2 seitig).rpt
+ SAC-BS-AS (A.01.06).rpt
+ SAC-BS-AS (A.01.07).rpt
+ SAC-BS-AS (A.02.05) 2spaltig.rpt
+ SAC-BS-AS (A.02.05).rpt
+ SAC-BS-AS (A.02.06).rpt
+ SAC-BS-AS (A.02.06).rpt
+ SAC-BS-AS (nach Anlage 6 einspaltig).rpt
+ SAC-BS-AS (nach Anlage 6 einspaltig)2.rpt
+ SAC-BS-AS (Vorbereitungsklasse) (A.01.06).rpt
+ SAC-BS-AZ (2 seitig).rpt
+ SAC-BS-AZ (A.02.02).rpt
+ SAC-BS-AZ (A.02.03).rpt
+ SAC-BS-AZ (A.02.04) 2spaltig.rpt
+ SAC-BS-AZ (A.02.04).rpt
+ SAC-BS-AZ (nach Anlage 8).rpt
+ SAC-BS-Bescheinigung  über erreichten Leistungen.rpt
+ SAC-BS-Bescheinigung (F.01.01).rpt
+ SAC-BS-HJI (A.01.02).rpt
+ SAC-BS-HJI (A.01.04).rpt
+ SAC-BS-HJZ (1 seitig).rpt
+ SAC-BS-JZ (A.02.01) 2spaltig.rpt
+ SAC-BS-JZ (A.02.01).rpt
+ Schulbescheinigung (mit Klasse und Ausbildungsdauer).rpt
+ Schulbescheinigung (SHL - in Word ausfüllbar).rpt
+ Schüler (Anzahl Schüler je Herkunftsschulen).rpt
+ Schüler (Anzeige Schulpflichtverletzung).rpt
+ Schüler (Bescheinigung-Laufbahn).rpt
+ Schülerliste (Abi Statusanzeige).rpt
+ Schülerliste (Fehlzeiten nach Klasse gruppiert).rpt
+ Schülerliste (Fehlzeiten nach Schüler gruppiert).rpt
+ Schülerliste (gruppiert nach Berufen mit Wohnort).rpt
+ Schülerliste (mit Sorgeberechtigten deutsch).rpt
+ Schülerliste (mit Sorgeberechtigten französisch).rpt
+ Schülerliste (mit Sorgeberechtigten).rpt
+ Schulzeitenbescheinigung (in Word ausfüllbar).rpt
+ Unfallanzeige (in Word ausfüllbar).rpt
+ Zeugnisliste nach Schülerfächern (DIN A4 nur aktive Schueler und Fachkuerzel).rpt

## 6.0.161 653 (27.08.2015)

### Magellan:
+ Korrigiert: Beim Export von Schlüsselverzeichnissen nach Excel/HTML werden alle Datensätze exportiert
+ Korrigiert: Automatische Adressänderung des Erziehungsberechtigten 
+ Korrigiert: Eingabe von Fehlstunden und Fehltagen Schüler|Zeugnis|Details 4-stellig möglich
+ Korrigiert: Sammelzuweisung von mehreren Zeugnisformularen möglich
+ Korrigiert: Schüler einschulen | Liste der auszuwählenden Fachtafeln gefüllt 
+ Neu: Für das Saarland - "Extras|Schüler fortschreiben"  Option "Niveau als Unterrichtsart übernehmen". Dafür müssen die Werte aus dem Schlüsselverzeichnis 
  Niveau auch im Schlüsselverzeichnis Unterrichtsart angelegt sein

### Importe:
+ Geändert: neue Schulen-Import-Datei für Berliner Schulen zum Einlesen über das Magellan-Importformat => Schulen.Import.2015.07.27.csv

### Skripte:
+ RLP-Statistik SchuelerBewegung BBS 2015 Plausibilitäten korrigiert


## Prerelease 6.0.160 653 (31.07.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan:
+ Neu: Erweiterung der Datenstrukturen für den Abgleich mit ENBREA. 

### Magellan-Administrator:
+ Korrigiert: Fehlende Felder der Tabelle "SchuelerZeitraeume" bei 
              Datenbankpflege|"Mandanten kopieren" eingepflegt.

## 6.0.159 652 (28.07.2015)

### Magellan:
+ Neu: Über Ansicht Betriebe|Bearbeiten|Organisieren|Betriebe zusammenführen kann man jetzt die Auszubildenden und Kontakte eines 
  Betriebes in einen anderen Betrieb zusammenführen und dabei optional den Ausgangbetrieb gleichzeitig löschen. Somit kann 
  das Problem der irrtümlichen mehrfachen Anlage des gleichen Betriebs einfach behoben werden.
  Bitte lesen Sie dazu den Abschnitt "Doppelt erfasste Betriebe zusammenführen" im Magellan-Benutzerhandbuch. 
+ Korrigiert: Extras|Export|SIP => alle angezeigten Meldungen werden exportiert 

### Magellan-Pool:
+ Korrigiert: Problem beim Übernehmen aus dem Schülerpool behoben

### Administrator:
+ Korrigiert: Problem beim Import von Postleitzahlen importieren|Rheinland-Pfalz|Gemeinden behoben

## Prerelease 6.0.158 652 (17.07.2015)  

### Import:

+ Geändert: für Berliner Schulen wurden die folgenden Schlüsselverzeichnisse vom Senat aktualisiert zur Verfügung gestellt:
  00_Amtsbez.keys
  00_Dienstbez.keys
  00_Herkunftsarten.keys
  00_Klassenorganisation.keys
  00_LehrerAusbildung.keys
  00_SchulartenHerkunft.keys
  00_Schularten.keys
  00_SchulformenHerkunft.keys
  00_SchulformenUebergang.keys
  00_Schulformen.keys
  00_Uebergangsarten.keys
  AS_Abgangsarten.keys
  AS_Berteuungsformen.keys
  AS_Faecher.keys
 

## 6.0.157 652 (13.07.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: unter Klassen|Klassen markieren|Drucken|Kurslisten kann auch nach einem Fachlehrerkürzel(Eintrag unter Schüler|Zeugnis|Fächer|Lehrer) gefiltert 
  werden. Alle Kurslisten wurden daran angepasst.
+ Geändert: Die Auswahlliste des Menüpunkts Berufschule kann nach Excel exportiert werden
+ Neu: Unter "Extras|Schüler fortschreiben" kann man jetzt optional die Einträge unter Fehlstunden/Fehlstunden unentschuldigt/
  Fehltage/Fehltage unentschuldigt/Fehltage im Praktikum/Fehltage im Praktikum unentschuldigt mit fortschreiben
+ Neu: Nur für SAR - Unter "Extras|Schüler versetzen" können Sie die neue Optionen "Niveau als Unterrichtsart übernehmen" markieren. 
  Mit dieser Optionen werden die für das nächste Schuljahr voreingestellten Werte unter "Niveau" in der neuen Klasse unter "Unterrichtsart"
  eingetragen.
+ Neu: Unter "Extras|Schüler versetzen" bzw. "Extras|Schüler wechseln" können Sie mit der neuen Optionen 
  "Noten mit Endnote fortschreiben übernehmen" analog wir beim Fortschreiben die Endnote dieser Fächer mit übernehmen.
+ Neu: Unter "Ansicht Klassen|Drucken|Kurslisten drucken" wurde im Dialogfenster "Kursliste drucken" zusätzlich das Filter "Lehrer" eingefügt. 
+ Neu: Unter "Ansicht Schüler|Zeugnisse|Leistungen" bzw. "Ansicht Schüler|Zeugnisse|Leistungen|Notenübersicht" kann man jetzt zusätzlich die Notenfelder
  "Zusatz Note 4"..."Zusatz Note 9" und die weiteren Felder "Vergessene Hausaufgaben" und "Vergessene Arbeitsmittel" einblenden.
+ Neu: Unter "Ansicht Schüler|Zeugnisse|Leistungen" bzw. "Ansicht Schüler|Zeugnisse|Leistungen|Notenübersicht" kann man jetzt zusätzlich eine schriftliche
  Beurteilung pro Fach erfassen. Sie können dabei einen freien Text eintragen oder vordefinierte Beurteilungstexte mit einfügen. Diese Funktion ist 
  verfügbar für Schüler aus Klassen, deren Beurteilungsart auf "Noten" gesetzt wurde.
+ Geändert: Unter "Ansicht Mandant|Daten" kann man das Feld "Straße" jetzt mit max. 100 Zeichen eintragen.

### Schnittstellen

+ Korrigiert: NRW-Statistik 2015; Auslesen und Ausgabe Foerderschwerp1 und Foerderschwerp2 
              aus den neuen Feldern "FoerderSchwerp1" und "FoerderSchwerp2" in Klassen und Schüler
              Dokumentation entsprechend angepasst.

### Skripte

 + BER-APO-KO-2011: Berechnung der Gesamtpunktzahl für die Fachhochschulreife korrigiert.
 
### Berichte (neu oder geändert)

+ Alle Ausleihvorgaenge pro Schueler (nach Klassen gruppiert).rpt
+ Alle Ausleihvorgaenge pro Schueler (nach Klassen und Medien gruppiert).rpt
+ BAW-GY-ABI (2014 - Abschrift RP).rpt
+ BAW-GY-ABI (2014 - Abschrift SuS).rpt
+ BAW-GY-ABI (2014 - Kontrolle vor mündlichen Abi - 2 Seite).rpt
+ BAW-GY-ABI (2014).rpt
+ BER Abi-1a – Übersichtsplan über die Schullaufbahn ab 2010 – 12jähriger Bildungsgang (VO-GO) (01.12).rpt
+ BER-GY-JZ (Schul Z 250)(05.08).rpt
+ Etiketten (No.3475 - 70 x 36 mm - 1fach - 8 x 3).rpt
+ Klassenliste Schüler-Notenmatrix (Querformat-Durchschnitt).rpt
+ Kursliste (Schüler-Kursart-Klasse-Lehrer).rpt
+ Kursliste (Zensurerfassung nach Lehrer gruppiert).rpt
+ Kursliste (Zensurerfassung).rpt
+ Kursliste Namen (mit Foto und Behinderung).rpt
+ Kursliste Namen und Endnote.rpt
+ Kursliste Namen.rpt
+ MVP-FG-ABI (2013).rpt
+ NRW-GY-HJZ (Klasse 5-8).rpt
+ RLP-BG (Punktekreditkarte-2010).rpt
+ RLP-BG-ABI (2010).rpt
+ RLP-BG-ABI (2010)A4.rpt
+ SAC-BS-Bescheinigung (F.01.01).rpt
+ SAC-BVJ-AS mit HS (A.01.08).rpt
+ SAR-GEMS-AZ (Klasse 5-8)(Vollschulzeitpflicht nicht erfüllt).rpt
+ SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
+ Schüler-BBS (Bescheinigung-Laufbahn).rpt
+ SHL-GY-ABI (2011).rpt
+ Unfallanzeige.rpt
+ Zeugnisliste nach Schülerfächern (Kopfnoten).rpt

### Datenstruktur
+ Neu: Feld "Lehrer" in Tabelle/Ansicht "AuswahlKurslisten"
+ Neu: Felder "Note9", "Note10", "Note11", "Note12", "Note13", "Note14",
       "HausaufgabenVergessen","ArbeitsmittelVergessen" in Tabelle 
       "SchuelerFachdaten"   

## Prerelease 6.0.156 651 (25.06.2015)   

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan:
+ Geändert: Unter Schüler|Zeugnis|Zeugnisformulare können per Sammelzuweisung auch mehrere Formulare in einem Arbeitsgang an die ausgewählten Schüler verteilt werden.
+ Neu: Magellan kann die Pfade zu den Dateien Magellan.evm (enthält die Pfadangaben zur Datenbank und den Datenordnern), Magellan.lic (enthält die Lizenzdaten) Magellan.opt 
  (auch die Optionsdateien für Magellan Bibliothek und Magellan Haushalt&Inventar)aus einer Paths-Datei auslesen. Diese Datei kann auf eigene Verzeichnisse verweisen und wird 
  beim Programmstart ausgelesen. Bitte lesen Sie dazu den Abschnitt "22.2 Die Paths-Datei" im "Magellan6.pdf" oder den entsprechenden Abschnitt im "Magellan6SetupInfo.de.pdf".
  
### Bibliothek:
+ Korrigiert: Drucken der Quittung bei Kurssatzausleihe

### Skripte:

Geändert: in den Skripten "Synchronisiere Zugriffsrechte" und "Benutzerrechte zuweisen" wurden die Tabellen Wettkaempfe und WettkampfDisziplinen für Benutzergruppen ergänzt.

### Schnittstellen:
+ Korrigiert: (MVP-SIP) Ausgabe des Geburtsortes für den Schüler 
+ Korrigiert: (MVP-SIP) Ausgabe des AbschlussDatums für schulische berufliche Vorbildung

### Datenstruktur:
+ Gelöscht: Einige doppelte Indizes wurden entfernt
+ Korrektur: Fremdschlüssel "FK_LEHRERLEHRAEMTER_LEHRAMT" in Tabelle "tblLehrerLehraemter"


## 6.0.155 650 (12.06.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan:
+ Geändert: im Seriendruckassistenten werden für die Auswahl Vorlagen außer dot- und dotx-Dateien auch doc- und docx-Dateien gezeigt
+ Korrigiert: die Auswahl eines neuen Berufes unter Schüler|Ausbildung per Maus und Return wird korrekt gespeichert
+ Korrigiert: Sportfeste|Schüler Synchronisieren|Wettkampfdisziplinen: beim Synchronisieren von Schülern werden die dem Wettkampf zugeordneten Disziplinen zugewiesen
+ Korrigiert: Berliner Masken|Auswahlliste|Spalte Klassen: die möglichen Filterwerte wurden korrigiert
+ Korrigiert: Zeichenlänge des Feldes Vorname2 im Schnelleingabeformular beim Anlegen eines neuen Schülers/Bewerbers wurde auf die mögliche Zeichenlänge des Feldes Vorname2 erweitert
+ Neu: unter Abitur|Prüfung gibt es den neuen Assistenten "schriftliche Prüfungsnoten". Damit können Sie fachweise direkt in der Spalte Endnoten (bereits erfasste Noten werden in der Spalte eingeblendet) die schriftliche Note eingeben oder jeder Prüfer trägt seine Note in der Spalte Prüfer1 oder Prüfer2 ein. Sind beide Prüfernoten gleich, wird die Spalte Endnote gefüllt. Beim Schließen des Assistenten werden die Endnoten für den Schüler mit als schriftliche Prüfungsnote übernommen. 

### Magellan-Administrator:
+ Korrigiert: Beim Einlesen des Schlüsselverzeichnisses Faecher 
+ Korrigiert: Der Punkt Datenbankpflege|"Mandanten kopieren" wurde an die aktuelle Datenstruktur angepasst

### Magellan-Bibliothek:
+ Korrigiert: Problem beim Neuanlegen von Medien behoben

### Skripte: 
+ Korrigiert: RLP-APO-BGY-2010.dws 
    - Geändert wurde, dass 4 Kurse eines über Fächer|Aufgabenbereich als gesellschaftswissenschaftlich gekennzeichneten Fachs als Vorschlag markiert werden. Zusätzlich werden für Wirtschaftsgymnasien noch jeweils ein Kurs folgender Fächer (erkannt über die Kategorie der Fächer im Verzeichnis) erwartet:
      - Gemeinschaftskunde, also Kategorie Geschichte, Sozialkunde oder Erdkunde
      - BWLRW
      - VWL
    - Diese Änderung ist nur für Schulen relevant, deren Schüler die Fachwahl bereits vor dem Erscheinen der Verordnungsänderungen (Juli 2014) abgeschlossen hatten. Für alle anderen Schüler verwenden Sie bitte das Skript "RLP-APO-BGY-2010.dws".
+ Korrigiert: SAC-APO-BGY-2014.dws 
    - Neu aufgrund der Veränderungen beim Runden gemäß §§39, 44 und 50a sowie der Anlage 2. Im Skript SAC-APO-BGY-2011.dws wird bei unrunden Ergebnissen der Bruchteil abgeschnitten, mit dem Skript SAC-APO-BGY-2014.dws wird nun mathematisch gerundet.
+ Korrigiert: SHL-APO-2010.dws 
    - Berechnung für  Sport als 3PF (schriftliche und praktische Prüfung)
+ Korrigiert: SAR-APO-BGY-2007.dws 
    - Erkennen des Fachs Gesundheit als 1PF für Berufliche Gymnasien der Fachrichtung Gesundheit und Soziales
    - Berechnen der Durchschnittsnote
+ Korrigiert: SAR-APO-DFG-2014.dws
  
### Schnittstellen:
+ Neu: RLP-Statistik 2015 veröffentlicht; Schlüsselverzeichnisse aktualisiert
o Neu: (MVP-SIP) Ausgabe des Geburtsortes für den Schüler hinzugefügt 
o Korrigiert: (MVP-SIP) Berechnung des Schüler-Status in alten Zeiträumen korrigiert   

### Datenstruktur:
+ Neu: Feld "PruefungSchriftlich1Pruefer1" in Tabelle "SchuelerABI"
+ Neu: Feld "PruefungSchriftlich1Pruefer2" in Tabelle "SchuelerABI"
+ Neu: Feld "PruefungSchriftlich2Pruefer1" in Tabelle "SchuelerABI"
+ Neu: Feld "PruefungSchriftlich2Pruefer2" in Tabelle "SchuelerABI"
+ Neu: Feld "PruefungSchriftlich3Pruefer1" in Tabelle "SchuelerABI"
+ Neu: Feld "PruefungSchriftlich3Pruefer2" in Tabelle "SchuelerABI"
+ Neu: Feld "PruefungSchriftlich4Pruefer1" in Tabelle "SchuelerABI"
+ Neu: Feld "PruefungSchriftlich4Pruefer2" in Tabelle "SchuelerABI"
+ Neu: Ansicht "ABIPruefungsfaecherSchriftlich" für die Eingabe schriftlicher 
       Prüfungsnoten im Abiturmodul
o Korrektur: Fremdschlüssel "FK_SCHUELER_ABSCHLUSSBBSBERUF" in Tabelle "Schüler"
  Ermöglicht das verändern des Berufekürzels, wenn dieser als Höchster Abschluss 
  BBS Beruf eingetragen ist.      

### Berichte (neu oder geändert):  
+ BAW-BG (Schülerzeugnisblatt).rpt
+ BAW-BG-ABI (DIN A4 doppelseitig 2015 - Abschrift).rpt
+ BAW-BG-ABI (DIN A4 doppelseitig 2015).rpt
+ BAW-BG-Abi (Ergebnisliste).rpt
+ BAW-BG-Abi (Stammkarte).rpt
+ BAW-BG-GY (Mitteilung Prüfungsergebnisse).rpt
+ BER-GS-JZ (Schul Z 103)(11.05) (französ. Gymn).rpt
+ BER-GY-JZ (Schul Z 250)(05.08).rpt
+ RLP-GY-AZ (2006).rpt
+ SAC-BG-ABI (E.01.06).rpt    
  - Beachten Sie die neue Anmerkung A0661:
  - Die Fachrichtung des Schülers legen Sie wie folgt an:
     1)	Weisen Sie im Menü „Schüler“ auf der Registerkarte „Ausbildung“ den Bildungsgang des Schülers im Feld „Bildungsgang“ zu. Grundlage bildet das Schlüsselverzeichnis „Verzeichnisse|Bildungsgänge“. 
     2)	Weisen Sie unter „Verzeichnisse|Bildungsgänge“ die Fachrichtung im Feld „Fachrichtung“ zu. Grundlage bildet das Schlüsselverzeichnis „Verzeichnisse|Weitere Schlüsselverzeichnisse|Fachrichtungen“.
     Ausgegeben auf dem Zeugnis wird die Fachrichtung des Bildungsganges.
+ Zeugnisliste nach Schülerfächern (DIN A4 mit UA und Niveau).rpt
+ Zeugnisliste nach Schülerfächern (DIN A4).rpt

## 6.0.154 649 (22.05.2015)

### Magellan:
+ Korrigiert: Problem beim Aufrufen des Druckfensters korrigiert unter Zeugnisformulare und Berufsschulmatrix

### Magellan-Administrator:
+ Neu: Magellan-Import schueler.import.csv importiert jetzt auch das Feld "NichtDeutscheHerkunft" J/N 

### Skripte:
+ geändert: BAW-APO-BGY-2010-G9.dws -> Neue Rundung bei der Berechnung des Gesamtergebnisses der Englischnote berücksichtigt 

### Berichte (neu oder geändert):  
+ SAR-FHReife (Nachweis).rpt
+ BAW-GY (Stammkarte).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ Abi (Ergebnisliste).rpt
+ Schülerliste (Abitur).rpt
+ BAW-BG-ABI (DIN A4 doppelseitig 2015 - Abschrift).rpt
+ Unfallanzeige.rpt


## 6.0.153 649 (18.05.2015)

### Magellan-Administrator:
+ Korrigiert: Fehler beim Synchronisieren der Benutzerrechte bzw. beim Zuweisen der Benutzerrechte 
  behoben


## 6.0.152 649 (13.05.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan:
+ Neu: Unter "Ansicht Adressen|Daten|Unfallanzeige" kann markiert werden, ob die Adresse als möglicher Empfänger für 
       Unfallanzeigen Verwendung finden kann inkl. der Angabe der zugehörigen Trägernummer.
+ Neu: Unter "Ansicht Schüler|Bearbeiten|Unfallanzeigen" können jetzt Unfallanzeigen erfasst, gespeichert und 
       ausgedruckt werden. Bitte beachten Sie hierzu den Abschnitt "Unfallanzeigen erstellen und verwalten" im 
       Magellan-Handbuch.
+ Neu: Drucken von Crystal Reports Berichten. Erfolgt nach Auswahl des Berichts und Start des Drucks ein Abbruch durch 
       den Benutzer, bleibt ab sofort das Fenster zur Auswahl der Berichte geöffnet. 
+ Neu: Unter "Ansicht Schüler" wird auf den Registerkarten "Daten 1" .. "Zeugnis" in der Kopfzeile ausgewiesen, ob der 
       Schüler volljährig ist.
+ Neu: Feld Sorgeberechtigte | Daten | Geburtsland hinzugefügt.
+ Neu: Feld "Farbe" im Verzeichnis "Verkehrsmittel" hnzugefügt.
+ Neu: Funktion Sorgeberechtigte | Löschen mit neuer Option zum Löschen von Sorgeberechtigten, die noch Schüler verweisen. 
+ Geändert: Felder "Ausgestellt am" und "Bemerkung" des Schülerausweises sind vom Register "Extras" 
            auf das Register "Daten 4" in der Ansicht Schüler übertragen worden.
+ Geändert: bei der inkrementellen Suche in Auswahllisten oder Assistenten erreichen Sie den nächsten passenden 
            Datensatz mit STRG+Pfeiltaste auf- oder abwärts (siehe Handbuch unter dem Stichwort "inkrementelle Suche") 
+ Korrigiert: Synchronisiere Zugriffsrechte.dws (Schreibfehler bei Qualifikationsniveaus)
+ Korrigiert: Anzeige von dotx-Seriendruckvorlagen im Netzwerk


### Schnittstellen:
+ Neu: (MVP-SIP) Ausgabe des Knotens "Angabe" beim Schüler. Damit werden die Daten des 
       Ausbildungsbetriebes mit ausgespielt.
+ Korrigiert: (MVP-SIP) Auslesen der Fachrichtungen und Bildungsgänge
+ Korrigiert: (MVP-SIP) 
    * "Schüler | Daten 2 | Höchster Abschluss BBS | Beruf | Erreicht am" zur Anzeige und Eingabe hinzugefügt.
    * "Schüler | Daten 2 | Höchster Abschluss BBS | ..." Anzeige von Werten, die zuvor mal auf BBS kategorisiert waren, 
      aber im Schlüsselverzeichnis auf ABS umgestellt wurden und zuvor nicht im Feld geändert wurden.
    * Ausgabe Statistikfeld "BetriebPlz" korrigiert.            

### Magellan-Administrator:
+ Neu: Im Anschluss an das Löschen der Datenbankinhalte unter "Datenbankpflege|Datenbankinhalt löschen" werden 
  automatisch die ID-Generatoren synchronisiert

### Importe:
+ Geändert: (BER) Neue Schlüssel AS-Faecher.keys => bitte kontrollieren Sie, ob unter 
            Verzeichnisse|Fächer die Zeile für Kunst in der Spalte Schlüssel den Wert 131 hat,
            ggfs. ändern Sie den Wert bitte von Hand(KU;131;Bildende Kunst/Kunst)
+ Geändert: (SAC) neue Schlüsselverzeichnisse
+ Geändert: Im Postleitzahlimport für Deutschland sind die Berliner Vorwahlen angepasst worden (030)


### Datenstruktur:
+ Neu: Tabelle "SchuelerUnfallberichte"
+ Neu: Tabelle "SchuelerFoerderschwerpunkte"
+ Neu: Felder "Volljaehrig", "Unfallbericht" in Tabelle/Ansicht "AuswahlSchueler"
+ Neu: Feld "Volljaehrig" in Tabelle/Ansicht "AuswahlZeugnisse"
+ Neu: Felder "EmpfaengerUnfallbericht", "EmpfaengerUnfallberichtNr" in Tabelle "Adressen"
+ Neue Felder "Foerderschwerpunkt1", "Foerderschwerpunkt2" in Tabellen "Klassen" und "Schueler"
+ Neue Felder "Barcode", "BarcodePrint" in Tabellen/Ansichten "Schueler", "Lehrer", "Personen"
+ Neu: Feld "Farbe" in Tabelle "Verkehrsmittel"
 
### Berichte:
+ Neu: Crystal Reports Druck - Die Tabellen/Ansichten "AuswahlSchueler" und "AuswahlZeugnisse" 
       enthalten das neue Feld "Volljaehrig", welches angibt, ob der Schüler volljährig ist.
       
### Berichte (neu oder geändert):
+ Unfallanzeige (mit Erläuterungen).rpt
+ Unfallanzeige.rpt
+ BER-GY-JZ (Schul Z 251)(07.10).rpt
+ SAC-Fremdsprachenzertifikat (F.01.05)(DIN A3).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-GY-ABI (2010-G8-G9)A4.rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 2).rpt



## 6.0.151 648 (02.04.2015)

### Magellan:
+ Neu: Unter "Extras|Notfall senden" gibt es über das Optionfeld "Nicht an Sorgeberechtigte senden" die 
  Möglichkeit, die Sorgeberechtigten der Schüler des aktuellen Zeitraums mit einzubeziehen.
+ Neu: Unter "Extras|SMS Protokoll" werden jetzt auch SMS aufgelistet, die über "Extras|Notfall senden" versendet werden.

### Skripte:
+ Geändert: (BER-APO-2011.dws): Beleg- und Einbringverpflichtung im 2. Aufgabenfeld
+ Geändert: (NRW-APO-BK-2012 ): Vorschlagsautomatik

### Importe:
+ Geändert: (BER) neue Schulen-Import-Datei für Berliner Schulen zum Einlesen über das Magellan-Importformat => Schulen.Import.2015.02.26.csv
+ Geändert: (BER) neue Schlüssel AS-Faecher.keys und BS_Faecher.keys


### Berichte (neu oder geändert):
+ Mandant (Prüfbericht Schüler unter 18 ausgeschult und keinen Eintrag unter ZugangAbgang An Schule).rpt
+ Kursliste (Zensurerfassung).rpt
+ Klassenliste (welche Bewerber sind Wiederholer).rpt
+ Zeugnisliste nach Schülerfächern (Kopfnoten).rpt
+ Klassenliste (Fehltage und Fehlstunden).rpt
+ RLP-GY-ABI (2010-G8-G9)A4.rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 2).rpt



## 6.0.150 648 (12.03.2015)

+ Korrektur: Aufruf des Bewerbermenüs  


 
## 6.0.149 648 (12.03.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Neu: Unter "Verzeichnisse|Noten" kann in der neuen Spalte "Hintergrundfarbe" eine Hintergrundfarbe angeben.
+ Neu: Unter "Extras|Optionen|Einstellungen" kann man einstellen, ob die Hintergrundfarben aus dem Verzeichnis "Noten" 
  in der Ansicht "Schüler|Zeugnis|Leistungen" und "Schüler|Zeugnis|Leistungen|Notenübersicht" verwendet werden sollen.
+ Korrektur:(MVP-SIP-Schnittstelle|Ausgabe) für die Ausgabe der Fremdsprache, des Fremdsprachenstatus und des Fremdsprachenzusatz 
+ Korrektur:(MVP-SIP-Schnittstelle|Prüfung) Wenn ein Bildungsgang eingetragen wurde, muss auch eine Fachrichtung erfasst sein
+ Korrektur:(MVP-SIP-Schnittstelle|Prüfung) wenn eine schulische Vorbildung erfasst wurde(ABS, BBBS oder Beruf), muss auch das Abschlussdatum erfasst sein
+ Korrektur:(MVP-SIP-Schnittstelle|Ausgabe) wenn das Lehramt nicht in Magellan erfasst wurde, wird kein Eintrag in der Datei erzeugt
+ Korrektur: Seriendruckfelder Briefanrede und Briefempfänger für die Übergabe an Word (Bewerber|Brief an Sorgeberechtigte des Schülers) ergänzt
+ Korrektur: (Berlin Abiturdatenschnittstelle 2015): Jahrgang aktualisiert, Meldung wenn keine statistisch relevanten Daten vorliegen angepasst

### Magellan-Biblíothek:
+ Korrektur:  Datum "Ausleihe bis" wird beim Ausführen einer Aktion automatisch gesetzt, wenn es zuvor im Editfeld geleert wurde

### Importe:
+ Geändert: neue Schulen-Import-Datei für Berliner Schulen zum Einlesen über das Magellan-Importformat => Schulen.Import.2015.02.26.csv
 
### Skripte:
+ Korrigiert: (RLP-APO-2014): Vorschlag für Fremdsprachen optimiert
+ Korrigiert: (RLP-APO-2014): Ersatzfach für Sport; bitte kennzeichnen Sie das Ersatzfach im Fachstatus mit "Ersatz"
+ Neu: (RLP-APO-BGY-2014): § 12(1) abgeändert:  ...bei einem nicht ganzzahligen Gesamtergebnis wird ab der Dezimalen 5 aufgerundet.

### Berichte(neu oder geändert):
+ Bewerber gruppiert nach Gesamtnote.rpt
+ Bewerber nach Herkunftsschulen und Klassen.rpt
+ Schülerliste (Anwesenheit Ags).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-GY-HJZ (11-13).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 2).rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 1).rpt
+ RLP-GY-ABI (2010-G8-G9)A4.rpt
+ RLP-FS-AS (Sozialpädagogik DIN A3).rpt
+ Abi (Ergebnisliste).rpt


## 6.0.148 647 (18.02.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Neu: Unter "Ansicht Abitur|Qualifikation" gibt es jetzt die neue Spalte "Niveau" für das Fachniveau.
+ Neu: Unter "Ansicht Mandanten|Daten 1" gibt es das neu Feld "Prüfungsnummer". [Tabelle Mandanten|PruefungsNr]
+ Neu: Für Berlin wird die Abiturschnittstelle 2015 mit dieser Ausgabe freigegeben. Bitte beachten Sie 
  dazu das aktualisierte Dokument Magellan6Berlin.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan6Berlin.pdf
+ Neu: Unter Verzeichnisse|Zeiträume|Art wird die Art nachgetragen, für Halbjahre, in denen die Angabe fehlt   

### Skripte:
+ Korrigiert (MVP-APO-2010.dws): Block I Prüfung Mindestanzahl der Fächer mit weniger als 5 Punkten
+ Geändert (SAR-APO-DFG-2014.dws): große Notenverzeichnisse können verarbeitet werden
+ Geändert: Synchronisiere ABI.dws : übertragt das Niveau in den Abiturbereich
+ Korrigiert: Synchronisiere Zugriffsrechte.dws 

### Berichte(neu oder geändert):
+ BAW-BG-ABI (DIN A4 doppelseitig 2015).rpt
+ Schülerliste (Anwesenheit Ags).rpt
+ SAC-BS-HJI (A.01.04).rpt
+ Alle Ausleihvorgaenge pro Schueler (nach Klassen gruppiert).rpt
+ Alle Ausleihvorgaenge pro Schueler (nach Klassen und Medien gruppiert).rpt
+ Medienvorgaenge (Standard).rpt


## 6.0.147 646 (28.01.2015)

### Magellan
+ Korrektur: Problem beim Synchronisieren der Zugriffsrechte (Qualifikationsniveau) gelöst
+ Korrektur: Problem beim Anzeigen unter Abitur|Prüfung gelöst (11PF/BLL)
+ Korrektur: Anzeigeproblem unter Schüler|Zeugnis|Details behoben
+ Neu: Berlin - In den Berliner Masken kann das neue Feld "Gültig bis" für den Schülerausweis über 
  "Ansicht Schüler|Bearbeiten|Sammelzuweisung..." mehreren Schülern zugewiesen werden.
+ Neu: Ansicht Schüler/Bewerber|Bearbeiten|Export|Schüler Berlin exportieren: Es wird jetzt auch das neue Feld für den 
  Jahrgang des Schülers exportiert. Bitte beachten Sie dazu das aktualisierte Dokument Magellan6Berlin.pdf auf unserer 
  Webseite:  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan6Berlin.pdf  
+ Neu: Ansicht Schüler|Zugang/Abgang: Durch Markieren des Optionsfeldes "Als neue Herkunftsschule übernehmen" wird die
  neue eingetragene Schule zur neuen Herkunftsschule des Schülers.

### Berichte (neu oder geändert):
+ MVP-Schullastenausgleich-Teilzeit (nicht im Landkreis Mecklenburgische Seenplatte).rpt
+ MVP-Schullastenausgleich-Vollzeit (nicht im Landkreis Mecklenburgische Seenplatte).rpt
+ SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
+ BAW-GY (Stammkarte).rpt
+ SAR-GY-AZ (Klassenstufen 5-10).rpt
+ SAR-GY-Verhaltenszeugnis.rpt
+ SAR-GY-AZ (modifiziert Klassenstufen 9 und 10).rpt
+ SAR-GY-HJZ-JZ (Klassenstufen 5-10).rpt


## 6.0.146 646 (19.01.2015)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].
         
> Bitte beachten Sie auch die geänderten Punkte des vorangegangenen Prerelease 6.0.145!

### Magellan
+ Geändert: Beim automatischen Erzeugen von Crystal Reports Berichten als PDF in der Dokumentenverwaltung werden
  jetzt Berichte mit Filterfuntionen korrekt verbeitet. Erzeugt der erstellte Bericht z.B. für den Schüler nur 
  eine leere Seite, so dazu keine PDF-Datei mehr für diesen Schüler in der Dokumentenverwaltung abgelegt. 
+ Neu: "Ansicht Schüler|Auswahlliste": Neues Feld "Volljährig", die Ausgabe des Wertes erfolgt automatisch.
+ Neu: "Ansicht Schüler|Daten 4": Neues Feld "Gültig bis" für den Schülerausweis. 
  Dieses Feld kann über "Ansicht Schüler|Bearbeiten|Sammelzuweisung..." mehreren Schülern zugewiesen werden.  
+ Neu: "Ansicht Schüler|Zeugnis|Details": Neues Feld "Jahrgang" für den Jahrgang des Schülers zur Berücksichtigung von 
  jahrgangsgemischten Klassen. Die Sammelzuweisung auf der Registerkarte wurde ebenfalls um den Wert "Jahrgang" erweitert
+ Neu: "Ansicht Schüler|Auswahlliste": Neues Feld "Jahrgang" für den Jahrgang des Schülers
+ Neu: Berlin - In der Maske "Grundstufe" wird hinter dem Wert "Jg/Saph/Jül" nun der Wert "Jahrgang Schüler" editierbar 
angzeigt. Er entspricht dem Wert unter "Ansicht Schüler|Zeugnis|Details|Jahrgang".
+ Neu: Berlin - In der Maske "Grundstufe" kann bei der Sammelzuweisung zusätzlich das Feld "Jahrgang Schüler" zugewiesen 
werden.
+ Neu: "Extras|Schüler fortschreiben" bzw. "Extras|Schüler versetzen": Optional kann der Jahrgang des Schülers im Rahmen d
       es Fortschreibens bzw. Versetzens erhöht werden. 
+ Neu: "Ansicht Schüler|Bearbeiten|Schüler als Bewerber kopieren": Beim Kopieren werden jetzt auch die bisherigen 
      besuchten Schulen mit übernommen. Zusätzliche wird nach Möglichkeit der aktuelle Mandant als zuletzt
       besuchte Schule eingetragen inkl. der bei der Schule hinterlegten Schulform. Dies ist nur möglich, wenn es zur 
       Schulnummer des Mandanten eine entsprechende Schule mit gleiche Schulnummer in der Ansicht "Schulen" gibt.
  Zusätzlich werden folgende Angaben für die Herkunftsschule mit übernommen:
  - die letzte Klasse
  - die letzte Klassenstufe
  - der Klassenleiter  
  - die Schulform
  - der Jahrgang
+ Neu: Magellan berücksichtigt jetzt den Deutschen Qualifikationsrahmen. Dazu gibt es ein neues Schlüsselverzeichnis
  "Qualifikationsniveaus". In diesem können die Qualifikationsniveaus erfasst werden.  
+ Neu: "Verzeichnisse|Bildungsgänge": Neues Feld "DQR-Stufe" zur Erfassung der Stufe des Qualifikationsniveaus gemäß
  dem Deutschen Qualifikationsrahmen.
+ Neu: "Verzeichnisse|Berufe": Neues Feld "DQR-Stufe" zur Erfassung der Stufe des Qualifikationsniveaus gemäß
  dem Deutschen Qualifikationsrahmen. 
+ Neu: "Ansicht Lehrer|Auswahlliste": Neues Feld "Dienstbez."

### Skripte:
+ Neu: Saarland - Magellan berücksichtigt beim Import des Lehrer-Unterrichts in der Oberstufe (z.B. aus DAVINCI) über 
  das Schuldatentransferformat neben den Unterrichtsarten "Kurs", "GK", "LK" jetzt auch die Unterrichstarten "E" und "G" 
  für E-Kurse und G-Kurse.

### Berichte (neu oder geändert):
+ SAR-GY-AZ (Klassenstufen 5-10).rpt
+ SAR-GY-Verhaltenszeugnis.rpt
+ SAR-GY-AZ (modifiziert Klassenstufen 9 und 10).rpt
+ SAR-GY-HJZ-JZ (Klassenstufen 5-10).rpt
+ BAW-GY (Mitteilung Prüfungsergebnisse).rpt
+ Sorgeberechtigte ohne Kinder im aktuellen Zeitraum.rpt
+ Abi (Ergebnisliste).rpt
+ Schulbescheinigung (mit Klasse und vorauss. Ende einfach).rpt
+ Zeugnisliste nach Schülerfächern (DIN A4 nur aktive Schueler und Fächerkürzel).rpt
+ Schulbescheinigung (Anmeldung weiterführende Schule).rpt
