# Änderungen 2018

## LEGENDE

Abkürzung | Bedeutung     
----------|----------
FIX       | Korrektur bestehender Funktionalität              
NEW       | Neue Funktionalität                              
CHANGE    | Änderung des Ablaufs, Verarbeitung oder Bedienung



> #### primary::Aktuelle Hinweise
>
> * SERIENDRUCK: Einige Kunden erhielten beim Aufruf des Seriendruck eine Fehlermeldung "Makrospeicher konnte nicht geöffnet werden". Diese Meldung resultiert aus Sicherheitseinstellungen in Word. Bitte lesen Sie dazu diesen [Artikel](https://doc.magellan6-kb.stueber.de/seriendruck/makrospeicher.html).
> * RUNTIME-ERROR: Einige Benutzer, die von älteren Versionen umsteigen, können MAGELLAN im Anschluss nicht starten. Meist ist die Ursache, dass eine der Dateien, die beim Programmstart geladen werden, beschädigt ist. 
>   Sie finden hier eine [Anleitung](https://doc.magellan6.stueber.de/installation/probleme-beim-update.html#meldung-runtime-error-) um dieses Problem zu beheben.

---


## 6.5.30 - 671 (21.12.2018)

### MAGELLAN

* FIX: Korrektur bei BBS-Prüfungsnote Kontrolle, Rechte und Ansicht
* FIX: Saarland: Ergänzung für den Assistenten unter `Extras > Statistik > Saarland`


### Importe

* FIX: SAC-BS_Bildungsgaenge.keys: In der Spalte `Bezeichnungen` wurden die vorangestellten Schlüsselnummern entfernt.


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: DE-DIAP-2015.dws: Fehler bei Summierung im Bereich 4 behoben
* FIX: NRW-APO-2012.dws Fehler bei der Einbringung der Defizitkurse behoben
* CHANGE: NRW-APO-BK-1999.dws - Ausgabe verbessert
* FIX: NRW-AS-APO.BK-1999.dws - Korrektur 


### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE: Betrifft alle Berichte: Die Berichtsdateien wurden vorbereitet, um für einen ggfs. parallelen Einsatz von Version 7 verwendbar zu sein, alte Berichte wurden dabei teilweise in Archivverzeichnisse verschoben.
* CHANGE: DAS-GY-ABI \(Anlage7\).rpt / Layoutanpassungen, Ausgabe des Jahrganges bei den Fremdsprachen ergänzt
* CHANGE: Schüler (Anzahl Schüler je Herkunftsschulen).rpt 
* CHANGE: Klassenliste (inklusive Zusatzklasse).rpt
* CHANGE: Unfallanzeige.rpt
* NEW: DAS-Übersicht über Prüfungsfächer Abitur \(Anlage 6\).rpt
* NEW: Schülerliste mit Integrationsstatus.rpt | Diese Liste gibt nur Schüler mit Integrationsstatus gruppiert nach Klassen aus.
* CHANGE: BER-Schul Z 510 (12.13).rpt | Ausgabe Fachbezeichnung **Sport/Gesundheitsförderung** korrigiert
* CHANGE: DAS-ZZ (Q-Phase)(Anlage 1)(RiLi 1.6).rpt | Punktwerte werden mit dem Zusatz "Punkte" ausgegeben

## 6.5.29 - 671 (27.09.2018)

### MAGELLAN

* NEW: Für die Lizenzausbaustufe MAGELLAN ABITUR (Deutsche Auslandsschulen, die MAGELLAN nur für die Abiturberechnung, nicht für die Verwaltung einsetzen) wurde die Anzahl der pro Halbjahr anlegbaren Klassen auf 9 Klassen erhöht.  
* FIX: NRW SIM.TXT Regel ST-031-1 an Position 7 erwartet
* FIX: NRW SIM.TXT Herkunftsschule/Schulform korrigiert
* FIX: NRW SIM.TXT Schüler nicht als versetzte Schüler gekennzeichnet
* FIX NRW SIM.TXT korrekte Ausgabe der Jahrgänge
* FIX NRW SIM.TXT korrekte Ausgabe der Jahrgänge bei Wiederholern
* FIX: Link zu Firebird 2.5.8 ist jetzt korrekt im Fenster zur Datenstrukturanpassung
* FIX: SHL-Statistik DATSA 2018 Skriptfehler REGEL SA9501

## 6.5.28 - 671 (14.09.2018)

### MAGELLAN

* CHANGE: Min. Voraussetzung Firebird 2.5.8
* NEW: SHL: Veröffentlichung der Statistik 2018
* FIX: Betriebe zusammenführen
* FIX: SAR: Abfrage der Lizenz für die Statistik Saarland
* FIX: Statistik NRW SIM.TXT

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE: Zeugnisliste \(Schuljahr\).rpt / Layoutanpassungen

## 6.5.27 - 671 (28.08.2018)

### MAGELLAN

* FIX: RLP-BBS-Bewegung: In die Bewegungsdatei werden nur noch Schüler übernommen, für die unter `Schüler > Laufbahn > Abschluss > Abschluss1` eine Eintragung vorgenommen wurde. Damit werden BVJ-Schüler, die nach dem ersten Jahr in eine Klasse mit anderem Bildungsgang (8101050/8101060 ) wechseln nicht mehr für die Bewegungsdatei ausgegeben.


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: RLP-Statistik LehrerNeuanlage BBS 2018.xml
  * STALA-5600 
  * STALA-5160


## 6.5.26 - 671 (16.08.2018)

### MAGELLAN

* FIX: Beim Export von Schülerdaten in die Einlesedatei für SchülerOnline wird auch bei gewechselten Schülern die korrekte Klasse übergeben.


### Importe

* FIX: Die Dateien "00\_Postleitzahlen.keys" und "00\_Gemeinden.keys" wurden für die Region RLP überarbeitet. 
  Bitte lesen Sie die Dateien vor der Statistikerstellung ein, eine Anleitung dazu finden Sie in der Dokumentation für die Landesstatistik im Abschnitt [Postleitzahlverzeichnisse aktualisieren](https://doc.ls.stueber.de/schluesselverzeichnisse.html#postleitzahlverzeichnisse-aktualisieren). ** Bitte beachten Sie die Abschnitte  "Postleitzahlverzeichnis importieren", "Gemeinden synchronisieren" und "Vollständigkeit der Gemeindekennziffern für Schüler überprüfen"!**


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: "RLP-Statistik LehrerNeuanlage BBS 2018.xml":

  * STUEBER-15
  * STUEBER-16
  * STUEBER-17
  * STUEBER-18
  * STUEBER-19
  * STUEBER-20-1
  * STUEBER-20-2
  * MORGEN-170
  * STALA-5550
  * MORGEN-60
  * STUEBER-6

* FIX: DE-DIAP-2015.dws \(Vorschlag überarbeitet: genau 36 Kurse, mindestens 14 Kurse aus Naturwissenschaft und Fremdsprachen, nur die 3 besten Sportkurse\)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE: DAS-GY-ABI \(Anlage 7\).rpt (4.Kurshalbjahr der Prüfungsfächer wird ausgegeben [Bereich I.], nicht erbrachte Prüfungen werden ausgestrichen [Bereich II.], Designänderungen[Bereich II. und V.])

## 6.5.25 - 671

### MAGELLAN

* FIX: Beim Anlegen eines Schülers werden die Felder `Zusatz` und `2.Vorname` leer gespeichert, wenn keine Auswahl getroffen wurde. Damit werden Sie in der Filterung der Auswahlliste ggfs. auch als leer erkannt.
* NEW: Nordrhein-Westfalen: Statistikmodul 2018. Beachten Sie bitte die aktualisierten [Schlüsselverzeichnisse](https://doc.ls.stueber.de/schluesselverzeichnisse.html). Die aktualisierte [Statistikdokumentation](https://doc.ls.stueber.de/nordrhein-westfalen/abs+bbs.html)
  für NRW finden Sie hier.
* NEW: Für die Lizenzausbaustufe MAGELLAN ABITUR (Deutsche Auslandsschulen, die MAGELLAN nur für die Abiturberechnung, nicht für die Verwaltung einsetzen) wurde die Anzahl der pro Halbjahr anlegbaren Klassen auf 6 Klassen erhöht.  

  ### MYMAGELLAN CENTER

* NEW: Beim Erstellen der MYMAGELLAN-Dateien wird ein Hinweis ausgegeben, wenn beim Erstellen der Dateien keine Auswahl für das Feld `Fehlstunden/Fehltage` getroffen wird.

![Bitte treffen Sie eine Auswahl!](/images/liesmich/6.5.25.01.png)

### Importe

* FIX: in der Datei "00_Postleitzahlen.keys" (unter `Import > Deutschland > PLZ`) wurde für alle Vorwahlen eine Führungsnull ergänzt. Bitte lesen Sie ggfs. die Datei neu ein, die Möglichkeit finden Sie im MAGELLAN Administrator.

![Postleitzahlen neu importieren](/images/liesmich/6.5.25.00.png)


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: BAW-APO-BGY-2010-G9.dws | Korrektur in der Durchschnittsnotenberechnung

### Berichte (neu oder geändert)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: Unfallanzeige.rpt (zwei Sorgeberechtigte werden angezeigt, Hergangsfeld vergrößert)
* FIX: RLP-GY-JZ (2018).rpt (Noten der LKs werden nicht mehr vertauscht ausgegeben)
* FIX: SHL-GY-AZ (A3)(2015).rpt (Beurteilung der Fächer wie Attest oder ohne Bewertung wird nun auf dem Zeugnis ausgegeben)
* FIX: BER-Schul Z 251b (05.16).rpt (Schülernamen werden nun in den Bericht richtig übergeben)
* NEW: DAS-Versetzungszeugnis-GY-MSA (ZKA)(Anlage 11)(§23).rpt (Versetzungszeugnis Gymnasium - Mittlerer Schulabschluss (ZKA))
* NEW: Fachwahl-Kursliste.rpt (Die Liste kann nach Kursen gruppiert Schüler eines Kurshalbjahres aus dem Bereich `Abitur > Fachwahl` ausgeben)
* FIX: SAC-FOS-AZ (D.01.03).rpt (Schülernamen werden wieder ausgegeben)
* FIX: SAC-FOS-FHReife (D.01.04).rpt (Berechnung Durchschnittsnote korrigiert)
* FIX: BAW-BG-ABI (DIN A4 doppelseitig 2018 - Abschrift).rpt | Layoutanpassungen
* BAW-BG-ABI (DIN A4 doppelseitig 2018 - Neuausstellung).rpt | Layoutanpassungen
* BAW-BG-ABI (DIN A4 doppelseitig 2018).rpt | Layoutanpassungen
* BAW-BG-Abi (Stammkarte 2018)| Layoutanpassungen


## 6.5.24 - 671

### MAGELLAN

* NEW: Rheinland-Pfalz Statistikmodul 2018. Beachten Sie bitte die aktualisierten [Schlüsselverzeichnisse](https://doc.ls.stueber.de/schluesselverzeichnisse.html). Die aktualisierte [Statistikdokumentation](https://doc.ls.stueber.de/rheinland-pfalz/abs+bbs.html)
  für RLP finden Sie hier.
* FIX: Unter `Schüler > Familie` wird die Telefonpriorität für Mobilnummern farblich unterlegt
* FIX: Unter `Schüler > Verzeichnisse > Fachtafeln > Fachwahltafeln` können Fächer nach Klick auf die Schaltfläche `Bearbeiten` editiert werden
* FIX: Beim Einschulassistenten wird im Feld `Fachtafel` die Liste der Fachtafeln gefüllt.
* FIX: Problem beim Speichern von Layoutinformationen \(nur Berliner Masken\) unter `Schüler > Fächer` und `Schüler > Leistungen` behoben


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: für das Fachwahlskript BER-FW-APO-2011.js wird die Fachkategorie Psychologie für das zweite Aufgabenfeld berücksichtigt
* FIX: NRW-APO-2012.dws \(Korrektur der Vorschlagsautomatik\)
* FIX: NRW-APO-2012.dws \(Korrektur der Vorschlagsautomatik\)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: BER-GY \(abi\_4\_berechnungsbogen\)\(10.16\).rpt
* FIX: DAS-GS-GY \(Klasse 3-10\).rpt \| \(Ausgabe Schulart, abgefragt wird die Schulart des Schülers oder die Schulart der Klasse\)
* FIX: DAS-JZ \(5-12\).rpt \| \(Ausgabe Schulart, abgefragt wird die Schulart des Schülers oder die Schulart der Klasse\)
* NEW: RLP-GY-JZ \(2018\).rpt \| \(aktualisiert, Grundlage dieses Berichtes ist RLP-GY-JZ \(2006\).rpt 
* NEW: SAR-GEMS-AS \(Klasse 9-10\) Ansicht Mittelstufe.rpt \(Abschlusszeugnis für die Ausgabe aus der Ansicht "Mittelstufe"\)


## 6.5.22 - 671 (06.06.2018)

### MAGELLAN

* FIX: Der Sammelzuweisungsassistent und das dazugehörige Skript unter `Berufsschule > Zeugnis > Sammelzuweisung` wurden korrigiert.

### Importe

* FIX: [Sachsen] Die Importkataloge "BS_Bildungsgaenge.keys" und "00_Faecher.keys" wurde korrigiert

### MAGELLAN ADMINISTRATOR

* FIX: Importassistent

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)


* FIX: BER-APO-2017.dws \(berücksichtigt nun auch die Note des Prüfungsgespräches der PRS bzw. BLL\)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: BER-GY \(abi\_4\_berechnungsbogen\)\(10.16\).rpt
* FIX: DAS-GS-GY (Klasse 3-10).rpt | (Ausgabe Schulart, abgefragt wird die Schulart des Schülers oder die Schulart der Klasse)
* FIX: DAS-JZ (5-12).rpt | (Ausgabe Schulart, abgefragt wird die Schulart des Schülers oder die Schulart der Klasse)


## 6.5.21 - 671 (28.05.2018)


> #### warning::Wichtig!
>
> Die Datenstruktur von MAGELLAN ist erweitert worden!   
> Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von MAGELLAN erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](http://doc.magellan6.stueber.de/installation/serviceupdates.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](http://doc.magellan6.stueber.de/installation/troubleshootingupdate.html).

### MAGELLAN

* FIX: MAGELLAN passt sich an die Windows-Skalierung an
* NEW: Anpassung der Statistikschnittstelle Abiturdaten für Berlin


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* CHANGE: SAR-APO-BGY-2017.dws Korrektur fehlender Parameter beim Speichern für Summenberechnung der Prüfung	
* CHANGE: RLP-APO-G8-2017|[[Vorabdownload](https://my.hidrive.com/lnk/cjyJCm2N)|[Anleitung](https://doc.la.stueber.de/Skripte/rlp-apo-2014-g8.html)]: Korrektur des Vorschlags, vierter Kurs wurde von jedem Fach markiert.
* NEW: SAR-VO-GEM-2015.dws: Ist auch für Berechnung des Jahrgangs 10 im Menü `Mittelstufe` erweitert worden, bitte beachten Sie auch die Dokumentation im Abschnitt [Mittelstufe](https://doc.la.stueber.de/mittelstufe.html) und für das Berechnungsskript [SAR-VO-GEM-2015](https://doc.la.stueber.de/mittelstufe/berechnungsskripte/sar-vo-gem-2015dws.html).

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

#### Berlin

* FIX: BER-Schul Z 303 (05.16).rpt (Zeugnisdatum)

#### Deutsche Auslandsschulen

* NEW: DAS-HS-MSA-AS (Anlage 8 und 9)(§23).rpt | Zeugnis-Hauptschulabschluss (Anlage 8)(§23) und Zeugnis Realschule Mittlerer Schulabschluss (Anlage 9)(§23)
* NEW: DAS-Zeugnis Gymnasium - Mittlerer Schulabschluss (Anlage 10)(§23).rpt | Zeugnis Gymnasium - Mittlerer Schulabschluss (Prüfung)(Anlage 10)(§23)
* FIX: DAS-JZ (5-12).rpt

#### Sachsen

* NEW: SAC-BG-ABI (E.01.06)(ab 2017).rpt | Zeugnis der allgemeinen Hochschulreife
* NEW: SAC-FOS-HJZ (D.01.01).rpt | Halbjahreszeugnis der Fachoberschule
* NEW: SAC-FOS-JZ (D.01.02).rpt | Jahreszeugnis der Fachoberschule
* NEW: SAC-FOS-AZ (D.01.03).rpt | Abgangszeugnis der Fachoberschule
* NEW: SAC-FOS-FHReife (D.01.04).rpt | Zeugnis der Fachhochschulreife
* FIX: SAC-BG-HJZ (E.01.03).rpt | Halbjahreszeugnis des Beruflichen Gymnasiums, Jahrgangsstufe <12/13>

#### Saarland

* FIX: SAR-GEMS-AZ (Klasse 5-10).rpt


## 6.5.20 - 670 (07.05.2018)

> #### warning::Wichtig!
>
> Die Datenstruktur von MAGELLAN ist erweitert worden!   
> Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von MAGELLAN erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](http://doc.magellan6.stueber.de/installation/serviceupdates.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](http://doc.magellan6.stueber.de/installation/troubleshootingupdate.html).

### MAGELLAN


* CHANGE: Erweiterung der Tabelle SchuelerBBS
* CHANGE: `Extras > in Mandanten versetzen > Lehrer versetzen` kann mit den Rechtegruppen Schulleitung1, Schulleitung2, Sekretariat1 und Sekretariatsrechten ausgeführt werden.
* CHANGE: Beim Versetzen von Schülern in einen anderen Mandanten, werden die übernommenen Sorgeberechtigten nur neu im zweiten Mandanten angelegt, wenn sie noch dort noch nicht existieren. Überprüft wird dabei die GUID der Sorgeberechtigten.

### Importe

* NEW: Sachsen: neue Schlüsselverzeichnisse, bitte lesen Sie die Schlüsselverzeichnisse entsprechend der [Anleitung](https://doc.magellan6.stueber.de/admin/import-export.html#schlüsselverzeichnisse-importieren) ein. 

Hinweise für die SAXSVS-Exportschnittstelle finden Sie in der Dokumentation [MAGELLAN Landesstatistiken](https://doc.ls.stueber.de/) im Abschnitt [Sachsen BBS](https://doc.ls.stueber.de/sachsen/sachsen.html).

| Verzeichnisname | Anmerkung |
| --- | --- |
| BS\_Organisationen.keys | relevant für SAXSVS |
| BS\_Schulformen.keys | relevant für SAXSVS |
| BS\_SopaedFoerderungen.keys | relevant für SAXSVS |
| 00\_Fachstati.keys | - |
| 00\_Faecher.keys | - |
| 00\_FoerderSchwerpunkte.keys | relevant für SAXSVS |
| 00\_Klassenstufen.keys | - |
| 00\_Konfessionen.keys | - |
| 00\_Noten.keys | - |
| 00\_SchuelerMerkmale.keys | relevant für SAXSVS |
| 00\_Sprachreferenzen.keys | - |
| 00\_Staatsangehoerigkeiten.keys | relevant für SAXSVS |
| 00\_Unterrichtsarten.keys | - |
| AS\_Schulformen.keys | - |
| BS\_Bildungsgaenge.keys | relevant für SAXSVS |



### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* NEW:MVP-APO-FG-2017, bitte beachten Sie die [Beschreibung](https://doc.la.stueber.de/mvp-apo-fg-2017.html).

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* NEW: BER-GY (abi_4_berechnungsbogen)(10.16).rpt
* FIX: DAS-GS-GY \(Klasse 3-10\).rpt




## 6.5.19 - 669 (17.04.2018)


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* Fix: [SAC-APO-BGY-2017](https://doc.la.stueber.de/skripte_SAC-APO-BGY-2017.html): Problem bei der Fremdspracheneinbringung gelöst, Kennzeichnung der neu beginnenden Fremdsprache geändert, siehe [Anleitung "Merkmale"](https://doc.la.stueber.de/skripte_SAC-APO-BGY-2017.html).
* FIX: [BER-APO-FOS-2013.dws](https://doc.la.stueber.de/skripte_ber-apo-fos-2013.html)
* FIX: [SAR-APO-2017.dws](https://doc.la.stueber.de/Skripte/SAR-APO-2017.html): Problem bei Initialisieren von Fächern gelöst \(Prüfungsfächer mit den Kategorien Politik, Sozialkunde, Erdkunde, Philosophie oder Geschichte\)\)
* FIX: [NRW-APO-BK-2017.dws](https://doc.la.stueber.de/skripte_nrw-apo-bk-2012.html): Korrektur bei der Markierung für das Fach Sport.
* FIX: [NRW-APO-2012.dws](https://doc.la.stueber.de/skripte_nrw-apo-2012.html) Problem bei Philosophie und maximaler Anzahl von Defizitkursen bei Grundkursen gelöst. Berechnung der optimalen Punktzahl angepasst.
* FIX: allgemeine Optimierungen:
  * BAW-APO-1999.dws
  * BAW-APO-BGY-2002.dws
  * BER-APO-2004.dws
  * BER-APO-2007.dws
  * BER-APO-2010.dws
  * BER-APO-2011.dws
  * BER-APO-2017.dws
  * BER-BBS-Matrix-2007.dws
  * BER-APO-KO-1987.dws
  * BER-APO-KO-2011.dws
  * BER-APO-KO-2017.dws
  * BRE-APO-1998.dws
  * BRE-APO-2006.dws
  * BRE-APO-2010.dws
  * BRE-APO-AGY-2006.dws
  * BRE-APO-BGY-1998.dws
  * BRE-APO-BGY-2005.dws
  * BRE-APO-BGY-2010.dws
  * BRE-APO-KO-2006.dws
  * BRE-APO-KO-2010.dws
  * DE-DIAP-2005.dws
  * DE-DIAP-2015.dws
  * DE-DRP-2005.dws
  * HES-APO-2015.dws
  * HES-APO-BGY-2015.dws
  * MVP-APO-1999.dws
  * MVP-APO-2006.dws
  * MVP-APO-2010.dws
  * MVP-APO-FG-1999.dws
  * MVP-APO-FG-2014.dws
  * NIE-APO-2005.dws
  * NIE-APO-2007.dws
  * NIE-APO-FG-1997.dws
  * NIE-APO-FG-2007.dws
  * NIE-APO-G8-2010.dws
  * NIE-APO-G8-2014.dws
  * NIE-APO-G8-2016.dws
  * NIE-APO-G9-2010.dws
  * NIE-APO-G9-2014.dws
  * NIE-APO-G9-2016.dws
  * NRW-APO-1998.dws
  * NRW-APO-2012.dws
  * NRW-APO-BK-1999.dws
  * NRW-APO-BK-2011.dws
  * NRW-APO-BK-2012.dws
  * RLP-APO-1999.dws
  * RLP-APO-2006.dws
  * RLP-APO-2010.dws
  * RLP-APO-2014.dws
  * RLP-APO-BGY-1999.dws
  * RLP-APO-BGY-2010.dws
  * RLP-APO-BGY-2014.dws
  * RLP-APO-G8-2014.dws
  * RLP-APO-WG-1999.dws
  * SAA-APO-1999.dws
  * SAC-APO-1996.dws
  * SAC-APO-BGY-2004.dws
  * SAC-APO-BGY-2010.dws
  * SAC-APO-BGY-2011.dws
  * SAC-APO-BGY-2014.dws
  * SAC-APO-BGY-2017.dws
  * SAR-APO-1999.dws
  * SAR-APO-BGY-1999.dws
  * SAR-VO-GEM-2015.dws
  * SHL-APO-1998.dws
  * SHL-APO-2007.dws
  * SHL-APO-2010.dws
  * SHL-APO-2015.dws
  * THÜ-APO-1999.dws

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: DAS-GY-ABI (Anlage 7).rpt \ (auf Seite 3 erfolgt nun die richtige Ausgabe "V. Sprachen" und nicht mehr "V. Fremdsprachen")
* FIX: BER-Abi 8 \(01.12\).rpt \(Anzeige des Fachs "Bildende Kunst"\)
* NEW: BER-Schul Z 510 \(12.13\).rpt
* NEW: NRW-BKO-ABI \(Bescheinigung Schullaufbahn\)\_Zeugnisbemerkung\_Fachdaten.rpt: Dieser Bericht gibt die Zeugnisbemerkungen aus dem Bereich `Schüler > Zeugnis > Zeugnis > Zeugnisbemerkungen` für das beim Druck gewählte Halbjahr aus. Die Anleitung wurde im Modul MAGELLAN Berichte ergänzt.





## 6.5.18 - 669 (09.03.2018)

### MAGELLAN

* CHANGE: NRW: Schlüsselverzeichnis "00\_Muttersprachen.keys" aktualisiert
* FIX: Bewerbersammelzuweisung korrigiert
* FIX: Löschen von Fachtafel-Fächer-Zeilen in Fachwahltafeln korrigiert
* FIX: Eingabe negativer Positionen für Zeugnisbemerkungen möglich (hierfür wurde auch [MyMagellan](ftp://ftp.stueber.de/pub/bin/de/magellan/v6/mymagellan6.msi) korrigiert)
* CHANGE: Schüler > Zeugnis > Zeugnis > Sammelzuweisung `Zeugnisbemerkung`: inkremetelle Suche beim Kürzel möglich
* FIX: Schüler > Zeugnis > Details > Sammelzuweisung `Tutor`: Beim Setzen des Häkchens für den Tutor ohne Auswahl eines Tutors kann der bereits zugewiesene Tutor für die ausgewählten Schüler gelöscht werden
* FIX: Löschen von Sorgeberechtigten korrigiert (Resteinträge in SchuelerSorgebe werden mit entfernt)

### MAGELLAN Center

* FIX: Daten verteilen: Liste der Zeiträume und die Liste der Klassen wurden für Windows 10 nicht vollständig gezeigt

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: [SAR-APO-DFG-2014](https://doc.la.stueber.de/skripte_sar-apo-dfg-2014.html): angepasst für aktuelle MAGELLAN Version
* FIX: [RLP-APO-2014](https://doc.la.stueber.de/skripte_rlp-apo-2014.html): Wenn Sport LK ist, aber der praktische Teil nicht erbracht werden konnte, sondern nur der Sporttheorieteil, dann wird die Summe einfach gewichtet. Voraussetzung: Unter `Abitur > Qualifikation` wird für die Sportzeile des betroffenen Schülers im Feld `Merkmal`der  Wert `ST` erfasst. 
* FIX: [RLP-APO-2014](https://doc.la.stueber.de/skripte_rlp-apo-2014.html): Berechnung der optimalen Punktzahl in Sonderfällen verbessert. 
* FIX: [BER-APO-2011.dws](https://doc.la.stueber.de/skripte_ber-apo-2011.html) + [BER-APO-2017.dws](https://doc.la.stueber.de/Skripte/BER-APO-2017.html)
  * Berechnung Gesamtpunktzahl FHR korrigiert
  * Philosophie wird korrekt berücksichtigt
* FIX: Synchronisiere Abi: Beim Synchronisieren von Schülerdaten in die Ansicht `Abitur > Qualifikation` mit der Option `Fächer mit unterschiedlichen Unterrichtsarten getrennt synchronisieren` werden Fächer mit der Unterrichtsart FA korrekt übernommen

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: Bewerberliste mit Summendaten.rpt \(Sortierung korrigiert\)
* FIX: BER-BF-AS \(einjährig\).rpt


## 6.5.17 - 669 (14.02.2018)

> #### warning::Wichtig!
>

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](http://doc.magellan6.stueber.de/installation/serviceupdates.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](http://doc.magellan6.stueber.de/installation/troubleshootingupdate.html).



### MAGELLAN

* FIX: Korrektur beim Versetzen von Schülern mit Sorgeberechtigten in einen anderen Mandanten.
* FIX: Unter `Abitur > Prüfung  > schriftliche Prüfungsnoten...` wurde die Speicherung des Layouts und der Note korrigiert.

### MAGELLAN Center

* UPDATE: Beim Importieren der MyMAGELLAN-Dateien wurde die Logik der Leistungsbeurteilungen (`Schüler > Zeugnis > Leistungen > Beurteilung`) und der Fehlzeiten wie nachstehend geändert. 
Bitte beachten Sie auch den aktualisierten Abschnitt ["Importlogik"](https://doc.magellan6.stueber.de/admin/mymagellan-center.html#importlogik).

**Leistungsbeurteilung **

Stand in MAGELLAN/MYMAGELLAN |Was passiert beim Import?
---|---
Beurteilung ist in MAGELLAN /keine Beurteilung in MyMAGELLAN| Beurteilung in MAGELLAN bleibt bestehen
Beurteilung ist nicht in MAGELLAN, Beurteilung ist in MyMAGELLAN| Beurteilung aus der MyMAGELLAN-Datei wird eingelesen
Beurteilung sind in beiden Programmen|Beurteilung aus MyMAGELLAN wird eingelesen

**Fehlzeiten**

Option|Ergebnis
-|-
Fehlstunden/-tage in MAGELLAN beim Einsammeln überschreiben|Der Eintrag aus der MYMAGELLAN überschreibt den Eintrag in MAGELLAN. <br/> **Ausnahme: Es wird nichts oder eine NULL erfasst, in diesem Fall bleibt der MAGELLAN-Eintrag erhalten.**
Fehlstunden/-tage in MAGELLAN beim Einsammeln addieren|Fehlstunden/-tage aus allen MYMAGELLAN-Dateien werden aufaddiert. <br/>Bitte beachten Sie, dass das erneute Einlesen einer Datei bei dieser Option auch erneut die Werte addiert.
Fehlstunden/-tage in MAGELLAN beim Einsammeln nicht aktualisieren|Es erfolgt keine Änderung in MAGELLAN.



### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: NRW-APO-BK-2012.dws: Korrektur der Vorschlagsautomatik 


### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: 
* NEW: BER-Schul Z 255 \(09.17\).rpt \(_Abgangszeugnis des Gymnasiums, Jahrgangsstufen 5 bis 9 \(09.17\)_\)
* NEW: BER-Schul Z 240 \(09.17\).rpt \(_Zeugnis des Gymnasiums, Jahrgangsstufen 5 bis 9 - \(09.17\)_\)
* CHANGE: SAC-BG-HJZ (E.01.01).rpt  _(Halbjahreszeugnis des Beruflichen Gymnasiums, Klassenstufe 11)_
* CHANGE: SAC-BG-JZ (E.01.02).rpt  _(Jahreszeugnis des Beruflichen Gymnasiums, Klassenstufe 11))_
* CHANGE: SAC-BG-HJZ (E.01.03).rpt _(Halbjahreszeugnis des Beruflichen Gymnasiums, Jahrgangsstufe <12/13>)_
* CHANGE: SAC-BG-HJZ (E.01.04).rpt _(Halbjahreszeugnis des Beruflichen Gymnasiums Jahrgangsstufe <12/13>)_
* CHANGE: Ausländerliste (nur Minderjährige).rpt



## 6.5.16 - 668 \(25.01.2018\)

### MAGELLAN

* FIX: Ansicht `Schüler > Zeugnis > Details`: Fehltage, Fehltage unentschuldigt, Fehlstunden, Fehlstunden unentschuldigt werden korrekt gespeichert.


### MAGELLAN Administrator

* FIX: Die Sicherung einer Datenbank und Wiederherstellung einer Sicherung wurden korrigiert.
* FIX: Das Problem beim Löschen eines Benutzers im Menüpunkt `Benutzerverwaltung` wurde gelöst.
* CHANGE: Beim Ändern eines Benutzerpasswortes unter `MAGELLAN > Datenbank > Kennwort ändern..` werden die Eingaben mit Sternchen verdeckt.
* NEU: Unter `Datenbankpflege > Datenbank überprüfen > `gibt es eine neue Reinigungsfunktion, um überzählige Fachzeilen aus der Ansicht `Abitur > Qualifikation` zu entfernen.

![Löscht pro Abschlussjahrgang überzählige Fachzeilen, verglichen werden Fach und Unterrichtsart, erhalten bleibt ggfs. eine Zeile mit gefüllten Fachstatus.](/images/liesmich/6.5.16.00.png)

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: Synchronisiere ABI.dws:Beim Synchronisieren ins Menü Abitur gab es eine Meldung, wenn zusätzlich unter Extras > Optionen > Einstellungen der Haken "Automatischer Abgleich Qualifikation/Fachwahl" aktiviert war. Sie können den Haken deaktiveren oder das mit dieser Ausgabe veröffentlichte Skript verwenden.
* FIX: Synchronisiere ABI.dws: Die Option "Fächer mit unterschiedlichen Unterrichtsarten getrennt synchronisieren" wurde korrigiert. 
![Option "Fächer mit unterschiedlichen Unterrichtsarten getrennt synchronisieren"](/images/liesmich/6.5.16.01.png)



### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: Schülerpersonalblatt incl. Schuleintritt und -austritt \(mit Vorbildung\).rpt
* CHANGE:  Bescheinigung zur Rentenversicherung \(V0510 - 26.06.2017\).rpt \(Gemäß offizieller Vorlage vom 26.06.2017\)







