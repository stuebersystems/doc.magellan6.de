# Änderungen 2014 (und früher)

## 6.0.145 645 (30.12.2014) Prerelease

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Unter Extras|Optionen|Einstellungen kann man einstellen, ob man bei den Zeiträumen mit Halbjahren oder 
  Trimestern arbeiten möchte. Eine Kombination von Halbjahren und Trimestern ist nicht möglich. Wenn Sie bereits mit 
  Halbjahren arbeiten und Trimester nutzen möchten, wenden Sie sich bitte an unser Supportteam unter 
  http://support.stueber.de
+ Geändert: Modul Live-Message: Fehler beim Versenden von Benachrichtungen per E-Mail behoben.
+ Geändert: Modul Live-Message: Anpassung beim Versenden von SMS-Benachrichtigungen.
+ Geändert: Optionen: Darstellung der Passwortangaben für E-Mail und SMS geändert.

Haushalt&Inventar
+ Korrigiert: Problem beim Anlegen von Buchungen behoben.

Skripte:
+ Neu: (RLP-APO-2014.dws): Dieses Skript bildet folgende Regel mit ab:
       ....§12 (1) ….. 2. soweit in einem Fach schriftlich und mündlich geprüft wurde, werden die Punkte der 
       schriftlichen Prüfung mit zwei Drittel, die der mündlichen Prüfung mit einem Drittel multipliziert; die 
       Ergebnisse werden addiert und zur Ermittlung des Gesamtergebnisses in Block II bei vier Prüfungsfächern mit 
       fünf, bei fünf Prüfungsfächern mit vier multipliziert; bei einem nicht ganzzahligen Gesamtergebnis wird ab der 
       Dezimalen 5 aufgerundet.
+ Neu: (SAR-APO-DFG-2014.dws): Abiturskript für das Deutsch-Französische Gymnasium Saarbrücken.
  Bitte beachten Sie dazu das aktualisierte Dokument Landesanpassungen.pdf.

## 6.0.144 644 (09.12.2014)

***Datenstrukturerweiterung***
--------------------------
WICHTIG: Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! 
Die Datenstruktur von Magellan 6 ist erweitert worden. Beim ersten Start von Magellan erfolgt eine 
automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Sie müssen dazu wie folgt vorgehen:  
      1. Melden Sie sich als sysdba in Magellan an. Alle anderen Benutzer müssen Magellan verlassen haben!        
      2. Der Assistent zur Konvertierung erscheint. Führen Sie die Konvertierung aus. Schließen Sie danach Magellan. 
      3. Rufen Sie den Magellan-Administrator auf. Synchronisieren Sie die Zugriffsrechte der Benutzer 
         (Datenbankpflege > Datenbank prüfen, Option: Zugriffsrechte synchronisieren).
         
Firebird: Magellan ist für die Einsatz unter Firebird 2.5.2 optimiert, gehen Sie wie folgt vor:
      1. Stellen Sie sicher, dass die Benutzer von Magellan abgemeldet sind.
      2. Bitte laden Sie sich diese Version aus dem Downloadbereich unter www.stueber.de.
      3. Stoppen Firebird 2.5.1 auf Ihrem Server in der Systemsteuerung|Klassische Ansicht|Firebird Server Manager.
      4. Installieren die neuere Version per Doppelklick und folgen den Anweisungen.
      5. Im Anschluss starten Sie Firebird bitte wieder.
      6. Erstellen Sie über den Magellan-Administrator eine Sicherung Ihrer Datenbank
      7. Stellen Sie diese Sicherung bitte wieder her.
      8. Stoppen Sie Firebird, tauschen die Datenbank gegen die wiederhergestellte Datenbank aus und starten Firebird wieder.
### Magellan
+ Neu: Unter Extras|Optionen|Einstellungen gibt es die "Art des Zusammenführens von Schülern". Ist ein Schüler in der 
  Datenbank bereits angelegt und wird als Bewerber kopiert, können beim späteren Einschulen der Kopie beide Datensätze 
  wieder zusammengeführt werden. Sie entscheiden mit dieser Option, ob die aktualisierten Daten der Bewerberkopie
  übernommen werden sollen oder die Schülerdaten des Stammschülers bestehen bleiben sollen.
+ Geändert: Kopie vom Schüler (mit interner ID) und Vagabunden (Schüler ohne Klassenzuordnung) können in einem Durchgang eingeschult werden
+ Geändert: Kopie vom Schüler (mit interner ID) und Schüler können im gleichen Zeitraum beim Einschulen zusammengeführt werden. Der Bestandsschüler wird dann in die neue Klasse gewechselt. 
+ Neu: Im Verzeichnis der Fächer (Verzeichnisse|Fächer) kann eine zusätzliche Bezeichnung im Feld 
  "Bezeichnung 2" eingetragen werden. Dieses neue Feld kann beispielsweise zur Bezeichnung des Fachs 
  in einer anderen Sprache genutzt werden.
+ Neu: Im Verzeichnis der Kurssprachen (Verzeichnisse|Weitere Schlüsselverzeichnisse|Kurssprachen) 
  kann eine zusätzliche Bezeichnung im Feld "Bezeichnung 2" eingetragen werden. Dieses neue Feld kann 
  beispielsweise zur Bezeichnung der Kurssprache in einer anderen Sprache genutzt werden.
+ Korrigiert: Unter Schüler|Bearbeiten|Sammelzuweisung|Fremdsprachen wurden weitere Werte für den Zusatz und den Status ergänzt
+ Korrigiert: SHL-SA: Problem beim Auslesen des Merkmal T1 (G8) im aktuellen Zeitraum behoben.
+ Korrigiert: (RLP-Statistik SchuelerBewegung BBS 2014.xml) Plausibilität STALA-37610
+ Korrigiert: RLP-Statistik SchuelerBewegung BBS unterscheidet zwischen Verbleiber und Abgänger. 
              Bitte dazu die Korrekturen in der Statistikdokumentation beachten.

Administrator:
+ Korrigiert: Problem beim Bereinigen vor dem Importieren des Schlüsselverzeichnisses Fächer behoben.
                                                                                                                                                                                                                               
Skripte:
+ Korrigiert: RLP => Prüfung der ABS-Neuanlage, die Plausibilität STALA 16260-2 wurde korrigiert
+ Korrigiert: RLP => Prüfung der BBS-Neuanlage, die Plausibilität STALA-29450-11 wurde korrigiert
+ Korrigiert: Zugriffsrechte synchronisieren: Kollegium 5 

Importe:
+ Magellan-Importformat-Konverter: Korrektur der IBIS Konvertierung der Betriebe  
geändert: für Berlin ist das Verzeichnis 00_Dienstbez.keys geändert worden
Bitte importieren Sie die Verzeichnisse über den Punkt Datenimporte|"Schlüsselverzeichnisse importieren" im Modul 
Magellan Administrator.


### Berichte (neu oder geändert)
+ 	Abi-Übersicht-Prüfungsergebnisse.rpt
+ 	Anwesenheitsliste (Schüler einer Klasse nach Fach).rpt
+ 	Anwesenheitsliste (Schüler nach Fach).rpt
+ 	MVP-Schullastenausgleich-Teilzeit (nicht im Landkreis Mecklenburgische Seenplatte).rpt
+ 	MVP-Schullastenausgleich-Vollzeit (nicht im Landkreis Mecklenburgische Seenplatte).rpt
+ 	Schülerliste (Bafög).rpt
+ 	Schülerliste (Klasse, Geburtsdatum und Geburtsland).rpt
+ 	Schülerliste (Nachprüflinge).rpt
+ 	RLP-FS-AS (Sozialpädagogik DIN A3).rpt
+ 	SAC-BBS-AS (Prüfungszeugnis).rpt
+ 	SAC-BF-HJI (B.01.01).rpt
+ 	SAC-BF-HJI (B.02.01).rpt
+ 	SAC-BF-HJI (B.04.01).rpt
+ 	SAC-BF-HJI (B.05.01).rpt
+ 	SAC-BF-HJZ (B.02.01).rpt
+ 	SAC-BF-HJZ (nach Anlage 9).rpt
+ 	SAC-BF-JZ (B.03.02).rpt
+ 	SAC-BF-JZ (B.04.02).rpt
+ 	SAC-BF-JZ (B.07.02).rpt
+ 	SAC-BF-ZAS (B.04.04).rpt
+ 	SAC-BG (Punktekreditkarte-2010).rpt
+ 	SAC-BG-ABI (2010).rpt
+ 	SAC-BG-ABI (E.01.06).rpt
+ 	SAC-BG-ABI (E.01.09).rpt
+ 	SAC-BG-ABI.rpt
+ 	SAC-BG-AZ (E.01.05).rpt
+ 	SAC-BG-HJZ (E.01.01).rpt
+ 	SAC-BG-HJZ (E.01.03).rpt
+ 	SAC-BG-HJZ (E.01.04).rpt
+ 	SAC-BGJ-AS mit HS (A.01.10).rpt
+ 	SAC-BGJ-AS ohne HS (A.01.11).rpt
+ 	SAC-BGJ-HJI.rpt
+ 	SAC-BGJ-JZ (nach Anlage 3).rpt
+ 	SAC-BS-AS (A.01.06).rpt
+ 	SAC-BS-AS (A.02.05) 2spaltig.rpt
+ 	SAC-BS-AS (A.02.05).rpt
+ 	SAC-BS-AS (nach Anlage 6 einspaltig).rpt
+ 	SAC-BS-AS (Vorbereitungsklasse) (A.01.06).rpt
+ 	SAC-BS-AZ (A.02.02).rpt
+ 	SAC-BS-AZ (A.02.03).rpt
+ 	SAC-BS-Bescheinigung (F.01.01).rpt
+ 	SAC-Fremdsprachenzertifikat (F.01.05).rpt





## 6.0.143 643 (19.09.2014)

### Magellan
+ Korrigiert: RLP-BBS-Neuanlage (Feld Ist in IstStunden umbenannt)
+ Korrigiert: RLP-BBS-Neuanlage (Soll ohne Aufrechnung von Solländerung)
+ Korrigiert: NRW-SIM.txt (Erkennen von Neuzugang, Verbleiber und Abgängern)
+ Korrigiert: NRW-SIM.txt (Ausspielen von Klassenleiter, auch wenn Lehrer inaktiv)
+ Korrigiert: NRW-SIM.txt (Ausspielen der Gliederung anhand des Bildungsganges der Klasse und der Ausbildung)
              Wichtig: Zum korrekten Erkennen bei der Ausbildung, muss das Von- und Bis Datum der Ausbildung 
              im entsprechenden statistischen Zeitraum liegen. 
+ Korrigiert: NRW-ABI.txt (Erkennen der Mandantenschulform am Schlüssel; Erkennen von Abiturienten, die einen neuen Bildungsgang belegen)

Administrator:
+ Korrigiert: Problem beim Bereinigen vor dem Importieren des Schlüsselverzeichnisses Kurssprachen behoben.

Importe:
Nachfolgende Schlüsselverzeichnisse wurden für Berlin aktualisiert oder stehen neu zur Verfügung. Bitte 
importieren Sie die Verzeichnisse über den Punkt Datenimporte|"Schlüsselverzeichnisse importieren" im Modul 
Magellan Administrator. Die Datei "SchulenBER_20140725.csv" kann als Schulendatei über den Punkt Datenimporte|"Magellan-Importformat" 
eingelesen werden.
- 00_AbschluesseExtern
- 00_Amtsbez
- 00_Besoldungen
- 00_Bewerbungsempfehlungen
- 00_Dienstbez
- 00_Dienstverh
- 00_Empfehlungen
- 00_Klassenorganisation
- 00_Lehraemter
- 00_LehrerAbgaenge
- 00_LehrerAusbildung
- 00_LehrerFehlgruende
- 00_LehrerFunktionen
- AS_AbschluesseIntern
- AS_Faecher
- BS_AbschluesseIntern
- BS_Berufe
- BS_Faecher
- BS_Schwerpunkte
- BS_Unterrichtsformen
- SchulenBER_20140725.csv

### Berichte (neu oder geändert)
+ Schülerliste (mit Sorgeberechtigte).rpt
+ Schülerpersonalblatt incl. Schuleintritt und -austritt (mit Vorbildung).rpt
    Für nachfolgenden Zeugnisse wurden folgenden Änderungen vorgenommen:
 -  Es wurden die Felder Namenszusatz (in Magellan unter Schüler|Daten1|Zusatz, zum Beispiel ein Namenszusatz wie "von" oder "van" ) 
    und Vorname2 (für weitere Vornamen) ergänzt. Der Aufbau ist jetzt "Vorname" "Vorname2" "Namenszusatz" "Nachname".
 -  Für Zeugnisbemerkungen können in den Zeugnissen Schlüsselwerte gesetzt werden, die im Ausdruck mit personalisierten Werten befüllt werden.
    Bemerkungen Legen Sie im Menü „Schüler“ unter „Zeugnis|Zeugnis“ oder im Menü "Abitur" unter "Zeugnis" in „Zeugnisbemerkungen“ an. Sie können 
    Zeugnisbemerkungen über Platzhalter auch personalisieren. Für die Zeugnisse wurde diese Möglichkeit auch im Modul Magellan Berichte dokumentiert.
    Einen Platzhalter definieren Sie über „<<“ zum Beginn und „>>“ zum Ende Ihres Platzhalters, z.B. So <>. 
    Möglich sind:
    <> --> Vorname, Vorname2, Namenszusatz und Nachname des Schülers
    <> --> Nachname des Schülers
    <> ---> Vorname, Vorname2 und Namenszusatz des Schülers
    <> ---> Er/Sie (je nach Geschlecht des Schülers)
    <> ---> er/sie (je nach Geschlecht des Schülers)
    <> ---> seine/ihre (je nach Geschlecht des Schülers)
    <> ---> ihm/ihr (je nach Geschlecht des Schülers)
    <> ---> seinen/ihren (je nach Geschlecht des Schülers)
+ SAC-BF-AZ (B.03.04).rpt
+ SAC-BF-AZ (B.01.02).rpt
+ SAC-BF-AS (B.07.05).rpt
+ SAC-BF-AS (B.04.06).rpt
+ SAC-BF-AS (B.04.05).rpt
+ SAC-BF-AS (B.03.05).rpt
+ SAC-BF-AS (B.01.03).rpt
+ SAC-BF-AS (A.02.07).rpt


## 6.0.142 643 (09.09.2014)

### Magellan
+ Korrigiert: Menü Klassen - Fehler beim Anlegen einer neuen Klasse korrigiert

### Berichte (neu oder geändert)
+ BER-KO-ABI (Schul Z 323)(03.11).rpt
+ Schüler (Bescheinigung-Laufbahn).rpt
+ Schülerpersonalblatt (A5 - Laufbahn).rpt
+ SAR-FHReife (Nachweis).rpt



## 6.0.141 643 (02.09.2014)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Neu: Max. Länge der Bezeichnung für die Schlüsselverzeichnisse "Abschlüsse(Intern)" und 
       "Abschlüsse(Extern)" wurden auf 300 Zeichen erweitert.   
+ Neu: Max. Länge der Felder "Name1" und "Name2" für "Schulen" wurde auf 100 Zeichen erweitert.       
+ Neu: Max. Länge für das Feld "Vertragsnr" der "SchuelerAusbildung" auf 30 Zeichen erweitert.

+ Korrigiert: NRW: Statistik ABI.TXT wird jetzt im korrekten Zeitraum durchlaufen.
  
Importe:
+ Neu: SAR: Schlüsselverzeichnis "00_Schulformen.keys" hinzugefügt, passend zum neuen Import saarländischer Schulen. Importieren Sie die Datei bitte über Importe|Schlüsselverzeichnisse importieren.
+ Neu: SAR: Import-CSV für saarländischer Schulen "schulen.import.csv". Importieren Sie die Datei bitte über Importe|Magellan-Importformat|Schulen.

Skripte:
+ Geändert: (SAR-APO-BGY-2007.dws): Berechnung der Fachhochschulreife angepasst und eine 
  Vorschlagsautomatik für die Berechnung der Fachhochschulreife integriert.
+ Korrigiert: (RLP-Statistik SchuelerNeuanlage BBS 2014.xml) Plausibilität STALA-29450-1 bis STALA-29450-11
  
Berichte:
Für nachfolgenden Zeugnisse wurden folgenden Änderungen vorgenommen:
 -  Es wurden die Felder Namenszusatz (in Magellan unter Schüler|Daten1|Zusatz, zum Beispiel ein Namenszusatz wie "von" oder "van" ) 
    und Vorname2 (für weitere Vornamen) ergänzt. Der Aufbau ist jetzt "Vorname" "Vorname2" "Namenszusatz" "Nachname".
 -  Für Zeugnisbemerkungen können in den Zeugnissen Schlüsselwerte gesetzt werden, die im Ausdruck mit personalisierten Werten befüllt werden.
    Bemerkungen Legen Sie im Menü „Schüler“ unter „Zeugnis|Zeugnis“ oder im Menü "Abitur" unter "Zeugnis" in „Zeugnisbemerkungen“ an. Sie können 
    Zeugnisbemerkungen über Platzhalter auch personalisieren. Für die Zeugnisse wurde diese Möglichkeit auch im Modul Magellan Berichte dokumentiert.
    Einen Platzhalter definieren Sie über „<<“ zum Beginn und „>>“ zum Ende Ihres Platzhalters, z.B. So <>. 
    Möglich sind:
    <> --> Vorname, Vorname2, Namenszusatz und Nachname des Schülers
    <> --> Nachname des Schülers
    <> ---> Vorname, Vorname2 und Namenszusatz des Schülers
    <> ---> Er/Sie (je nach Geschlecht des Schülers)
    <> ---> er/sie (je nach Geschlecht des Schülers)
    <> ---> seine/ihre (je nach Geschlecht des Schülers)
    <> ---> ihm/ihr (je nach Geschlecht des Schülers)
    <> ---> seinen/ihren (je nach Geschlecht des Schülers)
    
+ 	BER (Kurswahl).rpt
+ 	BER Abi-1a – Übersichtsplan über die Schullaufbahn ab 2010 – 12jähriger Bildungsgang (VO-GO) (01.12).rpt
+ 	BER-AbdGy (abi_4b_berechnungsbogen_abendgym (03.12.).rpt
+ 	BER-AbdGy-ABI (Schul Z 325)(02.11).rpt
+ 	BER-ABI (Schul II 929-3)(01.09).rpt
+ 	BER-ABI (Schul II 929-3)(09.07).rpt
+ 	BER-Abi 8 (01.12).rpt
+ 	BER-BBS (Zeugniskarte).rpt
+ 	BER-BBS-AS.rpt
+ 	BER-BF-AS (einjährig).rpt
+ 	BER-BF-AS (Schul Z 522c)(05.06).rpt
+ 	BER-BF-AS (Z 522-542).rpt
+ 	BER-BF-AS.rpt
+ 	BER-BF-AZ (einjährig).rpt
+ 	BER-BF-AZ (ohne Wahlpflicht).rpt
+ 	BER-BF-AZ.rpt
+ 	BER-BF-HJZ (einjährig).rpt
+ 	BER-BF-HJZ.rpt
+ 	BER-BF-MSA (einjährig).rpt
+ 	BER-BFS-AS (Z 522a)(04.11).rpt
+ 	BER-BFS-AZ (Schul Z 523a).rpt
+ 	BER-BFS-HJZ (Schul Z 520b)(07.09).rpt
+ 	BER-BOS-AS (Schul Z 533)(03.05).rpt
+ 	BER-BOS-AZ (Schul Z 534)(03.05).rpt
+ 	BER-BOS-FHReife (Schul Z 531)(09.05).rpt
+ 	BER-BOS-FHReife (Schul Z 532)(06.05).rpt
+ 	BER-BOS-HJZ (Schul Z 530)(03.05).rpt
+ 	BER-BQL TZ-AZ (Schul Z 507 c).rpt
+ 	BER-BQL VZ-FL-TZ (Schul Z 505 a-b-c).rpt
+ 	BER-BQL VZ-HJZ (Schul Z 505 a).rpt
+ 	BER-BQL-AZ (Schul Z 506 a)(BGL VZ).rpt
+ 	BER-BS-AS (MSA  Schul Z 502).rpt
+ 	BER-BS-AS (MSA  Schul Z 502c).rpt
+ 	BER-BS-AS (MSA  Schul Z 502d).rpt
+ 	BER-BS-AS (Schul Z 500).rpt
+ 	BER-BS-AS (Schul Z 501).rpt
+ 	BER-BS-AS.rpt
+ 	BER-BS-AZ (Schul Z 503).rpt
+ 	BER-BS-AZ (Schul Z 503).rpt
+ 	BER-BS-FHReife (Schul Z 504).rpt
+ 	BER-BS-HJZ (2006 mit Gewichtung).rpt
+ 	BER-BS-HJZ (2006).rpt
+ 	BER-BS-HJZ (Bescheinigung 2006).rpt
+ 	BER-BS-HJZ (Schul Z 500).rpt
+ 	BER-BV-AS (Schul Z 508).rpt
+ 	BER-BVJ-AS (Schul Z 506 a)(BQL VZ).rpt
+ 	BER-BVJ-AS.rpt
+ 	BER-BVJ-AZ (Schul Z 507 a)(BGL VZ).rpt
+ 	BER-BVJ-HJZ (Schul Z 505 b)(BQL FL).rpt
+ 	BER-FHReife (Bescheinigung 2).rpt
+ 	BER-FHReife-Bescheinigung (Schul Z 350)(10.07).rpt
+ 	BER-FOS-AZ (Schul Z 513)(05.06).rpt
+ 	BER-FOS-FHReife (Schul Z 511)(05.06).rpt
+ 	BER-KO-ABI (Schul Z 324)(02.11).rpt
+ 	BER-KO-AS (Schul Z 320)(06.07).rpt
+ 	BER-KO-AS (Schul Z 320a-b)(03.11).rpt
+ 	BER-KO-AS (Schul Z 322)(03.11).rpt
+ 	BER-KO-AZ (Schul Z 321)(03.11).rpt
+ 	BER-KO-AZ (Schul Z 321).rpt
+ 	BER-KO-ZAS (Schul Z 371)(02.12).rpt
+ 	BER-RS-AS (Schul Z 240)(03.08).rpt
+ 	BER-RS-AS (Schul Z 241)(07.10).rpt
+ 	BER-RS-AZ (Schul Z 242)(06.08).rpt
+ 	BER-RS-AZ (Schul Z 242)(07.05).rpt
+ 	BER-Schul Z 102 (11.10).rpt
+ 	BER-Schul Z 202 (07.10).rpt
+ 	BER-Schul Z 302 (12.07).rpt
+ 	BER-Schul Z 306 (09.12).rpt
+ 	BER-Schul Z 350 (10.07).rpt
+ 	BER-Schul Z 510 (12.13).rpt
+ 	NRW-ABI-AZ  (Anlage D42).rpt
+ 	NRW-Abitur (Prüfungsergebnisse 1).rpt
+ 	NRW-Abitur (Prüfungsergebnisse 2).rpt
+ 	NRW-BBS-AG-AS-JZ-HZ (A01-A04).rpt
+ 	NRW-BBS-JZ-HJ-AG-AS (A05-A06).rpt
+ 	NRW-BBS-JZ-HJ-AG-AS (A07).rpt
+ 	NRW-Bescheinigung (Nichtzulassung Abitur D37).rpt
+ 	NRW-BF-FHReife (Anlage C17 schulischer Teil).rpt
+ 	NRW-BG-AS (Anlage D 48).rpt
+ 	NRW-BG-HJZ VZ Jahrgangsstufe 11 (Anlage D32).rpt
+ 	NRW-BK-ABI (Anlage D33a).rpt
+ 	NRW-BK-ABI (Anlage D33b - 2014).rpt
+ 	NRW-BK-ABI (Anlage D33b).rpt
+ 	NRW-BK-ABI (Anlage D34).rpt
+ 	NRW-BK-ABI (Anlage D41 - 2012).rpt
+ 	NRW-BK-ABI (Anlage D41).rpt
+ 	NRW-BK-AS (Anlage E4).rpt
+ 	NRW-BK-AZ (Anlage D 31).rpt
+ 	NRW-BK-AZ (Anlage D30).rpt
+ 	NRW-BK-AZ (Anlage D35).rpt
+ 	NRW-BK-AZ (E01-0A).rpt
+ 	NRW-BK-JZ (Anlage C14 - 1 Seitig).rpt
+ 	NRW-BK-JZ (Anlage C14 - 2 Seitig).rpt
+ 	NRW-BKO-ABI (Bescheinigung Schullaufbahn).rpt
+ 	NRW-BKO-ABI (Bescheinigung Schullaufbahn2).rpt
+ 	NRW-BKO-ABI (Bescheinigung Schullaufbahn3).rpt
+ 	NRW-BKO-ABI (Bescheinigung Schullaufbahn4).rpt
+ 	NRW-BKO-ABI.rpt
+ 	NRW-BKO-AS (2007).rpt
+ 	NRW-BKO-AZ (2007).rpt
+ 	NRW-BS-AS (A01).rpt
+ 	NRW-E01-6A-J (Fachschulabschluss +- FHR).rpt
+ 	NRW-Zertifikat.rpt

### Berichte (neu oder geändert)     
+ 	Alle Ausleihvorgaenge pro Schueler (nach Klassen gruppiert).rpt
+ 	BAW-BG-ABI (DIN A4 doppelseitig 2010).rpt
+ 	RLP-BBS (Bescheinigung Niveaustufen).rpt
+ 	RLP-BG-ABI (2010)A4.rpt
+ 	SAR-FHReife (Nachweis).rpt
+ 	SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
+ 	Etiketten (No.3651 - 52,5 x 29,7 mm - 1fach).rpt
+ 	Klassenliste Schüler-Notenmatrix (Querformat-Durchschnitt).rpt
+ 	Mandant (SchülerAbgang).rpt
+ 	Mandant (SchülerNachprüfung).rpt
+ 	Schüler (Wiederholer innerhalb eines Schuljahres).rpt
+ 	Schüler mit Herkunftsschulen u. letzte Klasse.rpt
+ 	Schülerliste (gruppiert nach Bildungsgängen).rpt
+ 	Zeugnisliste (Schuljahr).rpt
  


## 6.0.140 642 (15.07.2014)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Neu: Die Landesstatistik Schleswig-Holstein 2014/2015 und Nordrhein-Westfalen 2014/2015 wird mit dieser Ausgabe freigegeben. Bitte 
  beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf 
  
+ Neu: (RLP-Statistik) die Schlüsseldatei für die SchuelerMerkmale für ABS und für BBS wurden geändert. 
       Neu ist der Schlüssel "Ausschluss" mit dem Wert "J" und der Bezeichnung "Schüler von der Statistik ausschließen" Für das Feld Schüler|Statistik|MerkmalS7. 
       Sie können damit einzelne Schüler von der statistischen Auswertung ausschließen.
+ Neu: Kontextsensitive Suche in der Magellan-Standardansicht: Je nach aktiver Ansicht wird gleich der entsprechende Suchbereich angezeigt.  
+ Neu: Statusfeld der Klasse zeigt die Anzahl der Schüler der ausgewählten Klasse nach Geschlecht
+ Neu: Anlegen von Schulen direkt aus den Dialogen "Extras|Schüler ausschulen" und 
       "Schüler|Zugang/Abgang|Bereits besuchte Schulen|Schulbesuche editieren/hinzufügen"
+ Neu: Eingestellter Filter in den Start-Auswahllisten der Ansichten werden gespeichert
+ Neu: Dublettenprüfung komplett überarbeitet, Prüfung der Sorgeberechtigten anhand von Vor- und Nachname hinzugefügt.  
+ Neu: neue Felder für den SchülerSorgeberechtigten "Briefanrede" und "Briefempfänger". Die Felder werden für bereits erfasste SchülerSorgeberechtigte vorbesetzt 
       (Briefempfänger z.b. Herrn Müller, Briefanrede: Sehr geehrter Herr Müller,) Für das Vorbesetzten wird die Anrede des Sorgeberechtigten ausgewertet. Bei einem 
       Schüler neu zugewiesenen Sorgeberechtigten werden die Felder vorbesetzt, können für Eltern mit unterschiedlichen Nachnamen aber manuell ergänzt werden. 
       Bitte verwenden Sie diese neuen Felder in Ihren Serienbriefen für den Adressblock und die Briefanrede.
       Als Beispiel wurde auch die Vorlage "Brief an Sorgeberechtigte des Schülers.dot" angepasst.
+ Neu: in der Magellan-Standardansicht: Beim Ändern der Adressdaten eines Schülers/Bewerbers oder eines Sorgeberechtigten erscheint beim Speichern ein Dialog, der das gleichzeitige Mitanpassen der Adressendaten
       des Schülers/Bewerbers oder des/der Sorgeberechtigten ermöglicht. Geprüft werden die Felder Postleitzahl, Ort und Straße, werden die identischen Daten beim Schüler oder Sorgeberechtigten gefunden, wird die Änderung angeboten.     

### Magellan-Bibliothek:
+ Korrigiert: Bericht "Etiketten (No.3651 - 52,5 x 29,7 mm - 1fach).rpt". Titel wird zweizeilig ohne Zeichenbegrenzung angezeigt.
+ Korrigiert: Bei Ansichten, die Medienkataloge erfordern wird geprüft, ob mind. ein Medienkatalog vorhanden ist, 
              um die Ansicht darstellen zu können. Anderenfalls wird eine entsprechende Meldung ausgegeben und der Zugriff auf die Ansicht verweigert.
              
### Berichte (neu oder geändert)
+ BER-GY-ABI (Schul Z 306)(09.12).rpt
+ BER-GS-JZ (Schul Z 103)(11.05).rpt
+ BER-GS-JZ (Schul Z 103)(11.05) (französ. Gymn).rpt
+ SAC-BS-JZ (A.02.01).rpt
+ SAR-FHReife (Nachweis).rpt
+ Etiketten (No.3651 - 52,5 x 29,7 mm - 1fach).rpt
+ Alle Ausleihvorgaenge pro Schueler (nach Klassen gruppiert).rpt
+ Quittung(DIN A5).rpt
+ Schülerliste (mit Ausbildungsbetrieben und Geburtsdatum).rpt              
   

## 6.0.139 641 (04.07.2014)

### Magellan
+ Korrektur: (BER) Problem beim Export der Abiturdatenstatistik behoben
+ Korrektur: (BER) Polnisch wird als Fach aus dem Schlüssel 065 abgeleitet und als "P" in der Abiturdatenstatistik übergeben
+ Korrektur: (RLP) Landesstatistiklizenz wird unter Hilfe|Lizenz mit aufgelistet
+ Korrektur: Bewerberemail wird in voller Länge für den Seriendruck übergeben

### Berichte (neu oder geändert)
+ SAC-BS-JZ (A.02.01).rpt
+ SAR-FHReife (Nachweis).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ SHL-GY-ABI (2011).rpt
+ SAC-BGJ-AS ohne HS (A.01.11).rpt
+ SAC-BGJ-AS mit HS (A.01.10).rpt
+ SAC-BVJ-AS ohne HS (A.01.09).rpt




## 6.0.138 641 (27.06.2014)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan 
+ Neu: Die Landesstatistik Rheinland-Pfalz 2014/2015 wird mit dieser Ausgabe freigegeben. Bitte 
  beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf

Skripte:
+ Neu: (BER-APO-FOS-2013):  enthält gegenüber dem BER-APO-FOS-2006 die Änderungen, das Sport als Prüfungsfach im Gesamtdurchschnitt berückschtigt wird
+ Geändert: (BER-APO-2011.dws): neu einsetzende zweite Fremdsprache, Geschichte als Prüfungsfach, künstlerisches Fach und neu einsetzende Fremdsprache
+ Geändert: (BER-FW-APO-2011.js): neu einsetzende zweite Fremdsprache, Geschichte als Prüfungsfach, künstlerisches Fach und neu einsetzende Fremdsprache
+ Geändert: (BER-APO-KO-2011.dws): Rundungsregeln an Verordnungsänderung angepasst
+ Geändert: (NIE-APO-G9-2014.dws): Bei der Prüfung von Unterkursen wir jetzt auch das mündliche Prüfungsfach 
  korrekt mit berückschtigt

### Berichte (neu oder geändert)
+ BER-GY (Abi-18a - Mitteilungen zu den schriftlichen und mündlichen Prüfungen)(03.12).rpt
+ RLP-BG-ABI (2010).rpt
+ RLP-BG-ABI (2010)A4.rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ SAC-BG-ABI (E.01.06).rpt
+ SAC-BGJ-AS mit HS (A.01.10).rpt
+ SAC-BGJ-AS ohne HS (A.01.11).rpt
+ SAC-BVJ-AS mit HS (A.01.08).rpt
+ SAC-BVJ-AS ohne HS (A.01.09).rpt
+ SHL-GY-ABI (2011).rpt
+ SHL-GY-HJZ (Profil).rpt
+ Etiketten (No.3651 - 52,5 x 29,7 mm - 1fach).rpt


## 6.0.137 641 (17.06.2014)

MyMagellan-Center:
+ Korrektur: Problem behoben für Dateien mit im MyMagellan-Center vergebenen Passwort (Kennwort für Teilnehmer ohne MyMagellan-Kennwort)
WICHTIG: Bitte MyMagellan-Dateien, die mit dieser Version erstellt werden, können nur mit der parallel veröffentlichten Version ## 6.0.14 bearbeitet werden.

Skripte:
+ Geändert: (BER-APO-FOS-2006): Sport wird als Prüfungsfach in der Berechnung berückschtigt

### Berichte (neu oder geändert)
+ RLP-BG-ABI (2010)A4.rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ RLP-BG (Punktekreditkarte-2010).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 2).rpt
+ SAC-BVJ-AS mit HS (A.01.08).rpt
+ SAC-BVJ-AS ohne HS (A.01.09).rpt



## 6.0.136 641 (13.06.2014)

MyMagellan-Center:
WICHTIG: die mit dieser MyMagellan-Center-Version erstellen mym-Dateien müssen mit der parallel 
erscheinenden MyMagellan-Version (## 6.0.13) bearbeitet werden.
+ Neu: Die erzeugten MyMagellan-Dateien sind jetzt immer verschlüsselt.

### Berichte (neu oder geändert)
+ SHL-GY-HJZ (Profil).rpt
+ SAC-BG-ABI (E.01.06).rpt
+ BER-ABI (Schul II 929-3)(01.09).rpt



## 6.0.135 641 (11.06.2014)

### Bibliothek:
+ Optionen | Allgemein | Vorgang: Möglichkeit das automatische Löschen der historischen Vorgänge auszuschalten
  und zusätzlichen Hinweistext zu den Konsequenzen bei Änderung dieser Option eingetragen.  
+ Vorgänge | Historie: Wenn das automatische Löschen der historischen Vorgänge angeschaltet ist,
  wird jedesmal nachgefragt, bevor eine Löschung stattfinden soll. 
 
### Administrator:
+ Korrigiert: beim Importieren vom Fächern (Verweis auf Kurssprachen)
+ Neu: Unter Datenbankpflege|Datenbank überprüfen|Gemeinden synchronisieren wird auch nachträglich der Stadtbezirk zugewiesen, wenn die Postleitzahl und der Ort erkannt wird
+ Neu: (nur für RLP Berufsschulen)Unter Datenbankpflege|Datenbank überprüfen gibt es den Punkt "RLP Berufskennziffern austauschen".

### Importe:
+ Neu: (nur für RLP) Schlüsselimportkataloge für die Herbststatistik

### Skripte:
+ Korrigiert: (RLP-BGY-APO-2010) Einbringungspflicht 13/2-Ergebnis in VWL
+ Geändert: (BER-APO-2011) Verordnungsänderung -> Anpassung der Berechnung für die Prüfungsergebnisse (aus schriftl. und mdl. Prüfung) 
+ Geändert: (BER-APO-FOS-2006): Übernahme des 10. und 11.PFs

### Berichte (neu oder geändert)
+ BER-GY-ZAS (Schul II 929-11a)(01.09).rpt
+ BER-KO-ABI (Schul Z 324)(02.11).rpt
+ NRW-Abitur (Prüfungsergebnisse 2).rpt
+ SAC-BGJ-AS mit HS (A.01.10).rpt
+ SAC-BS-Bescheinigung (F.01.01).rpt
+ SAC-BS-JZ (A.02.01) 2spaltig.rpt



## 6.0.134 641 (20.05.2014)

### Magellan
+ MagSDTF.exe für den Untis-Export erneuert
+ Änderung des Typs der Zeugnisformulare wird bei den bereits an Schüler zugewiesenen Zeugnisformularen korrekt übernommen
+ Neu: Protokollierung von Änderungen in der Datenbank. Bitte beachten Sie unsere neues Kapitel "23 Protokollierung in Magellan" 
  im Magellan-Benutzerhandbuch Magellan6.pdf. Hier erläutern wir, wie Sie das Ändern, Einfügen und Aktualisieren von Daten 
  in der Magellan-Datenbank in einer Logdatei festhalten können.
 + Änderung: Abiturdatenschnittstelle Berlin: für Berufskollegs wird der Status 5PF und das Häkchen  "Besondere Lernleistung" 
 (Abitur|Prüfung) ausgewertet um zwischen Präsentationsprüfung (Häkchen deaktiviert) und Besonderer Lernleistung (Häkchen aktiviert) zu unterscheiden

 
### Skripte:
+ Korrigiert: (NIE-APO-2014-G8/NIE-APO-2014-G9) Rundung im BlockI-Ergebnis
+ Korrigiert: (RLP-BGY-APO-2010) 
  - Unterstützt jetzt auch die Fachrichtung "Gesundheit und Soziales"
  - Fachhochschulreife korrigiert
+ Korrigiert: (RLP-APO-2010) Fachhochschulreife korrigiert
+ Korrigiert: (BER-APO-2011):
  - Markierung:  Bei Neueinsetzen einer zweiten Fremdsprache in der Einführungsphase, entfällt die Verpflichtung ein 
    künstlerisches Fach zu belegen 
+ Korrigiert: (BER-FW-APO-2011): neu einsetzende Fremdsprache kann Referenzfach zur 5.PK sein

### Berichte (neu oder geändert)
+	BER-Abi 8 (01.12).rpt
+	BER-FOS-FHReife (Schul Z 511)(05.06).rpt
+	NRW-BG-AS (Anlage D 48).rpt
+	SAC-BGJ-AS ohne HS (A.01.11).rpt
+       SAC-BGJ-AS mit HS (A.01.10).rpt
+	SAC-BS-AS (Vorbereitungsklasse) (A.01.06).rpt
+	SAC-BS-Bescheinigung (F.01.01).rpt
+	SAC-BV-HJI (A.01.01).rpt
+	SAC-BVJ-AS mit HS (A.01.08).rpt
+	SAC-BVJ-AS ohne HS (A.01.09).rpt
+	SAC-FS-AS (C.01.11).rpt
+	Bewerber gruppiert nach Bewerberstatus.rpt
+	Bewerber gruppiert nach Gesamtnote.rpt
+	Schülerpersonalblatt incl. Schuleintritt (Betriebe).rpt



## 6.0.133 641 (13.04.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Neu: Unter "Ansicht Klassen | Daten" gibt es ein neues Feld "Nächste Klasse". Hier kann man 
  über "Bearbeiten | Nächste Klasse" die Nachfolgeklasse einer Klasse definieren.
+ Neu: Unter "Ansicht Klassen | Auswahl" können jetzt zusätzlich die Spalten "Nächste Klasse" und 
  "Zeitraum nächste Klasse" angezeigt werden.
+ Erweitert: Unter "Ansicht Abitur" werden unter "Bearbeiten | Fachwahlen exportieren" jetzt auch die 
  nächste Klasse mit berückschtigten. Dadurch können auch Fachwahlen von Schülern z.B. in der Klasse 10 
  mit der korrekten nächsten Klasse 11 exportiert werden.   
+ Neu: in der Auswahlliste der Ansicht Abitur wird der Durchschnitt ABI + Durchschnitt FHR 
eingeblendet
+ Neu: Für Berlin werden für die Abiturschnittstelle 2014 beim Export nur die Schüler 
berücksichtigt, für deren Klasse unter Klassen|Daten|Statistikkürzel ein Wert erfasst wurde.

### Skripte:
+ Korrigiert: (NRW-APO-BK-2012.dws) 

### Berichte(neu oder geändert):
+ NRW-BK-ABI (Anlage D41 - 2012).rpt
+ NRW-BK-ABI (Anlage D33b - 2014).rpt
+ SHL-GY-HJZ (Profil).rpt
+ RLP-BG-ABI (2010).rpt
+ Lehrer (Personalhandkarte).rpt


## 6.0.132 640 (07.04.2014)

### Magellan
+ Neu: In der Ansicht "Schüler" bzw. "Bewerber" wurden die Sammelzuweisung erweitert. Die Spalten 
  "Bewerbungsziel 1" ... "Bewerbungsziel 4" werden zusätzlich bei der Auswahl der Schüler bzw.
  Bewerber angezeigt.
+ Neu: Für Berlin wird die Abiturschnittstelle 2014 mit dieser Ausgabe freigegeben. Bitte beachten Sie 
  dazu das aktualisierte Dokument Magellan6Berlin.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan6Berlin.pdf

### Magellan-Administrator:
+ Korrigiert: Allgemeines Importformat|Import schueler.csv BewerberNote korrigiert
  - Einbringung neu einzusetzenden Femdsprache korrigiert 

### Magellan-Bibliothek:
+ Korrektur: Medienstatuskontrolle

### Skripte:
+ Korrigiert: (NRW-APO-BK-2012.dws) 
  - Korrektur der Rundung 
  - Berücksichtigung von Fremdsprachen die nur ab der Klasse 12 belegt werden 
  - Berücksichtigung von nicht eingebrachten Kursen mit 0 Punkten
  
### Berichte (neu oder geändert)
+ BAW-Abiturprüfung-Erstkorrektur.rpt
+ BER-BF-AS (Z 522-542).rpt
+ SAC-BG (Punktekreditkarte-2010).rpt
+ SAC-BS-AZ (A.02.04) 2spaltig.rpt
+ SAC-BS-AZ (A.02.04).rpt
+ RLP-BG-ABI (2010)A4.rpt
+ RLP-BG-ABI (2010).rpt
+ NIE-GY-ABI (2014).rpt
+ NRW-BG-AS (Anlage D 48).rpt
+ NRW-Abitur (Prüfungsergebnisse 2).rpt
+ NRW-BK-ABI (Anlage D41 - 2012).rpt
+ NRW-BK-ABI (Anlage D33b - 2014).rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 2).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-GY-ABI (2010-G8-G9) (A4 Seite 1).rpt
+ RLP-GY-ABI (2010-G8-G9)A4.rpt
+ SAR-GY-Verhaltenszeugnis.rpt
+ SAR-GY-HJZ-JZ (Klassenstufen 5-9).rpt
+ SAR-GY-AZ (modifiziert Klassenstufe 9).rpt
+ SAR-GY-AZ (Klassenstufen 5-9).rpt  
+ Mandant (Statistik Abschlüsse).rpt
+ Medienliste (Inventur).rpt
+ Schüler (gruppiert nach Herkunftsschulen).rpt
+ Schulbescheinigung (mit Klasse und vorauss. Ende einfach).rpt


## 6.0.131 640 (10.03.2014)

### Magellan
+ Korrigiert: Import von SchülerOnline (NRW): sich erneut an Ihrer Schule bewerbende Schüler, können 
anhand Ihrer MagellanID+Schulnummer erkannt werden. Bei Übereinstimmung wird der bestehende 
Schülerdatensatz als Bewerberdatensatz dupliziert, die IDIntern wird gefüllt, um anschließend 
Bewerber und Schüler zusammenführen zu können, der Bewerber wird dabei gelöscht. Voraussetzung 
dafür ist, dass Sie Ihre Abgänger nach SchülerOnline übergeben haben. 

### Skripte:
+ Korrigiert: (RLP-APO-BGY-2010.dws) Neu einsetzende Fremdsprache, Vorschlag für mdl. Noten für 4. und 5.PF korrigiert
+ Korrigiert: (RLP-APO-2010.dws) Vorschlag für mdl. Noten für 4. und 5.PF korrigiert
+ Korrigiert: (BER-APO-2010.dws) bei manuellem Demarkieren des 4.PFs wird  gewarnt

### Magellan-Administrator: 
+ Korrigiert: Allgemeines Importformat|Import schueler.schulen.csv korrigiert

### Berichte (neu oder geändert)
+ BRA-GY-ABI (2013).rpt
+ NRW-BK-ABI (Anlage D33b - 2014).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt


## 6.0.130 640 (25.02.2014)

### Magellan
+ Neu: Im Verzeichnis "Fächer" gibt es die neue Kategorie "Recht"
+ Korrigiert: Problem beim Erfassen von mehreren Bewerbern aus der Ansicht Bewerber|Daten1 behoben
+ Korrigiert: (Schüler einschulen.dws) Beim Zusammenführen eines inaktiven Schülers und seiner 
Bewerberkopie, wird der Status des Schüler auf aktiv gesetzt
+ Korrigiert: Beim Anlegen einer Zeile unter Verzeichnisse|Bewerbungsziele wird kein Schlüssel 
erwartet
+ Korrigiert: nach dem Beenden der Abitursimulation ohne Datenübernahme werden die Inhalte der 
Ansichten "Qualifikation" und "Prüfung" korrekt dargestellt
+ Neu: (CH) Neue Rundungsmethode fürs kaufmännische Runden in Magellan integriert, aufrufbar per 
Skript

### Administrator:
+ Korrigiert: Import der Kataloge "BetreuungAusserschulisch" und "BetreuungInnerschulisch"  
korrigiert

### Skripte:
+ Korrigiert: (RLP-APO-BGY-2010.dws) Berechnung Fachhochschulreife, 
+ Korrigiert: (RLP-APO-2010.dws) Berechnung Fachhochschulreife + Besondere Lernleistung, Einbringung
aller Pflichtkurse aus 13/1, 
+ Neu: (RLP-APO-2010.dws) Mindestpunktzahl wird für 4.PF bzw. 5.PF für mündliche Prüfung angezeigt  
+ Korrigiert: (BER-FW-APO-BBS-2011.js, BER-FW-APO-2011.js)
+ Korrigiert: (BER-APO-2011.dws) Einbringung von Zusatzkursen; Kategorie Musik und Psychologie; 
Einbringungsverpflichtung Sporttheorie
+ Korrigiert: (BER-APO-KO-2011.dws) Einbringung von Zusatzkursen; Kategorie Musik und Psychologie; 
Einbringungsverpflichtung Sporttheorie
+ Neu: (BER-FW-APO-2011.js)Im Verzeichnis der Verordnungen muss man bei der Definition der 
Fachwahlverordnung in der Spalte "Typ" den Wert "G8" angeben, wenn es ein G8-Abitur ist (d.h. 
zweijährige Form). Keine Angabe in der Spalte "Typ" ist G9-Abitur (d.g dreijährige Form).
Geprüft wird nun wie folgt. Der Fachschlüssel von Sport-Praxis ist im Fachwahlskript fest mit dem 
Wert "129" angegeben, so wie er im Fächerverzeichnis (entscheident ist der Eintrag beim Schlüssel 
des Faches) steht. Gezählt wird: LK = 5 Std, GK=3 Std, Ausnahme Sport-Praxis= 2 Std.

### Berichte (neu oder geändert)
+ BER-Schul Z 302 (12.07).rpt
+ BRA-GY-ABI (2013).rpt
+ NRW-BK-ABI (Anlage D33a).rpt
+ RLP-BG (Punktekreditkarte-2010).rpt
+ RLP-BG-ABI (2010).rpt
+ RLP-FO-FHReife (DIN A3).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-GY-HJZ (11-13).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ SAC-BS-HJI (A.01.02).rpt
+ SAC-BS-HJI (A.01.04).rpt
+ SAC-BV-HJI (A.01.01).rpt
+ Lehrer (Personalhandkarte).rpt
+ Mandant (Statistik Abschlüsse).rpt
+ Schülerliste (gruppiert nach Berufen).rpt
+ Schülerliste (gruppiert nach Betrieben).rpt
        
## 6.0.129 640 (04.02.2014)

### Magellan

### Skripte:
+ Korrigiert: NIE-APO-G9-2014.dws
    - doppelte Wertung des 3PF in Block I
    - Block II Wertung bei 3 Unterkursen
+ Korrigiert: RLP-APO-2010.dws
    Kategorie: Darstellendes Spiel wird erkannt
+ Korrigiert: RLP-APO-BGY-2010.dws 

### Berichte (neu oder geändert)
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-BG-ABI (2010).rpt
+ RLP-BG (Punktekreditkarte-2010).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ SHL-GY-HJZ (Profil).rpt
+ SAC-BG-HJZ.rpt
+ SAC-BS-HJI (A.01.04).rpt
+ NIE-GY-ABI (2014).rpt


## 6.0.128 640 (16.01.2014)

### Magellan     

+ Korrigiert: Drucken und Archivieren als PDF bei Filterungen in der Auswahlliste "Schüler"
+ Neu: Unter "Ansicht Lehrer | Daten 3 | Lehrämter" kann man zusätzlich die Lehramtstypen
  "Lehrbefähigung kleine Fakultas" und "Lehrbefähigung große Fakultas" auswählen.
+ Neu: im Bewerbermenü werden in der Auswahlliste die Spalten "Rangzahl Bewerbungsziel 1" bis "Rangzahl Bewerbungsziel 4" eingeblendet. 
Bitte beachten Sie unsere erweiterte Beschreibung im Kapitel "5.4 Bewerberverfahren durchführen" im Magellan6.pdf.
+ Korrigiert: die Ausbildungsbemerkung unter Schüler|Ausbildung wurde eingeblendet
+ Korrigiert: Erstellen eines Rankings mit Priorität auf der Hauptfachnote

### Administrator

+  Korrigiert: Anlegen eines neuen Benutzers ohne MyMagellan Kennwort

### Statistik

+ Neu: Die Landesstatistik Niedersachsen ABS 2013/2014 wird mit dieser Ausgabe freigegeben.

### Skripte

+ Geändert: NIE-APO-G9-2014.dws
+ Geändert: NIE-APO-G8-2014.dws
+ Korrigiert: (RLP-APO-2010.dws) 
  - Diverse Korrekturen
  - Der Fachstatus "1PF", "2PF" bzw. "3PF" wird für die Leistungskurse auf der Registerkarte "Qualifikation"
    automatisch zugeordnet, falls kein Fachstatus gesetzt ist und die Schaltflächen "Initialisieren" oder "Vorschlag" 
    gedrückt werden.  
+ Korrigiert: (BER-APO-2011.dws) Fachhochschulreife: Zulässige einzubringende Halbjahre 
+ Korrigiert: (BER-APO-KO-2011.dws) Fachhochschulreife: 
  - Zulässige einzubringende Halbjahre
  - Summe der Leistungskurse
  - Doppelt gewichteter bester Grundkurs
+ Korrigiert: (SAC-APO-BGY-2011.dws): Berechnung der Durchschnittsnote
+ Korrigiert: Importiere SDTF.dws: Übertrag vom Lehrerunterricht für Nicht-Oberstufenklassen (UArt; Kurs, KursNr:0)  
  
### Schlüsselimportdateien

+ Geändert: (Berlin) 
  AS_Faecher.keys
  BS_Faecher.keys
  00_Kurssprachen.keys
  00_Staatsangehoerigkeiten.keys
  00_Muttersprachen.keys 
   
### Importdateien

 + Neu: (Berlin) Es steht eine aktualisierte CSV-Datei der Berliner Schulen zur Verfügung. 
 Bitte importieren Sie die Daten über Magellan-Administrator|Datenimporte|Magellan-Importformat. 
 Die Datei befindet sich auf dem Serverrechner unter Magellan 6|Importe|Berlin|SchulenBER_2014.01.14.csv
 
### Berichte (neu oder geändert)

+ RLP-BG-ABI (2010).rpt
+ RLP-GY-ABI (2010-G8-G9).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ SHL-GY-HJZ (Profil).rpt
+ Schülerliste (Einschulmerkmal1 sortiert nach Bewerber-Gesamtnote, Punkte, HF-Note).rpt

## 6.0.127 640 (19.12.2013)

### Magellan
+ Neu: Unter "Ansicht Schüler|Zeugnis|Fächer" wird im Assistenten "Fachtafel zuweisen" bei Auswahl der Schüler 
  zusätzlich die Spalte "Bildungsgang Bezeichnung" angezeigt. 
+ Neu: Unter "Ansicht Abitur|Auswahl" werden die neuen Spalten "Fachwahl gültig" und "Fachwahl berechnet" angezeigt.
+ Neu: Berlin: Bei den Sammelzuweisungen für Schüler bzw. Bewerber (Ansicht Schüler  bzw. Bewerber|Bearbeiten|Sammelzuweisung)
  werden jetzt auch die Felder der Registerkarte "Ansicht Schüler|Statistik" bzw. "Ansicht Schüler|Statistik" bei der Auswahl
  der Berliner Masken berückschtigt.
+ Neu: Im Dialogfenster zur Auswahl eines Betriebs (Dialog "Betrieb auswahlen") werdne jetzt die zuletzt gewählten Filter für Filter 1
  und Filter 2 (z.B. Kürzel, Name1 usw.) benuttzerspezifisch gespeichert. 
+ Korrigiert: Problem beim Neuanlegen von Personen und anschließendem Wechsel auf die Registerkarte "Daten 1" behoben

### Skripte:
+ Geändert: (SHL-Statistik DATEA 2013.xml) EA37, EA94, EA86, EA27
+ Korrigiert: (BER-APO-2011.dws) Fachhochschulreife: Leistungskurse werden doppelt gewichtet
+ Korrigiert: (RLP-APO-2010.dws) Fachhochschulreife: Berechnung der Leistungskurse ist jetzt korrekt
+ Geändert: NIE-APO-G9-2014.dws

### Berichte (neu oder geändert)
+ BER-GY-AZ (Schul Z 303)(12.07).rpt
+ BER-Schul Z 302 (12.07).rpt
+ MVP-GY-AS (Jahrgangsstufe 7-10).rpt
+ RLP-BG (Punktekreditkarte-2010).rpt
+ RLP-GY-ABI (2010).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ SAC-BG-HJZ (E.01.01).rpt
+ Schülerliste (mit Sorgeberechtigte französisch).rpt

## 6.0.126 640 (27.11.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Geändert: für die RLP-BBS-Bewegungsdatei wird das Abschlussdatum nicht mehr berücksichtigt
+ Korrigiert: MVP: Extras|Export|SIP-Schnittstelle gibt auch Daten aus, wenn das Feld Anrede nicht gefüllt ist
+ Korrigiert: Für Kollegium 5 wurde die Anzeige der Lehrerdaten auf den eigenen Datensatz beschränkt
+ Neu: in den Auswahllisten der Masken(Berlin) sind die nachfolgenden Spalten neu. 
  Bitte beachten Sie, dass diese Spalten standardmäßig ausgeblendet sind und in den Menüpunkten Bewerber und Schüler über Bearbeiten|Spalten bearbeiten eingeblendet werden können.
  Für die Schülerauswahlliste(Berlin):
    - Anrede
    - Geburtsname
    - Geburtsland
    - Adresszusatz
    - Gemeinde
    - Stadtbezirk
    - Staatsangehörigkeit 2
    - In Deutschland seit
    - Aufenthaltserlaubnis bis
    - Ndh (= nicht deutscher Herkunft)
    - Aussiedler
    - Förderschwerpunkt
    - Beeinträchtigung
    - Schularzt
    - Krankenkasse
    - Berlinpass
    - Berlinpass bis
    - BAFöG
    - BAFöG bis
    - Lernmittel befreit
    - Lernmittel befreit bis
    - Teilnahme Mittagessen
    - Rel.-Teilnahme
    - Klassenart
    - Klasse Schulart
    - Schulbeginn
  Für die Bewerberauswahliste (Berlin):    
    - Anrede
    - Geburtsname
    - Geburtsland
    - Adresszusatz
    - Gemeinde
    - Stadtbezirk
    - Staatsangehörigkeit 2
    - In Deutschland seit
    - Aufenthaltserlaubnis bis
    - NdH (= nicht deutscher Herkunft)
    - Aussiedler
    - Förderschwerpunkt
    - Beeinträchtigung
    - Schularzt
    - Krankenkasse
    - Berlinpass
    - Berlinpass bis
    - BAFöG
    - BAFöG bis
    - Lernmittel befreit
    - Lernmittel befreit bis
    - Teilnahme Mittagessen
    - Rel.-Teilnahme
    - Schulbeginn

### Statistik

+ Korrigiert: SHL: DATSA: Plausibilitäten SA51 und SA52
+ Korrigiert: SHL: Gastschüler werden auch bei der Plausibilität nicht mehr berücksichtigt.
+ Korrigiert: SHL: DATOS: Kursdatensätze werden klassenübergreifend gebildet

### Skripte

+ Geändert: Für Extras|Import|Untis|übernehme Lehrerunterricht wurde eine Anpassung zur parallelen Untis-Änderung vorgenommen

### Berichte (neu oder geändert)
+	BER Abi-1a – Übersichtsplan über die Schullaufbahn ab 2010 – 12jähriger Bildungsgang (VO-GO) (01.12).rpt
+	BER-BF-AS (Z 522-542).rpt
+	BER-BS-AZ (Schul Z 503).rpt
+	BER-FHReife-Bescheinigung (Schul Z 350)(10.07).rpt
+	BER-GY (abi_4_berechnungsbogen)(09.12).rpt
+	BER-GY-ABI (Schul Z 306)(01.09).rpt
+	BER-GY-ABI (Schul Z 306)(09.12).rpt
+	BER-Schul Z 302 (12.07).rpt
+	BRA-GY-Abi (Formblatt 20-Festlegung der Gesamtqualifikation).rpt
+	BRA-GY-Abi( Formblatt 09-Mitteilung über die Ergebnisse in den Abiturprüfungen).rpt
+	BRA-GY-AZ-AS (Abitur-2009).rpt
+	MVP-GY-AZ (2013).rpt
+	NRW-BK-ABI (Anlage D33a).rpt
+	NRW-E01-6A-J (Fachschulabschluss +- FHR).rpt
+	NRW-Schülerstammblatt.rpt
+	RLP-BG-Punktekreditkarte-2012.rpt
+	RLP-FO (HJZ-JZ-AZ).rpt
+	RLP-GY-AS (11-13).rpt
+	RLP-GY-Punktekreditkarte-2012.rpt
+	SAC-BGJ-HJI.rpt
+	SAC-BS-JZ (A.02.01) 2spaltig.rpt
+	SAC-FS-AS (C.01.08).rpt
+	SAC-FS-AS (C.01.09).rpt
+	SAR-FHReife (Nachweis).rpt
+	SAR-GY-HJZ-JZ (Klasse 5-9).rpt
+	Abiturprüfung-Ergebnisse (Erst- und Zweitkorrektur sowie Endbewertung).rpt
+	Alle Ausleihvorgaenge pro Schueler (nach Klassen gruppiert).rpt
+	Alle Ausleihvorgaenge pro Schueler (nach Klassen und Medien gruppiert).rpt
+	Betriebe mit Auszubildenden (Alle Zeiträume).rpt
+	Klassenliste (Durschnittsnoten Abitur).rpt
+	Klassenliste mit Fächern.rpt
+	Klassenliste Schüler-Notenmatrix (Querformat).rpt
+	Kursliste (Schüler-Kursart-Klasse-Lehrer).rpt
+	Medienvorgaenge (Standard).rpt
+	Schülerliste (mit Sorgeberechtigte französisch).rpt

## 6.0.125 639 (05.11.2013)

### Magellan
+ Korrigiert: Ansicht Schüler|Ausbildung: Neben dem Betrieb wird jetzt auch der Praxisbetrieb angezeigt.
+ Korrigiert: NRW: Ansicht Schüler|Bearbeiten|Export|Schüler Online exportieren: Beim Export werden jetzt Vorname und Nachname korrekt ausgegeben 
+ Korrigiert: die Suche (F3 oder Extras|Suche) zeigt nur gefundene Datensätze für den jeweiligen Mandanten an
+ Korrigiert: Ansicht Schüler/Bewerber|Bearbeiten|Export|Schüler Berlin exportieren: Beim Export der Schülerbemerkungen werden auch Semikolons, Anführungszeichen oder Kommas korrekt exportiert 

### Statistik:
+ Korrigiert: ALLE: Berechnung von Plausibilitäten mit Tools.IsEmpty werden 0 Werte korrekt berechnet  
+ Korrigiert: RLP.SchuelerNeuanlageABS: STALA-35810-2
+ Korrigiert: SHL: Oberstufendatensätze berechenen sich ab sofort klassenübergreifend kursbezogen
+ Korrigiert: SHL: Gastschüler werden für die EA-Datei nicht ausgespielt
+ Korrigiert: SHL: DATSA: Plausibilitäten Korrektur von Klasse.SCHHERK nach Schueler.SCHHERK 

### Skripte:
+ Korrigiert: (BER-FW-APO-2011.js) das 4.PF und 5.PK entsprechend Anlage 6a der Verordnung getauscht werden
+ Korrigiert: (BER-FW-APO-2011.js) die Belegungspflicht für Musik-Ensemble wird nicht mehr geprüft
+ Korrigiert: (BER-APO-2011.dws) das 4.PF und 5.PK kann entsprechend Anlage 6a der Verordnung getauscht werden

### Importe:
+ Aktualisiert: (ALLE)Die folgenden importierbaren Verzeichnisse wurden erneuert:
 00_Bezirke.keys
 00_Bundeslaender.keys
 00_Gemeinden.keys
 00_Kreise.keys
 00_Postleitzahlen.keys
 Um die Verzeichnisse in Ihrer Datenbank zu aktualisieren führen Sie bitte den Punkt Magellan-Administrator|Datenimporte|Postleitzahlverzeichnis importieren|Starten|Auswahl "Deutschland" oder "Berlin"|Alle Kataloge aus.
 WICHTIG: Anschließend führen Sie bitte Datenbankpflege|Datenbank überprüfen|Gemeinden synchronisieren aus.

### Berichte(neu oder geändert):
+ BER-GY-JZ (Schul Z 302)(12.07).rpt
+ Klassenliste Schüler-Notenmatrix (Querformat).rpt
+ Korrigiert: RLP-GY-Punktekreditkarte-2012.rpt


## 6.0.124 639 (22.10.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Geändert: Unter "Ansicht Abitur|Fachwahl" kann man über "Bearbeiten|Fachwahl exportieren" getrennt in das Schuldatentransferformat allgemein 
  (Menüpunkt "Schuldatentransferformat") und das Schuldatentransferformat speziell für Untis (Menüpunkt "Untis") exportieren.
+ Geändert: Unter "Extras|Export|Untis" erfolgt die Ausgabe in das Schuldatentransferformat in verbesserter Logik für Untis.
+ Geändert: Unter "Extras|Import|Untis" erfolgt der Import in des Schuldatentransferformats in verbesserter Logik für Untis.

### Statistik:
+ Korrigiert: ALLE: Berechnung von Plausibilitäten mit Tools.InRange wurden in wenigen Fällen falsch/positiv bewertet
+ Korrigiert: NRW: Berechnung des Statistikfeldes "Versetzung"
+ Korrigiert: NRW: Berechnung des Statistikfeldes "Schülerstatus" bei Abgängerdatensätzen, die an der gleichen Schule einen neuen Bildungsgang angefangen haben. 
+ Korrigiert: RLP.SchuelerNeuanlageABS: Berechnung zur Ausgabe der 2.Fremdsprache in RS+
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STUEBER-14
+ Korrigiert: RLP.SchuelerBewegungABS: Ausgeschulte Schüler mit FHR-Reife (Neuer Schlüssel 43) werden jetzt korrekt ausgespielt 

### Importe:
+ Neu:(Berlin) 
    00_SchulartenHerkunft
    00_SchulformenHerkunft
    00_SchulformenUebergang
    AS_BetreuungenAusserschulisch
    AS_BetreuungenInnerschulisch
+ Geändert:(Berlin)
    BS_Organisationen
    BS_Unterrichtsformen
    BS_Berufe
    BS_Berufsfelder
    BS_Faecher
    BS_Bildungsgaenge
    BS_Klassenstufen
    00_AbschluesseExtern
    00_SchuelerMerkmale
    00_Wiederholungsarten 
+ Neu: (NRW) die als csv-Datei importierbaren Schulverzeichnisse sind aktualisiert worden
    
### Skripte:
+ Korrigiert: (RLP-APO-BGY-2010) Fehler bei Gesamtpunktzahl behoben 
+ Korrigiert: (BER-FW-APO-2011.js) das 3. und 4. Prüfungsfach kann getauscht werden
+ Korrigiert: (BER-FW-APO-2011.js) für die Fachwahlkombinationen 57, 58 und 59 ist Sport als 2.Prüfungsfach zulässig
+ Korrigiert: (BER-APO-2011.dws) das 3. und 4. Prüfungsfach kann getauscht werden

### Magellan Administrator:
+ Korrigiert: Schnittstellenformat schueler_sorgebe.import.csv
+ Korrigiert: Löschen der Datenbank (Behoben durch Datenstrukturupdate)
+ Korrigiert: Problem beim Löschen des Logbuches behoben

### Berichte(neu oder geändert):
+ BER-Schul Z 306 (09.12).rpt
+ NRW-BK-ABI (Anlage D33a).rpt
+ Schülerliste (mit Praxisbetrieben und Geburtsdatum).rpt
+ Klassenliste Schüler-Notenmatrix (Querformat).rpt



## 6.0.123 638 (26.09.2013)

### Magellan
+ Neu: Seriendruckfelder Wahlvertreter 1 und 2 sowie Zusatz der Sorgeberechtigten für den Druck aus dem Menü Klassen
+ Korrigiert: Bearbeiten|Export|Schüler Berlin exportieren...: Schülerbemerkungen mit Umbrüchen 
+ Korrigiert: Sammelzuweisung der 4.FS
+ Korrigiert: Eintippen des Kürzels und navigieren per Pfeiltasten unter Schüler|Zeugnis|Details|Tutor
+ Korrigiert: Sorgeberechtigte|Daten|Zusatz
+ Neu: Schüler|Daten2 gibt es eine Checkbox für NdH
+ Neu: Unter Lehrer|Auswahl wird das Feld Diensttelefon mit eingeblendet

### Magellan-Administrator:
+ Geändert: Pfadhinweis beim Sichern der Datenbank
+ Korrigiert: Problem beim Importieren von Schülermerkmalen behoben

### Statistik:
+ Korrigiert: RLP.SchuelerNeuanlageABS: Plausibilität STALA-16260-2
+ Korrigiert: RLP.SchuelerBewegungABS:  Magellan unterbindet die teilweise fälschlich ausgegebene Plausibilität STALA 36250-1
+ Korrigiert: RLP.SchuelerBewegungABS:  Die Plausibilität STUEBER-12 wurde gelöscht, der Abschluss FH-Reife muss wieder mit dem Schlüssel 43 gesetzt werden
+ Korrigiert: RLP.LehrerNeuanlage:      Plausibilität STALA-5000, Gleitkommaberechnung korrigiert 
+ Korrigiert: RLP.LehrerNeuanlage:      Plausibilität STALA-5750, Gleitkommaberechnung korrigiert
+ Korrigiert: RLP.LehrerNeuanlage:      Plausibilität STALA-6400, leere SchulFormStufe berücksichtigt
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-24400-2, leere Fremdsprache berücksichtigt
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-27150, auf Schulform 810 umgestellt
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-27175, auf Schulform 810 umgestellt
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-38020, falscher Abschluss1 Schlüssel abgefragt
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-38080-2, Werteraum berücksichtigt
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-38700-1, Entlassungsschlüssel 46 nicht abgefragt
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-39600-1 entfernt, da veraltet  
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-39830-3, Plausibilitäten zusammengefasst und korrigiert
+ Korrigiert: RLP.SchuelerNeuanlageBBS: Plausibilität STALA-39830-4 / MORGEN-980, entfernt, da veraltet
+ Korrigiert: RLP.SchuelerNeuanlageBBS  Plausibilität STALA-25900
+ Korrigiert: RLP.SchuelerNeuanlageBBS  Plausibilität MORGEN-140
+ Korrigiert: RLP.SchuelerNeuanlageBBS  Plausibilität STALA-29415-12
+ Korrigiert: RLP.SchuelerNeuanlageBBS  Plausibilität STALA-24600
+ Korrigiert: RLP.SchuelerNeuanlageBBS  Plausibilität STALA-23710-1
+ Korrigiert: RLP.SchuelerNeuanlageBBS  Plausibilität STALA-23710-3
+ Korrigiert: RLP.SchuelerNeuanlageBBS  Plausibilität STALA-23710-4
+ Korrigiert: RLP.SchuelerNeunalageBBS  Ausbildungsberuf des Schülers wird nur für die Klassen.Schulform 810 ausgespielt.
+ Korrigiert: RLP.SchuelerNeuanlageBBS Solländerungsgründe
+ Korrigiert: RLP: Umgang mit Kommazahlen in Plausibilitäten
+ Korrigiert: SHL-Prüfdateien (SA,EA,FA,LE,OS)
+ Neu: Die Landesstatistik Nordrhein-Westfalen 2012/2013 wird mit dieser Ausgabe freigegeben.
+ Hinweis: NRW.Abi.txt: Bitte beachten Sie die überarbeitete Beschreibung im Landesstatistiken.pdf!
+ Neu: NRW.BBS: Bitte importieren Sie das neu hinzugekommene Schlüsselverzeichnis 00_Abschlussarten.keys. 
Setzen Sie für Schüler mit bestandenem Abitur den Wert unter Schueler|Laufbahn|Abschluss|Abschlussart. 
Ein Nicht-Bestehen muss nicht erfasst werden. Für die Zuweisung steht Ihnen eine Sammelzuweisung auf der Karte zur Verfügung.

### Importe:
+ Neu: (MVP BBS) aktualisierte Schlüsselimportdateien
+ Neu: (NRW BBS) 00_Abschlussarten.keys

### Skripte:
+ Korrigiert: (KFM-Profil-E 2012)CH-Promotion 
+ Korrigiert: (BER-APO-2011) Einbringung Sport und Sporttheorie, Prüfung für einen Sonderfall 2.Aufgabenfeld (3.PF GE + 5.PK GEO) 
+ Korrigiert: (BER-FW-APO-2011) §25.4  berücksichtigt
+ Korrigiert: (BER-FW-APO-2011)das 1. und 2.PF kann getauscht werden, wenn es sich um DE, FS(ab 9), MA oder NW handelt
+ Neu: (SAR-APO-2007.dws) um FHR aktualisiert
+ Neu: (BER-FW-APO-2011) Prüfung FS als Prüfungsfach, bitte markieren Sie die neu einsetzende Fremdsprache im Merkmal mit A
+ Neu: (BER-FW-APO-2011) Prüfung DS/IN als Prüfungsfach, bitte markieren Sie das Fach im Merkmal mit A, wenn es neu in der Oberstufe einsetzt

### Berichte(neu oder geändert):
+ SAC-FS-JZ (C.01.02).rpt
+ Sorgeberechtigte (nur Funktion1 und Funktion2).rpt
+ Medienliste (Inventur).rpt
+ Medienvorgaenge (Standard).rpt
+ Schülerliste (mit Vorbildung).rpt
+ Kursliste (Zensurerfassung).rpt
+ Sorgeberechtigte ohne Kinder im aktuellen Zeitraum.rpt



## 6.0.122 638 (29.08.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Neu: Unter Datenimporte|Postleitzahlen importieren können die Schlüsselverzeichnisse für Banken, Postleitzahlen, Gemeinden, Bezirke, Bundesländer, Kreise udn Stadtbezirke jetzt getrennt importiert werden. 
+ Neu: "Extras|Export|Untis bzw. Schuldatentranfersformat" bzw. "Extras|Import|Untis bzw. Schuldatentransferformat":
  Wenn Sie mit dem Recht "Administrator", "Statistk-Adminitrator" oder "Mandanten-Administrator" in 
  Magellan angemeldet sind, müssen Sie sich nicht nochmals beim Magellan-Datenaustausch-Assistenten anmelden.
+ Korrektur: "Ansicht Schüler|Zeugnis|Leistungen": Fehler beim Löschen der Einträge in den Feldern 
  "Durchschnitt 1".."Durchschnitt 3" behoben.
+ Neu: In der Ansicht "Berufschule"|Matrix können zusätzlich für die Spalten "J1 Note" bis "J9 Note" 
  der Wert "Status" festgehalten werden. Diese können beim Synchronisieren aus der 
  Ansicht "Schüler"|Zeugnis aus dem Feld "Status" übernommen werden.
+ Neu: Unter Ansicht "Schüler"/"Bewerber" kann auf der Registerkarte "Daten 4" das neue Feld "IBAN" genutzt werden.
  Durch die Änderung im Zahlungverkehr kann ab 2014 nur noch die IBAN anstelle der bisherige Kontonummer/Bankleitzahl verwendet werden.
+ Neu: Das Verzeichnis "Banken" wurde um die Felder "BIC", "Land" und "Prüfnummer" ergänzt. Um den für die Änderung im Zahlungverkehr 
  ab 2014 notwendigen BIC-Wert zu Ihre aktuellen Bankleitzahl verwenden zu können, müssen Sie die Bankleitzahlen nochmals 
  nach Magellan importieren. Wie Sie dazu vorgehen, entnehmen Sie bitte dem aktualisierten Magellan-Benutzerhandbuch unter
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan6.pdf im Abschnitt "3.3.1 Bankenverzeichnis importieren"    
+ Korrektur: Sicherheitsabfrage beim Löschen einer Zeile unter Verzeichnisse|Verordnungen per ENTF-Taste  
+ Korrektur: bei der Sammelzuweisung kann die 4.Fremdsprache korrekt zugewiesen oder geändert werden

### Magellan-Administrator:
+ Neu: Unter Datenimporte|Postleitzahlen importieren können die Schlüsselverzeichnisse für Banken, Postleitzahlen, Gemeinden, Bezirke, Bundesländer, Kreise udn Stadtbezirke jetzt getrennt importiert werden. 

### Statistik:
+ Neu: Die Landesstatistik Niedersachsen ABS 2013/2014 zum Export nach izn-stabil wird mit dieser Ausgabe freigegeben. Bitte 
  beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf
+ Neu: Die Landesstatistik Schleswig-Holstein 2013/2014 wird mit dieser Ausgabe freigegeben. Bitte 
  beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf
+ Korrektur: RLP ABS-Statistik)die Plausibilitäten STALA-35700-3 und STALA-36400-2 wurden ausgegeben, wenn die Abiturnote im Modul Abitur erfasst war

### Skripte: 
+ Korrektur: Importiere SDTF.dws (Übertrag des Lehrerunterrichtes aus daVinci bei Kursen ohne Kursnummer)

### Berichte (neu oder geändert)
+ CH-E-Profil (Kaufmann) 2012.rpt
+ Schülerausweis ABS.rpt
+ RLP-FO-FHReife (DIN A3).rpt
+ Klassenliste (inklusive Zusatzklasse).rpt
+ Schülerliste ( Klasse, Geburtsdaten, Adresse, Telefon).rpt



## 6.0.121 637 (16.08.2013)

### Magellan
+ Korrektur: Verzeichnisfelder in Sammelzuweisungen korrigiert

### Skripte:
+ Korrektur: Exportiere Fachwahl Schueler.dws, Importiere SDTF.dws und Exportiere SDTF.dws(Kursnummer im P1-Datensatz)
Mögliche Kursnummerwerte:
„0“= keine Kursnummer oder Kursnummer „0“
„1“ oder höher= entspricht der eingetragenen Kursnummer




## 6.0.120 637 (29.07.2013)

### Magellan
+ Neu: Unter Extras|Optionen|Einstellungen gibt es die neue Option "Abgleich Qualifikation/Fachwahl 
im Abitur". Bitte beachten Sie dazu die Beschreibungen im Handbuch in  den Abschnitten "Die 
Fachwahlüberprüfung" und "spezielle Einstellungen"
+ Neu: NRW-SchülerOnline: aus Magellan exportierte Schüler können von der abgebenden Schule nach 
SchülerOnline eingelesen werden. Aus Magellan exportierte Betriebe können für die aufnehmende Schule 
importiert werden. Bitte beachten Sie dazu das aktualisierte Dokument Landesanpassungen.pdf.



## 6.0.119 637 (26.07.2013)

Magellan-Administrator:
+ Korrektur: IBIS-Import: Problem beim Einlesen der schueler_laufbahn.import.csv behoben   

### Berichte (neu oder geändert)
+ BAW-BKO-FHReife (Einjähriges Berufskolleg).rpt
+ Anwesenheitsliste Lehrer (Monat).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt




## 6.0.118 637 (25.07.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan-Administrator:
+ Neu: In der Benutzerverwaltung können jetzt zwei neue Rechte eingestellt werden:
  * Berufsschule: Ist die Ansicht "Berufsschule" für den Benutzer editierbar
  * Berufsschule-Prüfungsnoten: Welche Spalten (Prüfungsnote, die Prüfungsnote (Kontrolle) oder beide)
    sind in Ansicht "Berufsschule" im Dialogfenster "Prüfungsnoten eingeben" sichtbar. Dieses Recht
    íst hauptsächlich für Anwender in der Schweiz gedacht. 
+ Korrektur: IBIS-Import: Problem beim Einlesen der schueler_laufbahn.import.csv behoben    

### Magellan
+ Korrektur: Fehler bei Seriendruck mit Word 2013 behoben.
+ Neu: die Seriendruckfelder Einschulmerkmal2 und Einschulmerkmal3 sind im Bewerber- und im Schülerseriendruck verfügbar
+ Korrektur: Anzeige von Umlauten im Willkommensfenster korrigiert
+ Neu: unter "Ansicht Berufsschule|Matrix" wurden die Spalten "Prüfungsnote (Kontrolle)" und "Fachnote" hinzugefügt.
+ Neu: Für die Schweiz kann man in der Ansicht "Berufsschule" über "Bearbeiten|Prüfungsnoten eingeben" im
  Dialogfenster "Prüfungsnoten eingeben" nach Auswahl eines Fachs und der Klasse, alle Schüler anzeigen lassen, 
  die das Fach in der Klasse in der Berufsschulmatrix besitzen. Je nach Rechteeinstellung in der Benutzerverwaltung
  kann jetzt nur die Prüfungsnote, die Prüfungsnote (Kontrolle) oder beide eingegeben werden.
+ Neu: Für die Schweiz kann man in der Ansicht "Schüler" über "Bearbeiten|Prüfungsnummern generieren" im Dialogfenster
  "Prüfungsnummern generieren" für Klassen automatisch Prüfungsnummern mit einer festzulegenden Syntax im Feld "Merkmal B1"
  der jeweiligen Schüler erzeugen.
+ Korrektur: RLP Statistik: Schülerneuanlage ABS: Datum beim Erkennen der Neuzugänge korrigiert
+ Korrektur: RLP Statistik: SchülerBewegung ABS: Korrektur beim Prüfen der Abiturnote  
+ Neu: Unter Schüler|Ausbildung|Editieren|Betrieb suchen kann per Option mit einem oder zwei Filtern nach Betrieben gesucht werden
  
### Haushalt&Inventar:
+ Änderung beim Anlegen und Löschen von Buchungen: 
  * Löschen von Buchungen nicht mehr möglich.
  * Anlegen und Stornieren von Buchungen auf die Schaltflächen + und -  
    aufgeteilt.
  * Dialogfenster für das Anlegen und Stornieren von Buchungen vereinheitlicht 
    und überarbeitet.
  * Beim Anlegen einer neuen Buchung können zusätzlich die Felder "Lieferant"
    und "Grund" angegeben werden.   
  * Wenn eine Buchung storniert wird, werden die Eckdaten bereits vorbesetzt, 
    es kann dann das Datum, der Betrag und der Grund für die Stornierung 
    angegeben werden.
  * Beim Anlegen von Buchungen zu denen keine oder zu wenige Haushaltsmittel 
    zur Verfügung stehen, wird ein Hinweis mit ausgegeben.
+ Neue Option "Restübernahme erlauben" hinzugefügt. Mit dieser Option kann die 
  Restübernahme beim Wechsel des Haushaltsjahres kontrolliert werden. Wenn die 
  Option ausgeschaltet ist, wird auch das Feld "Restübernahme" beim Haushaltstitel 
  ausgeblendet.                 

### Skripte:
+ Neu: CH-Promotion (KFM-Profil-E 2003).dws (Neues Promotionsskript für die Ansicht "Schüler"|Zeugnisse|Noten)
+ Ergänzung: CH-BBS-Matrix (KFM-Profil-E 2003 3-jährig).dws (Fachnoten werden in die neue Spalte "Fachnoten" übertragen)
+ Korrektur: BER-APO-2011.dws + BER-FW-APO-2011.js (diverse Korrekturen) 
+ Korrektur: Schüler wechseln.dws (Schulformeintritt wird beim Wechseln übernommen)
+ Korrektur: RLP-Statistik SchuelerNeuanlage BBS 2013.xml 
    STALA 26380
    STALA 26427
    STALA 27340
    STALA 29050-5
+ Korrektur: RLP-Statistik SchuelerBewegung ABS 2013.xml  
    STALA-35800-1
    STALA-35800-2
    STALA-36260-1...10

### Importe:
+ Änderung: Berliner Fachstatus erweitert  (Importe|Berlin|00_Fachstati.keys)
+ Änderung: Berliner Unterrichtsarten geändert (Importe|Berlin|00_Unterrichtsarten.keys)

### Berichte (neu oder geändert)
+ BAW-BKO-FHReife (Einjähriges Berufskolleg).rpt
+ SAC-BF-JZ (B.04.02).rpt
+ SAC-FS-AS mit FHR (C.01.12).rpt
+ SAC-BGJ-AS mit HS (A.01.09).rpt
+ RLP-FO-FHReife (DIN A3).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ Schülerliste (mit Betrieben).rpt
+ Anwesenheitsliste Lehrer (Monat).rpt
+ Lehrer (Personalhandkarte).rpt
+ Klassenliste (Adressen Schüler und Eltern).rpt
+ Zeugnisliste nach Schülerfächern (DIN A4 nur aktive Schueler und Fachkuerzel).rpt
+ CH-Notenausweis-E-Profil-2003.rpt

## 6.0.117 636 (29.06.2013)

Statistik:
+ Neu: Die Landesstatistik Rheinland-Pfalz 2013/2014 wird mit dieser Ausgabe freigegeben. Bitte 
  beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf

### Magellan
+ Dialogfenster "Schüler einschulen": Bei der Auswahl der Schüler werden zusätzlich die Spalten
  "Merkmal A1".."Merkmal A6", "Merkmal B1".."Merkmal B4" und "Bewerbungsziel 1".."Bewerbungsziel 4"
  als Auswahlkriterium angezeigt
+ Ansicht "Bewerber": Die Umbenennungen der Bezeichner "Merkmal D1".."Merkmal D4", "Merkmal U1" und
  "Merkmal U2" werden jetzt korrekt dargestellt. 
+ Schlüsselverzeichnis: Das Schlüsselverzeichnis "Bewerbungsempfehlungen" wurde zur leichteren 
  Auffindbarkeit in "Empfehlungen (Bewerbung)" umbenannt.

### Berichte (neu oder geändert)
+ RLP-GY-Punktekreditkarte-2012.rpt
+ RLP-FO-FHReife (DIN A3).rpt 
+ RLP-GY-FHReife (Jahrgangstufe 11-13).rpt 

## 6.0.116 636 (25.06.2013)

### Magellan
+ Berlin: In der Ansicht "Schüler" bzw. "Bewerber" wurden die Sammelzuweisung erweitert. In Abhängigkeit 
  von der eingestellten Maske können nun den Feldern der Masken Werte per Sammelzuweisung zugewiesen werden 
+ Statistik: SIP-Schnittstelle für Mecklenburg-Vorpommern veröffentlicht.Bitte beachten Sie 
  dazu das aktualisierte Dokument Statistik.pdf auf unserer Webseite
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf

### Magellan-Administrator:
+ Magellan Importformat: Verbesserte Hinweismeldungen beim Einlesen von Schülerlaufbahnen

### MyMagellan-Center:
+ Neu: Die Spalten "Letzter Export" bzw. "Letzter Import" wurden ersetzt durch die Spalten 
  "Letzter Export (Datum)"/"Letzter Export (Uhrzeit)" bzw. "Letzter Import (Datum)"/"Letzter Import (Uhrzeit)".
  Dadurch lassen sich die Informationen zum letzten Ex- bzw. Import besser sortieren bzw. gruppieren.
+ Korrektur: Spalte "Niveau" wird nun auch in der Fächeransicht nicht mehr angezeigt, wenn dies beim Export der mym.Dateien angegeben wurde
+ Korrektur: Kennwortänderung für MyMagellan funktioniert jetzt mit dem Benutzerrecht "Mandanten-Administrator"

### Haushalt&Inventar:
+ Korrektur: Beim Anlegen einer Buchung wird der Eintrag des Bereiches wieder korrekt berücksichtigt

### Skripte:
+ Korrektur: RLP-APO-2010.dws + RLP-FW-APO-2010.js (Berechnung für Fachhochschulreife korrigiert)
+ Korrektur: MVP-APO-2010.dws 
+ Korrektur: BER-APO-2011.dws + BER-FW-APO-2011.js (diverse Korrekturen)
+ Korrektur: SAR-APO-BGY-2007.dws (Korrektur der Durchschnittsnote)
+ Korrektur: Importiere SDTF.dws  (Übertrag des Lehrerunterrichts, Kurswahl: nur einem Kurs zugeordnete Fächer werden nach Magellan übernommen)
+ Korrektur: Exportiere SDTF.dws (Zuordnung von Schülern in Kurse ohne Kursnummer in daVinci)
+ Korrektur: Exportiere Fachwahl Schueler.dws (Kurszuordnung bei Kursen ohne Kursnummer der Schüler in daVinci)

### Magellan-Importkonverter:
+ Korrektur: Fehler beim Starten des Importkonverters behoben

### Berichte (neu oder geändert)
+ MVP-GY-ABI (2013).rpt
+ NRW-BS-AS (A01).rpt
+ SAC-BS-AS (A.02.05) 2spaltig.rpt
+ SAC-BS-AZ (A.02.04) 2spaltig.rpt
+ SHL-GY-AS (Klasse 5-10).rpt
+ SHL-GY-FHReife (2011).rpt
+ SHL-GY-HJZ (2008).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ RLP-GY-HJZ (11-13).rpt
+ RLP-GY-AS (11-13).rpt
+ Quittung(DIN A5).rpt
+ Schülerliste (mit Betrieben).rpt
+ Schülerliste (mit Betrieben und Geburtsdatum).rpt

## 6.0.115 635 (07.06.2013)

### Magellan
+ Neu: Unter der Ansicht "Abitur" ist die Sammelzuweisung auf der Registerkarte "Prüfung" erweitern bzw. auf der Registerkarte
  "Fachwahl" neu eingefügt worden. Dort können jetzt
  a) auf der Registerkarte "Fachwahl" nachträglich Zeiträume für die Halbjahre zugewiesen werde
  b) auf der Registerkarte "Fachwahl" die Markierungen der Spalten E1,E2,Q1,Q3 auf die Spalten Q1,Q2,Q3,Q4 verschoben werden
+ Korrektur: bei der Neuanlage von Schülern/ Bewerber mit Hilfe der Enter-Taste wird der Eingabecursor nun richtig im Feld "Anrede" gesetzt.
+ Korrektur: Für Berlin werden beim Export der Schüler/Bewerber (Ansicht Schüler/Bewerber|Bearbeiten|Export|
  Schüler/Bewerber Berlin exportieren)) die Informationen zum Berlinpass jetzt korrekt exportiert 
+ Neu: für Berlin wird in der Maske Bewerber|SekII das Feld Konfession angezeigt

### Haushalt&Inventar:
+ Korrektur: Beim Anlegen einer Buchung ist der Eintrag des Bereiches nicht mehr notwendig

### MyMagellan-Center:
+ Korrektur: Beim Assistenten zum Verteilen der MyMagellan-Dateien wird jetzt korrekt der aufgrund des 
  Rechnerdatums aktuelle Zeitraum automatisch markiert.

### MyMagellan 
+ Korrektur: Fehltage werden in der MyMagellan Datei ausgeblendet, wenn dies im MyMagellan angegeben wurde

### Magellan-Administrator:
+ Korrektur beim Zuweisen des Benutzerrechtes "Mandanten-Administrator"

### Skripte:
+ Neu: MVP-APO-2010.dws (Berechnungskript für diesjähriges Abitur)
+ Korrektur: NRW-APO-BK-2012.dws (Berechnung für Abiturdurchschnitt 1,2 korrigiert)
+ Korrektur: SHL-APO-2010.dws (Berechnung der Summe in Block II korrigiert)
+ Korrektur: SAC-APO-BGY-2011.dws (Berechnung Gesamtsumme und Durchschnitt  korrigiert)
+ Korrektur: BER-FW-APO-2011.js und BER-APO-2011.dws (diverse Korrekturen)

### Berichte (neu oder geändert)
+ RLP-GY-HJZ (11-13).rpt
+ RLP-GY-AS (11-13).rpt
+ RLP-GY-Punktekreditkarte-2012.rpt
+ RLP-GY-AZ (2006).rpt
+ SHL-GY-ABI (2011).rpt
+ Lehrer (Personalhandkarte).rpt
+ Quittung (Ausleihe).rpt
+ Etiketten (No.3651 - 52,5 x 29,7 mm - 1fach - 9 x 4 Zeilen).rpt
+ Etiketten (No.3651 - 52,5 x 29,7 mm - 2fach - 8 x 4 Zeilen).rpt
+ Etiketten (No.3651 - 52,5 x 29,7 mm - 2fach).rpt
+ Etiketten (No.3651 - 52,5 x 29,7 mm - 1fach).rpt
+ Bibliotheksausweis (Avery-Zweckfom-Etikett 3658).rpt
+ Schülerpersonalblatt incl. Schuleintritt (Betriebe).rpt

## 6.0.114 635 (31.05.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: In der Ansicht "Mandanten" ist in der Auswahlliste und auf der Registerkarte "Daten 1" 
  das zusätzliche "Rechtsstatus" verfügbar.
+ Neu: In der Ansicht "Mandanten" können in der Auswahlliste jetzt auch die Spalten ein- und 
  ausgeblendet werden über "Bearbeiten|Spalten bearbeiten".
+ Neu: In den Ansichten "Schüler" bzw. "Bewerber" können nun neben dem Nachnamen und Vornamen auch 
  der 2. Vorname und Zusatz zum Nachnamen gespeichert werden. 
+ Neu: In den Ansicht "Sorgeberechtigte" kann nun neben dem Nachnamen und Vornamen auch 
  der Zusatz zum Nachnamen gespeichert werden.
+ Neu: Für Berlin werden beim Export der Schüler,der Bewerber und der jeweiligen Sorgeberechtigten (Ansicht Schüler/Bewerber|Bearbeiten|Export|
  Schüler/Bewerber Berlin exportieren) 
  a) die neuen Felder "Vorname2" und "Namenszusatz" in der Datei 
     "schueler.export.csv"  und  "bewerber.export.csv"
  b) das neue Feld "Namenszusatz" für den Sorgeberechtigten in der Datei 
     "schueler.sorgebe_export.csv" mit exportiert. 
  Vergleichen Sie dazu auch das aktualisierte Dokument  "Landesanpassungen.pdf" auf unseren 
  Internetseiten.
+ Korrektur: In der "Ansicht Abitur|Fachwahl" werden beim Einfügen von Fächern nur noch die Spalten
  der maximal 6 Halbjahr automatisch markiert, die auch sichtbar sind.  

### MyMagellan-Center:

WICHTIG: die mit dieser MyMagellan-Center-Version erstellen mym-Dateien müssen mit der parallel 
erscheinenden MyMagellan-Version (## 6.0.10) bearbeitet werden.
+ Neu: Beim Exportieren in MyMagellan-Dateien können die Felder "Leistungsanforderungen" und "Versetzungsart" 
  optional mit übernommen werden.
+ Neu: Beim Exportieren in MyMagellan-Dateien können Sie festlegen, ob die Felder "Fehltage" und "Fehltage
  unentschuldigt" sichtbar und editierbar sein sollen.
+ Neu: Beim Assistenten zum Verteilen der MyMagellan-Datei ist der aufgrund des Rechnerdatums der aktuelle 
  Zeitraum automatisch markiert.

### Magellan-Bibliothek & Lernmittel

+ Korrektur: Export aus der Liste der Medien nach Excel berücksichtigt nur die ausgewählten Datensätze
+ Neu: Medien|Exemplare können auch nach Excel exportiert werden
+ Korrektur: das Handbuch kann über Hilfe|Benutzerhandbuch aufgerufen werden

### Magellan-Haushalt & Inventar

+ Neu: Über "Verzeichnisse|Bezeichnungen anpassen" können die Begriffe "Haushaltsstelle",
  "Haushaltsstellen" und "Haushaltstitel" individuell angepasst werden. 
             
### Magellan-Administrator:

+ Änderung: Die Rechtegruppe "Statistikadmin" wurde in "Statistik-Administrator" umbenannt
+ Neu: die Rechtegruppen wurden erweitert um "Kollegium 5". Kollegium 5 entspricht Kollegium 2, 
zusätzlich dürfen die Oberstufendaten im Menü Abitur aller Schüler editiert werden.
+ Neu: folgende Zusatzoptionen können in der Benutzerverwaltung pro Benutzer gewählt werden:
  
  Mandanten-Administrator: 
  Wird dieser Haken aktiviert, werden die Rechte des Benutzers auf vollständige Schreib- und 
  Leserechte innerhalb der Schulverwaltung erhöht. Zusätzlich kann das MyMagellan-Center bedient werden.
  
  Import/Export: 
  Dem Benutzer können sämtliche Import/Exportpunkte in Magellan gewährt werden. Dazu gehört 
  "Extras|Import", "Extras|Import", "Bearbeiten|Export" der Export nach Excel, Word(Seriendruck)
  oder HTML in allen Menüpunkten.
  
  Drucken: 
  Dem Benutzer kann das Drucken von Berichten, Zeugnissen, Kurslisten oder Zeugnisformularen 
  gestattet werden.
  
  Dokumente:
  Dem Benutzer kann der Zugriff auf die Dokumentenverzeichnisse (Schüler/Bewerber, Lehrer, Mandant, 
  Klassen...) gestattet werden.
  
  Diese Optionen können auch über den Benutzerimport/-export in der Benutzerverwaltung angepasst 
  werden. Bitte lesen Sie dazu die angepasste Dokumentation im Magellan-Benutzerhandbuch.pdf.
  
### Magellan-Importformat Konverter

+ IBIS-Import: Der Import der Betriebe kann jetzt wahlweise auch echte 
  Betriebekürzel konvertieren, wenn in IBIS das Feld "BETRIEKURZ" vorhanden ist
  (IBISEKEY.DBF und/oder FIRMEN.DBF) 

### Skripte

+ Neu: das Skript RLP-APO-2012.dws ist verfügbar!
+ Neu: das Skript RLP-APO-BGY-2012.dws ist verfügbar!
+ Korrektur: Das Abiturberechnungsskript BER-APO-2011.dws wurde angepasst:
    In der Ansicht "Abitur|Qualifikation" wird der Wert im Feld "GesamtPkt LK" jetzt korrekt berechnet
    In der Ansicht "Abitur|Prüfung" wurde die Ausgabe der Durchschnittsnote korrigiert
+ Korrektur: BER-FW-APO-2011.js (Fächer des 2.AF wurden mit dem Fachstatus PRS nicht korrekt markiert)

### Berichte (neu oder geändert)

+ Haushaltsstellen (Buchungen).rpt
+ RLP-GY-HJZ 11-1.rpt
+ RLP-GY-HJZ 11-2.rpt
+ BAW-Anmeldebogen 5 Klasse.rpt
+ SHL-ABI-Meldung-MdlAbitur (Profil 2011).rpt
+ SHL-GY-Abi (Leistungskarte 2011).rpt
+ SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
+ SAC-BS-AS (A.02.05).rpt
+ SAC-BS-AZ (A.02.04).rpt
+ SAC-FS-AS mit FHR (C.01.12).rpt
+ SAC-FS-JZ (C.01.02).rpt
+ SAC-FO-FHReife (D.01.05).rpt
+ SAC-FS-AZ (C.01.04).rpt
+ SAC-BF-AS (B.01.03).rpt
+ SAC-BS-AS (A.02.05) 2spaltig.rpt
+ SAC-FS-AS mit FHR (C.01.13).rpt
+ Zeugnisliste nach Schülerfächern (DIN A4 nur aktive Schueler und Fachkuerzel).rpt
+ Bewerber (Aufnahmebescheinigung an abgebende Schule - Fax).rpt
+ Bewerber (Aufnahmebescheinigung an abgebende Schule - Brief).rpt
+ MVP-GY-ÜZ (2013).rpt
+ MVP-GY-ABI (2013).rpt
+ NRW-BK-ABI (Anlage D41 - 2012).rpt
+ NRW-Abitur (Prüfungsergebnisse 2).rpt
+ NRW-Abitur (Prüfungsergebnisse 1).rpt
+ NRW-ABI-AZ  (Anlage D42).rpt
+ NRW-BK-AZ (Anlage D 31).rpt
+ BER-GY (abi_4_berechnungsbogen)(09.12).rpt
+ BER-GY-ABI (Schul Z 306)(09.12).rpt

## 6.0.113 635 (02.05.2013)

### Magellan

+ Erweiterung: Beim Fortschreiben von Schülern werden jetzt auch die Angaben zur Zusatzklasse 
  (Ansicht Schüler|zeugnis|Fächer|Spalte "Zusatzklasse") mit fortgeschrieben. 
+ Neu: Ansicht "Berufsschule": Bei Synchronisieren der Schüler werden jetzt auch die Fehlstunden,
  Fehlstunden unentschuldigt, Fehltage und Fehltage unentschuldigt übertragen. Zusätzlich kann 
  optional angegeben werden, ob der Wert Durchschnitt 1, Durchschnitt 2 bzw. Durchschnitt 3 aus
  "Ansicht Schüler|Zeugnis|Leistungen" auf die passenden Durchschnitte 1-9 abgebildet werden.  
+ Korrektur: Für Berlin wurde das Fachwahlskripte BER-FW-APO-BBS-2011.js aktualisiert
+ Korrektur: Bewerber|Bewerbungsstatus wurde wieder um den Status "Rückmeldung" ergänzt

### Importformat-Konverter

+ Geändert: Alle Konvertierungen berücksichtigen in den entsprechenden Importformatfeldern mit dem 
            Datentyp M für Memofeld die Konvertierung der Zeilenumbrüche in die neue Notation "\n" 
            (ohne Anführungszeichen)  

### Administrator

+ Korrektur: betriebe.import.csv: 
Der Import des Feldes "Kurzel" wurde auf die Datenbankgröße von 20 Zeichen korrigiert.
+ Korrektur: schueler.import.csv: Der Import des Feldes "BewerberStatus" erlaubt jetzt die Angabe der zwei Zeichenwerte.   
+ Geändert: schueler.import.csv: Der Import des Feldes "BewerberStatus" wurde um den neuen Wert 
"AG = Abgemeldet" erweitert.  
+ Geändert: Magellan-Importformat: Bei allen einzulesenden Feldern mit dem Datentyp M für Memofeld(meistens Bemerkungsfelder) entfällt die Größenbeschränkung von 255 Zeichen.                                                 
+ Geändert: Magellan-Importformat: Alle einzulesende Feldern mit dem Datentyp M für Memofeld(meistens Bemerkungsfelder) können mit der besonderen Notation"\n" (ohne Anführungsstriche) mit Zeilenumbrüchen im Text versehen werden.
+ Geändert: Änderungungen im Importformat Importdokument dokumentiert (Dokumentation siehe Magellan-Import.pdf)
            
### Berichte (neu oder geändert)

Bewerber (Aufnahmebescheinigung an abgebende Schule - Fax).rpt
Bewerber (Aufnahmebescheinigung an abgebende Schule - Brief).rpt
MVP-GY-ÜZ (2013).rpt
NRW-BK-ABI (Anlage D41 - 2012).rpt
NRW-Abitur (Prüfungsergebnisse 2).rpt
NRW-Abitur (Prüfungsergebnisse 1).rpt
BER-GY (abi_4_berechnungsbogen)(09.12).rpt
BER-GY-ABI (Schul Z 306)(09.12).rpt
NRW-ABI-AZ  (Anlage D42).rpt
BER-BFS-HJZ (Schul Z 520b)(07.09).rpt

## 6.0.112 635 (17.04.2013)

### Magellan

+ Korrektur: Fehler beim Aufruf der Ansicht "Bewerber" behoben.

### Skripte:
+ Korrektur: Das Abiturberechnungsskript BER-APO-2011.dws wurde angepasst. In der Ansicht
  "Abitur|Qualifikation" wird der Wert im Feld "GesamtPkt LK" jetzt korrekt berechnet. 




## 6.0.111 635 (16.04.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan
+ Änderung: Vorschau für Berichte/Zeugnisse ist von 75% auf standardmäßig 100% erhöht worden.
+ Neu: Unter Verzeichnisse|Zeiträume gibt es einen Assistenten zum Anlegen von Zeiträumen
+ Neu: Neues Feld "Sprache" unter Ansicht "Schüler|Zeugnis|Fächer" zum Kennzeichnen bilingual 
  unterrichteter Fächer
+ Neu: Neues Feld "Sprache" in Dialogfenster "Notenübersicht" unter "Ansicht Schüler|Zeugnis|Leistungen"
  zum Kennzeichnen bilingual unterrichteter Fächer
+ Neu: Neue Felder "Q1 Sprache" ... "Q4 Sprache" unter "Ansicht Abitur|Qualifikation" und 
  "Ansicht Abitur|Fachwahl" für die Angabe der Sprache des bilingualen Unterrichts.
+ Neu: Neues Feld "Lehrer" unter "Ansicht Abitur|Qualifikation". Dieses Feld wird auch bei der 
  Synchronisation ins Abitur mit berückschtigt. Dabei wird dieses Feld in der "Ansicht Abitur|Qualifikation"
  jeweils mit dem Wert aus dem letzten Zeitraum unter "Ansicht Schüler|Zeugnis|Fächer|Spalte Lehrer"
  belegt.
+ Neu: Neues Schlüsselverzeichnis "Kurssprachen" für die erwähnten Felder "Sprache" bzw. 
  "Q1 Sprache"..."Q4 Sprache"
+ Neu: Für Berlin werden in der "Ansicht Abitur|Qualifikation" zusätzlich die Felder "Belegte Kurse",
  "Gesamtpunktahl", "Gesamtpunktahl GK" und ""Gesamtpunktahl LK" angezeigt.
+ Korrektur: Unter "Ansicht Schüler|Zeugnis|Details" werden die Wortersetzungen für die Begriffe 
  "Fehlstunden", "Fehlstunden unentschuldigt", "Fehltage" und "Fehltage unentschuligt" jetzt korrekt
  angezeigt.
+ Neu: Unter "Ansicht Abitur|Auswahl" wird jetzt auch der Tutor des Schülern mit angezeigt
+ Neu: Unter "Extras|Optionen|Einstellungen" kann man jetzt unter "Niveau editierbar" einstellen, ob 
  die Spalte "Niveau" unter "Ansicht Schüler|Zeugnis|Noten" editierbar ist. 
+ Neu: Unter "Ansicht Schüler|Zeugnis|Details" gibt es das neue Feld "Leistungsanforderungen"
+ Neu: Für Berlin wird die Abiturschnittstelle 2013 mit dieser Ausgabe freigegeben. Bitte beachten Sie 
  dazu das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
  https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf

### Magellan-Konverter:
+ Korrektur: Konvertierung der IBIS-Daten funktioniert jetzt fehlerfrei, auch wenn erwartete IBIS-Dateien nicht zur Verfügung stehen.

### Skripte:
+ Korrektur: Für Berlin wurden die Fachwahlskripte BER-FW-APO-BBS-2011.js und BER-FW-APO-BBS-2011.js aktualisiert. 
Ebenso wurde das Abiturberechnungsskript BER-APO-2011.dws angepasst. 

### Berichte (neu oder geändert)
NRW-BK-JZ (Anlage C14 - 2 Seitig).rpt
NRW-BK-JZ (Anlage C14 - 1 Seitig).rpt
NRW-BK-ABI (Anlage D34).rpt
NRW-BK-ABI (Anlage D33a).rpt
NRW-BF-FHReife (Anlage C17 schulischer Teil).rpt
NRW-Abitur (Prüfungsergebnisse 1).rpt



## 6.0.110 634 (09.04.2013)

 
### Magellan
+ Neu: Unter "Ansicht Abitur|Bearbeiten|Fachwahlen exportieren" können die Fachwahlen direkt in eine 
  Schuldatentransferdatei exportiert werden 
+ Neu: Unter "Ansicht Klassen|Daten 1" kann im Feld "Klassenart" der neue Wert 
  "Standard mit Oberstufensynchronisation" angeben werden. Schüler mit Klassen mit dieser neuen 
  Klassenart stehen dann in der Ansicht "Abitur" ebensfalls für die Synchronisation zur Verfügung.
+ Beim Import einer Schuldatentransferdatei (Extras|Import|Schuldatentransferdatei bzw. 
  Extras|Import|Untis) können der Übernahme der Schülerkurswahlen zusätzliche Optionen ausgewählt werden.
  Ein genaue Beschreibung der zusätzlichen Optionen entnehmen Sie bitte dem aktualisierten
  Benutzerhandbuch von Magellan im Abschnitt "23. Stundenplandaten".
+ Beim Export einer Schuldatentransferdatei (Extras|Export|Schuldatentransferdatei bzw. 
  Extras|Export|Untis) werden für Schüler zusätzlich die Felder "Geschlecht", "Geburtsdatum" und "Email"
  und für Lehrer die Felder "Mobil" und "Email" exportiert.
  Ein genaue Beschreibung der zusätzlichen Optionen entnehmen Sie bitte dem aktualisierten
  Benutzerhandbuch von Magellan im Abschnitt "23. Stundenplandaten".
+ Das Schuldatentransferformat hat sich geändert. Beachten Sie dazu das 
  aktualisierte Dokument "Schuldatentransferformat.pdf" auf unseren Internetseiten.
+ Neu: Bei der Übernahme der Fachwahlen in der "Ansicht Abitur|Fachwahlen" gibt es die neue Option 
  "und Fachstatus beibehalten". Mit dieser Optionen werden bei der Markierung "Vorhandene Fächer
  nicht löschen" und der Markierung "und Fachstatus beibehalten" vorhandene Fächer aktualisieren ohne
  jedoch den bereits eingetragenen Wert im Feld "Fachstatus" zu verändern.
  
### Berichte (neu oder geändert)
NRW-BK-JZ (Anlage C14 - 2 Seitig).rpt
NRW-BK-JZ (Anlage C14 - 1 Seitig).rpt
NRW-BK-ABI (Anlage D34).rpt
NRW-BK-ABI (Anlage D33a).rpt
NRW-BF-FHReife (Anlage C17 schulischer Teil).rpt
NRW-Abitur (Prüfungsergebnisse 1).rpt
SAR-GEMS-AZ (Klasse 5-8)(Vollschulzeitpflicht nicht erfüllt).rpt
SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
MVP-GY-ABI (2010).rpt
NRW-BK-ABI (Anlage D33b).rpt
BER-GY (abi_4_berechnungsbogen)(09.12).rpt





## 6.0.109 634 (27.03.2013)

 
### Magellan
+ Neu: Unter "Ansicht Berufsschule|Matrix" gibt es auf der rechten Seite ein zusätzliches Feld 
  "Durchschnitt"
+ Geändert: Berliner Export für Schüler/Bewerber (mit Herkunftsschulen, Ausbildungsdaten, 
  Sorgeberechtige) wurde erweitert und überarbeitet. Beachten Sie dazu auch das aktualisiert Dokument 
  "Landesanpassungen.pdf" auf unseren Internetseiten unter "Dokumente".

### MyMagellan-Center:
WICHTIG: die mit dieser MyMagellan-Center-Version erstellen mym-Dateien müssen mit der parallel 
erscheinenden MyMagellan-Version (## 6.0.9) bearbeitet werden.
+ Neu: Beim Exportieren in MyMagellan-Dateien kann das Feld "Personalnummer" optional mit 
  übernommen werden.
+ Neu: Beim Exportieren in MyMagellan-Dateien können Sie festlegen, ob das Felder "Personalnummer",
  editierbar sein soll.

### Skripte:
+ Korrektur: Schweiz - Das Skript "CH-BBS-Matrix (KFM-Profil-E 3-jährig).dws" wurde umbenannt in 
  "CH-BBS-Matrix (KFM-Profil-E 2003 3-jährig).dws"   
+ Neu: Schweiz - Für das E-Profil Reglement 2012 gibt ein neues Skript 
  "CH-BBS-Matrix (KFM-Profil-E 2012 3-jährig).dws" für die Ansicht "Berufschule" und 
  zusätzlich ein Promotionsskript "CH-Promotion (KFM-Profil-E 2012).dws"  für die 
  Ansicht Schüler|Zeugnis|Leistungen

### Berichte (neu oder geändert)
Notenübersicht Endnoten.rpt
Notenübersicht Endnoten unterschiedlich.rpt
CH-Notenausweis-E-Profil-2003.rpt
RLP-GY-ABI (DIN A4 - 2. Seite)2006.rpt
BER-GY (abi_4_berechnungsbogen)(09.12).rpt
BER-FOS-MSA (Schul Z 512).rpt
Schülerliste (mit Prüfungsfächern inkl. Lehrer).rpt




## 6.0.108 634 (21.03.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].
 
### Magellan
+ Korrektur: Problem beim Anlegen eines Mandanten behoben
+ Neu: beim Erkennen einer Doublette im Bewerbermenü und Neuanlegen wird die SchülerID des Schülers 
als IDIntern des Bewerbers gespeichert
+ Korrektur: Bewerber anlegen|Doublettenprüfung|Schüler als Bewerber kopieren: Problem beim Anlegen 
der Sorgeberechtigten behoben
+ Korrektur: Zuweisen des Prüfungsvorsitzenden per Zeugnis|Details|Sammelzuweisung korrigiert
+ Korrektur: Länge der Seriendruckfeldes Email für Bewerber-/Schülersorgeberechtigten wurde angepasst
+ Korrektur: Länge der Seriendruckfeldes Email für Sorgeberechtigte wurde angepasst
+ Neu: Unter Verzeichnisse|"Bezeichnungen anpassen" können folgende Feldbezeichnungen in der Ansicht 
Schüler geändert werden:
- Zeugnis|Details|Fehlstunden
- Zeugnis|Details|Fehlstunden davon unentschuldigt
- Zeugnis|Details|Fehltage
- Zeugnis|Details|Fehltage davon unentschuldigt
- Daten3|Personalnummmer
+ Geändert: Für Nordrhein-Westfalen wurde der Import aus SchülerOnline überarbeitet:
- Fehlerkorrekturen und funktionale Ergänzungen 
- Import erfolgt über Bewerber bearbeiten statt Schüler bearbeiten
- Bitte beachten Sie dazu auch die überarbeitete Beschreibung im Landesanpassungen.pdf

### Skripte:
+ Korrektur: BER-APO-2011 Korrektur 5. Prüfungskomponente
+ Neu: NRW-APO-BK-2012 
+ Korrektur: NRW-APO-BK-2011 Pflichteinbringung Deutsch, Fremdsprache und Geschichte korrigiert

### Administrator:
+ Neu: schueler.import.csv - Erweitert um die Möglichkeit bereits bestehende Schüler als Bewerber zu 
importieren. Es wird die "ID" des Schülers als "IDIntern" beim Bewerber gemerkt. (Status: SB)   
+ Korrektur: Import exemplare.import.csv 
- Inventarnr
+ Korrektur: schueler.import.csv 
- FremdsprachenStatus, Bildungskarte, BildungskarteBis
+ Korrektur: schueler_laufbahn.import.csv 
  - Fehlstunden, FehlstundenU, Fehlbeschreibung in der Dokumentation, Felder sind Pflicht
  - TutorKuerzel
+ Korrektur: schueler_fachdaten.import.csv 
- Unterrichtsart 
- Prüfung auf bestehenden Fachdaten-Datensatz wird um das Feld "Unterrichtsart" erweitert. Somit ist
ein Mehrfachimport von Fachdaten mit gleichem Fach möglich, wenn sich die Unterrichtsart 
unterscheidet.

### Berichte (neu oder geändert)

SAC-FS-AS mit FHR (C.01.13).rpt
NRW-BK-AZ (Anlage D35).rpt
NRW-BK-ABI (Anlage D33a).rpt
NRW-BG-HJZ VZ Jahrgangsstufe 11 (Anlage D32).rpt
NRW-BK-ABI (Anlage D33b).rpt
Schülerpersonalblatt incl. Schuleintritt (Betriebe -Querformat).rpt
NRW-BK-ABI (Anlage D33b).rpt
RLP-GY-ABI (DIN A4 - 2. Seite)2006.rpt




## 6.0.107 633 (04.03.2013)

### Magellan
+ Neu: Für Nordrhein-Westfalen kann in der Ansicht "Schüler" unter "Bearbeiten|Import|Schüler-Online
importieren" die Exportdatei aus Schüler-Online importiert werden. Nähere Information hierzu 
entnehmen Sie bitte dem aktualisierte Dokument "Landesanpassungen.pdf" im Abschnitt "Schüler-Online 
für Nordrhein-Westfalen".  
+ Neu: In der Ansicht "Schüler" werden in der Auswahlliste zusätzlich die Felder "Bewerbungsziel 1".
"Bewerbungsziel 4" und der Bewerbungsstatus ausgewiesen, die zuvor in der Ansicht "Bewerber" 
eingetragen worden sind.
+ Neu: In der Ansicht "Bewerber" kann man im Bewerbungstatus zusätzlich den Status "Abgemeldet" 
eintragen
+ Korrektur: Auf der Register "Ansicht Schüler|Zeugnis|Details" sind in der Sammelzuweisung die 
Felder "Tutor" und "Prüfungsvorsitzender" wieder funktionsfähig.
+ Korrektur: In "Ansicht Mandanten|Daten 1" kann man jetzt das Feld "Schulstatus" korrekt füllen. 

### Bibliothek:
+ Neu: Schüler, die als Ausleiher in die Bibliothek übernommen wurden, werden wie in Magellan mit 
Zeitraumbezug angezeigt 

### Berichte (neu oder geändert)
NRW-Bescheinigung (Nichtzulassung Abitur D37).rpt
SAC-BF-AS (B.01.03).rpt
BER-BF-AS (Z 522-542).rpt




## 6.0.106 633 (25.02.2013)

### Administrator

+ Korrektur: Fehler beim Import von Postleitzahlen und Schlüsseln behoben

## 6.0.105 633 (20.02.2013)

### Magellan

+ Neu: Für Berlin kann aus der Ansicht Schüler bzw. Bewerber über 
  "Bearbeiten|Export|Export Schüler Berlin" bzw. "Bearbeiten|Export|Export Bewerber Berlin"
  ein Export der Berliner Masken ins CSV-Format vorgenommen werden. Beachten Sie dazu auch das
  aktualisiert Dokument "Landesanpassungen.pdf" auf unseren Internetseiten unter "Dokumente".

### Administrator

+ Neu: angelegte Benutzer können aktiv oder inaktiv gesetzt werden

### Haushalt&Inventar

+ Korrektur: Rundungsproblem in der Anzeige der Haushaltstitel und Haushaltsstellen behoben
+ Neu: Anzeige des Betrags bei Buchungen als zweistelliges Währungsformat eingestellt

### Berichte (neu oder geändert)

RLP-RSPLUS (HJZ-AS-AZ und 5.-10. Klasse).rpt
BER-BS-AS (Schul Z 501).rpt

## 6.0.104 633 (12.02.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Änderung: Neue Bewerberstatus auch im Bewerberverfahren ergänzt
+ Neu: Neue Bewerberstatus in Berliner Masken verfügbar
+ Korrektur: In der Ansicht "Personen" kann der Status der Person wieder über 
  "Bearbeiten|Status zuweisen" geändert werden
+ Neu: Auf der Registerkarte "Ansicht Schüler|Zeugnis|Leistungen" kann bei Markierung der Option
"Durchschnitt einblenden" kann auf der rechten Seite über das neue Zauberstab-Symbol eine 
Sammelzuweisung der Prüfungsverordnung für mehrere Schüler gleichzeitig durchgeführt werden.
+ Korrektur: Schuljahreswechselassistent zeigt Statistikkürzel der Klassen korrekt an
+ Korrektur: Fehler beim Schuljahreswechsel-Assistent in der Ansicht "Klassen" behoben. 
+ Korrektur: Schüler|Zeugnis|Fächer: Spalte Mahnung kann über "Layout anpassen" ein- und 
ausgeblendet werden
+ Korrektur: Feldlänge angepasst LehrerEmail/Seriendruckfeld LehrerEmail
+ Korrektur: Berlin|Bewerber|SekI|Profilfächer: Note kann wieder entfernt werden
+ Korrektur: Verzeichnisse in den Schüler-/Bewerbersammelzuweisungen auswählbar
 
### Administrator

+ Änderung: Hinweis auf ein 8-stelliges Passwort beim Benutzeranlegen
+ Änderung: Reihenfolge der Eingabe eines Benutzers angepasst 
+ Neu: Vorbereitung der Datenstruktur für mit der nächsten Version erscheinenden Möglichkeit, 
zwischen aktiven und inaktiven Benutzern unterscheiden zu können
+ Korrigiert: beim Import der Medien.Import.csv: Status und Mehrjahresband 
+ Korrigiert: Import von leeren Werten am Zeilenende
+ Neu: in der Datei Schueler_Laufbahn.Import.csv gibt es neue Felder: ZeugniskonferenzAm, 
ZeugnisausgabeAm

### Skripte

+ Korrektur: Zuweisen von Fachtafeln.dws - Feld "Merkmal" wird jetzt wieder mit
  übernommen

### Vorlagen

+ Änderung: Bewerberserienbriefvorlagen als Word 97-2003-Vorlage (*.dot) abgespeichert

### Berichte (neu oder geändert)
Schüler (Zeitraumübergreifende Notenübersicht).rpt
Schüler (Zeitraumübergreifende Notenübersicht).rpt
SAC-FS-HJZ (C.01.03).rpt
SAC-FS-JZ (C.01.02).rpt
SAC-FS-HJI (C.01.01).rpt
SAC-BF-HJI (B.04.01).rpt
Bewerberliste mit Summendaten.rpt
Klassenlehrerliste mit Räumen.rpt
SAC-FS-JZ2 (C.01.02).rpt
SAR-AZ-Verhaltenszeugnis.rpt
SAR-AS-Verhaltenszeugnis.rpt
SAR-GEMS-AZ (Klasse 5-8)(Vollschulzeitpflicht nicht erfüllt).rpt
SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
SAC-BS-Bescheinigung  über erreichten Leistungen.rpt

## 6.0.103 632 (09.01.2013)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Unter "Extras|Schüler rückversetzen" können Sie Schüler in einen zeitlich gesehen davor 
stattfindendn Zeit versetzen, was einem "Rückversetzen" entspricht. Dieser Sonderfall ist teilweise 
beim Datenimporten nach Magellan notwendig.

### Magellan-Administrator

+ Neu: Unter Ansicht "Benutzerverwaltung"|Benutzerliste|Hinzufügen bzw. Editieren kann im 
Dialogfenster "Benutzer editieren" auf der Registerkarte "MyMagellan" ein pro Benutzer 
individuelles MyMagellan-Kennwort festgelegt werden. Dieses wird dann im MyMagellan-Center beim 
Verteilen der MyMygallan-Datein verwendet, um diese MyMagellan-Datein mit einem Kennwort zu 
versehen.
+ Neu: Unter Ansicht "Benutzerverwaltung"|Benutzerliste|Hinzufügen bzw. Editieren kann im 
Dialogfenster "Benutzer editieren" auf der Registerkarte "Allgemein" über das neue 
Optionsfeld "Kennwort als MyMagellan-Kennwort übernehmen" festgelegt werden, ob das Kennwort für
Magellan auch als MyMagellan-Kennwort übernommen werden soll. 
+ Neu: für Import von Schulen wurde die Feldlänge für die Schulnummer auf 12 Zeichen erweitert 

### MyMagellan-Center

+ Neu: Beim Exportieren in MyMagellan-Dateien können die Feld "Niveau" und "Mahnung" optional mit 
übernommen werden.
+ Neu: Beim Exportieren in MyMagellan-Dateien können Sie festlegen, ob die Felder "Fachstatus",
"Unterrichtsart", "Niveau" bzw. "Mahnung" editierbar sein sollen.
+ Neu: Beim Exportieren in MyMagellan-Dateien können Sie festlegen, ob die Felder "Abschluss1", 
"Abschlussart1", "Abschlussdatum1", "Abschlussnote1", "Abschluss2", "Abschlussart2", 
"Abschlussdatum2", "Abschlussnote2", "Versetzt", "Zeugniskonferenz am" und "Zeugnisdatum" sichtbar 
und editierbar sein sollen.
+ Neu: Beim Expotieren in MyMagllean werden jetzt die in der Magellan-Benutzerverwaltung individuell 
festlegbaren MyMagellan-Kennwörter aus dem Magellan-Administrator verwendet. Diese 
MyMagellan-Kennwörter können auch im MyMagellan-Center nachträglich editiert werden. 

## 6.0.102 631 (17.12.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan 

+ Neu: In der Ansicht "Bewerber" können auf der Registerkarte "Daten 3" bis zu 6 Wahlfächer
  festgehalten werden.
+ Neu: In der Ansicht "Berufschule"|Matrix können zusätzlich für die Spalten "J1 Note" bis "J9 Note" 
  die Werte "Durchschnitt", "Fehltage", "Fehltage unentschuldigt", "Fehlstunden" und 
  "Fehlstunden unentschuldigt" festgehalten. Diese können beim Synchronisieren aus der 
  Ansicht "Schüler"|Zeugnis aus den Feldern "Durchschnitt 1", "Fehltage", "Fehltage unentschuldigt", 
  "Fehlstunden" und "Fehlstunden unentschuldigt" übernommen werden.  
+ Neu: Im Verzeichnis "Fächer": In der Spalte "Kategorie" können die zusätzlichen Kategorien 
"Gesundheit" und   "Psychologie" erfasst werden.
+ Erweiterung: In den Ansichten "Mandanten" und "Schulen" können im Feld "Schulnummer" jetzt bis zu 
12 Zeichen statt  der bisherigen 8 Zeichen gespeichert werden. 

### Skripte

+ Korrektur: Zuweisen von Fachtafeln.dws - Berücksichtigt das Feld "Hauptfach"
+ Neu: Synchronisiere BBS.dws - Berücksichtigt jetzt die Felder "Durchschnitt 1", 
  "Fehltage", "Fehltage unentschuldigt", "Fehlstunden", "Fehlstunden unentschuldigt" 
 
### Weitere Fachwahlskripte:

RLP-FW-APO-BGY-2010.js  
RLP-FW-APO-2010.js  
BER-FW-APO-2011.js
BER-FW-APO-BBS-2011.js
NIE-FW-APO-2010.js
SHL-FW-APO-2010.js 
Bitte beachten Sie die Dokumentation pro Skript im Dokument Landesanpassung.pdf
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesanpassungen.pdf

### Berichte (neu oder geändert)
SAC-BS-AZ (A.02.04).rpt
SHL-HS-AS.rpt
SHL-RS-AS.rpt
NRW-BK-AZ (Anlage D35).rpt
BER-GY-JZ (Schul Z 251)(07.10).rpt
CH-E-Profil (Kaufmann).rpt

## 6.0.101 630 (07.12.2012)

### Magellan
+ Korrektur: Anzeige des geänderten Feldes Bewerber|Zugang|Einschulung (Werteliste statt 
Optionshaken) für Berliner Masken geändert 

### Skripte

+ Neu: Fachwahlskript für RLP (RLP-FW-APO-2010.js)
+ Korrektur: Benutzerrechte zuweisen.dws
+ Korrektur:Synchronisiere Zugriffsrechte.dws

## 6.0.100 630 (06.12.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Schüler|Zugang/Abgang|Vorzeitige Einschulung wurde ersetzt durch Einschulung. 
  Anstatt eines Ja/Nein Feldes kann nun zwischen Vorzeitiger, Fristgerechter und 
  Verspäteter Einschulung ausgewählt werden. Vorherige Eingaben wurden übernommen.
+ Neu: Die Schlüsselverzeichnisse "Berufe" und "Bildungsgänge" wurden um das Feld "Kategorie",
  mit den Ausprägungen "Intern", "Extern", "Intern und Extern" erweitert , auch 
  die Importe wurden um dieses Feld erweitert. Damit lassen sich die Schlüssel 
  zwischen Intern und Extern erworbenen Daten trennen. Beispiel: Mitgebrachte  
  Berufe werden nur noch beim Schüler|Daten 3|Berufe angezeigt, "Interne" und 
  "Interne und Externe" (in der eigenen Schule erworbene) werden hingegen in den 
  anderen Felder bei der Klasse und beim Schüler angezeigt.
+ Neu: zusätzliche Werte unter Bewerber|Daten1|Status:
    Beratungstest
    Beratungsgespräch
    Nicht zum Gespräch/Test erschienen
    Aufnahmebescheid
    Zusage nicht zurück
+ Korrektur: Löschen von Mandanten|Logo2 korrigiert
+ Neu: für den Seriendruck aus dem Schülermenü gibt es das Feld Betriebe-E-Mail
+ Neu: Umbenennung: Unter Magellan|Extras gibt es statt Schuldatentransferformat|Import/Export und 
Untis Import/Export die Menüpunkte Import|Schuldatentransferformat/Untis und 
Export|Schuldatentransferformat/Untis
+ Neu: Neuer Aufruf unter Hilfe für Benutzerhandbücher (Landesstatistik, Landesanpassungen)

### Magellan-Administrator

+ Korrektur: Einlesen von Schlüsselverzeichnissen. Wenn mehrere Schlüsseldateien 
  für ein Schlüsselverzeichnis existierten, wurde beim zweiten Durchlauf die 
  neuen Schlüssel wieder gelöscht. 
+ Korrektur: Einlesen der Datei Import.Exemplare.csv geändert
+ Korrektur: MagellanImportformat-Konverter für IBIS-Übernahmen überarbeitet

### Magellan-Bibliothek

+ Neu: Medien|Exemplare|Sammelzuweisung: Korrektur der Funktion "Sammelzuweisung", 
  Problem beim Zuweisen von Standorten behoben

### Skripte

+ geändert: SHL-Statistik DATSA 2012.xml
+ Neu: NRW-AS-APO-1999(Berechnung der Abschlüsse für Berufskollegs), bitte beachten Sie dazu das 
akualisierte Dokument Landesanpassungen
+ geändert: Importiere SDTF.dws  (von daV->Mag: Lehrerunterricht, Schülerfachwahlen)

### Berichte (neu oder geändert)

Quittung(DIN A5).rpt
NRW-BG-HJZ VZ Jahrgangsstufe 11 (Anlage D32).rpt
NRW-BK-AZ (Anlage D30).rpt
SHL-GEMS-LE.rpt
SAR-GEMS-AZ (Klasse 5-8)(Vollschulzeitpflicht nicht erfüllt).rpt
SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
NRW-BK-AZ (E01-0A).rpt
BER-GY-JZ (Schul Z 251)(07.10).rpt
BER-BV-AS (Schul Z 508).rpt
BER-GY-AZ (Schul Z 252)(01.07).rpt
BER-GY-JZ (Schul Z 250)(05.08).rpt
NRW-BK-AZ (Anlage D35).rpt
SAR-AZ-Verhaltenszeugnis.rpt
Schülerpersonalblatt (mit Vorbildung und Herkunftsschule).rpt

## 6.0.99 629 (16.11.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Dokumente

+ Magellan-Benutzerhandbuch: das Handbuch enthält künftig nur noch die für alle Bundesländer 
gültigen Informationen. Bundeslandspezifische Informationen finden Sie im Dokument 
Landesanpassungen.pdf. In die Landesanpassung wurde aus dem Magellan-Benutzerhandbuch folgende Kapitel 
verschoben:
+ Kapitel „Bewerber- und Schülermasken für Berlin“: Dieses Kapitel beschreibt die speziell für die 
Berliner Schulen entwickelten Bewerber- und Schülermasken für die verschiedenen Schulstufe.
+ Kapitel „Klassenmaske für Berlin“: Dieses Kapitel beschreibt die speziell für die Berliner Schulen
angepasste Klassenmaske.
+ Kapitel „Mandantenmaske für Berlin“: Dieses Kapitel beschreibt die speziell für die Berliner 
Schulen angepasste der Mandantenmaske.
+ Kapitel „Schülergruppen für Rheinland-Pfalz“: Dieses Kapitel beschreibt die speziell für Schulen 
in Rheinland-Pfalz entwickelte Erfassung schülerbezogener Unterrichtseinheiten bzw. Lerngruppen.

### Magellan-Benutzerhandbuch

https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan6.pdf 

### Landesanpassungen

https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesanpassungen.pdf

### Magellan

+ geändert: Die Auswahl des Ausbildungsbetriebes beim Schüler/Bewerber wurde überarbeitet. Das
Dialogfenster ermöglicht jetzt neue Suche und Filteroptionen.
+ Neu: Auf der Registerkarte "Ansicht "Schüler" bzw. "Bewerber"|Merkmale" sind nun vier neue
Datumsfelder D1...D4 verfügbar
+ Neu: Auf der Registerkarte "Ansicht "Schüler" bzw. "Bewerber"|Statistik" sind nun zwei neue 
Datumsfelder U1 und U2 verfügbar
+ Neu: In der Ansicht "Mandanten" kann auf der Registerkarte "Daten 2" ein 2. Logo gespeichert 
werden.
+ geändert: Schueler|Zeugnis|Arbeits- und Sozialverhalten|Ergänzungen
+ korrigiert: Schüler|Zeugnis|Arbeits- und Sozialverhalten|Ergänzung
+ geändert: Eingabegeschwindigkeit für Schüler|Zeugnis|Arbeits- und Sozialverhalten|Bewertung 
optimiert
+ geändert: Zeilenwechsel per Enter unter Schüler|Zeugnis|Arbeits- und Sozialverhalten|Bewertung
 
### Magellan-Klassenbuch

+ geändert: Das Programm MagellanKlassenbuchSync.exe zum Übertrag der daVinci-Stundenplandatei in 
das Magellan-Klassenbuch kann aus Sicherheitsgründen nur noch über die Magellan-Administrator-
Kennung aufgerufen werden.
 
### Magellan-Bibliothek

+ geändert:  Ausleihe|Sammelaktion|Lehrersatz ausleihen
 
### Magellan-Administrator

+ geändert: Datenbankpflege|Datenbank überprüfen|Generatoren synchronisieren
+ geändert: Verbesserte IBIS-Konvertierung und Import (Dokumentation siehe Magellan-Import.pdf)
 
### Skripte

+ geändert: "Schueler einschulen.dws": Wird ein Schüler als Bewerber kopiert, die Doublette (Kopie 
des Schülers) aus dem Bewerbermenü übernommen,im gleichen Zeitraum eingeschult und versucht mit dem 
ursprünglichen Schüler zusammenzuführen, erscheint diese Meldung: "Schüler "Ihr Schüler" kann nicht 
mit Schüler mit ID=1111 zusammengeführt werden und wird eingeschult...OK". Die Schüler bleiben als 
zwei Datensätze getrennt erhalten und sind unterschiedlichen Klassen zugeordnet.
+ geändert: "BER-BBS-Matrix-2007.dws": Im Rahmen der Abschlussberechung wird nicht mehr der 
Abschluss in das Feld "Abschluss2" unter Ansicht "Schüler"/Laufbahn/Abschluss automatisch gefüllt.

### Statistik

+ geändert:SHL Plausibilitäten für Lehrerdatei (L411/461, L511/521, L531, L541, 561, L811/821, L831) 

### Berichte (neu oder geändert)

SAR-GEMS-HJZ-JZ (Klasse 5-8).rpt
SAR-GEMS-AZ (Klasse 5-8)(Vollschulzeitpflicht nicht erfüllt).rpt
BER-BQL VZ-HJZ (Schul Z 505 a).rpt
BER-BQL TZ-HJZ (Schul Z 505 c).rpt
BER-BS-HJZ (Schul Z 500).rpt
BER-BS-AZ (Schul Z 503).rpt
BER-BS-AS (Schul Z 501).rpt
BER-FOS-HJZ (Schul Z 510)(05.06).rpt
BER-FOS-AZ (Schul Z 513)(05.06).rpt
SAC-BG-AZ (E.01.05).rpt
SAC-BG-ABI (E.01.06).rpt
RLP-FO (HJZ-JZ-AZ).rpt
NRW-BBS-JZ-HJ-AG-AS (A05-A06).rpt
NRW-BBS-JZ-HJ-AG-AS (A07).rpt
NRW-BS-AS (A01).rpt
NRW-BK-ABI (Anlage D41).rpt
NRW-BBS-AG-AS-JZ-HZ (A01-A04).rpt
BAW-KMK-Fremdsprachenzertifikat (2012).rpt
Klassenliste (Adressen Schüler und Eltern).rpt
Schülerliste (mit Betrieben).rpt
Schülerliste (mit Betrieben und Geburtsdatum).rpt
Schüler-Abschlussbericht(Schulabgänger).rpt

## 6.0.98 628 (17.10.2012)

### Statistik

+ geändert SHL-ABS: SHL-Statistik DATLE.xml: L511/L521, L531, L811/L821
+ geändert SHL-ABS: Export der SAE(Schulartempfehlung) für Datei EA angepasst
+ geändert SHL-ABS: Meldung EA22 für dreistellige Schlüssel angepasst
+ geändert RLP-ABS: Schüler-BBS-Neuanlage|Klassenergänzungen|gekoppelt.mit => mehrfach vorkommende 
Klassen werden nicht mehr gesondert aufgeführt

### Magellan-Administrator

+ Neu: IBIS-Konvertierung und Import (Dokumentation siehe Magellan-Import.pdf)Administrator: 
+ Neu: Beim Einlesen der Schlüsseldatei BS_Berufe.keys kann für die Spalten Berufsfeld und 
Fachrichtung auf Werte der Verzeichnisse Berufsfeld und Fachrichtungen verwiesen werden. Verwiesen 
wird auf die Kürzel der beiden Schlüsselverzeichnisse. 
+ geändert SHL: unter Datenbankpflege|Daten überprüfen|Empfehlungen umkopieren wird das 
Gültig-bis-Datum frei gelassen

### keys-Dateien

+ Neu: Berliner Berufeverzeichnis wurde um die Fachrichtung und das Berufsfeld erweitert.

### SDTF

+ erweitert: U1-Datensatz 

### Berichte (neu oder geändert)

NRW-BS-AS (A01).rpt
SAC-BS-AS (A.02.04).rpt
RLP-GY-Punktekreditkarte-2012.rpt
NRW-BK-ABI (Anlage D41).rpt

## 6.0.97 628 (28.09.2012)

### Statistik

+ geändert SHL: SHL-Statistik DATSA 2012.xml: SA30
+ geändert SHL: SHL-Statistik DATEA 2012.xml: EA93
+ neu SHL: zusätliche Prüfungen für SA/EA: SCHHERK, HWS,SAE, JERST, ENTL
+ neu SHL: SA82,EA43,SB40,SB42-1-9, SB62,SB67
+ geändert SHL: SHL-Statistik DATLE.xml
+ geändert NRW: SIM.TXT

### Magellan

+ korrigiert: Die Auswahlliste des Feldes "An Schule" bleibt gefüllt,auch wenn zuvor Schüler|bereits
besuchte Schulen|Schule genutzt wurde 

### Importe

+ Neu: Berlin: 
  * 00_Lehraemter.keys
  * 00_Uebergangsarten.keys
  * 00_Wiederholungsarten.keys
  * BS_Klassenstufen.keys
+ Neu: NRW: BS_AbschluesseExtern.keys  
 
### Berichte (neu oder geändert)
Schüler-Abschlussbericht(Schulabgänger).rpt

## 6.0.96 628 (20.09.2012)

### Magellan-Importformat Konverter

+ geändert: Korrigieren der Klassenzeiträume bei fehlenden Austrittsdaten 
  optimiert. Es kommen jetzt mehr Zeiträume heraus.

### Magellan-Administrator

+ Magellan-Importformat: 
  - geändert: Das Importieren der Noten wird anhand der Notenart differenziert

### Statistik

+ geändert: SHL|AS_SchulformenHerkunft= Schlüssel 01 wurde entfernt
+ geändert: SHL|Plausibilität SA77 
+ geändert: NRW-SIM.TXT:
  * Aufnahmedatum bei Abgängern
  * LSFachklasse
  * LSGliederung
 Weitere Informationen finden Sie in unserem Landesstatistiken.pdf:
 https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf
 
### Berichte (neu oder geändert)

Klassenliste (Zensurenstatistik nach Punkten).rpt
Klassenliste (Zensurenstatistik nach Noten).rpt
      
## 6.0.95 628 (18.09.2012)

### Magellan

+ geändert: Bewerbervorlagen übernehmen Merkmalsfelder
+ Korrigiert: Berliner Masken|Berufsbildung: Rechteproblem beim Wiederholerhaken behoben
+ geändert: Lehrer|Daten2|Dienstbez. Gültigkeitsraute ergänzt 
+ geändert: Angaben unter Schüler|Ausbildung erweitert 

### Statistik

+ NRW: Ausspielen der Vorjahresdaten des Schülers korrigiert.
+ SHL: Für die EA-Datei werden anhand des Grundschuleintritts die Schulbesuchs-
  jahre berechnet. Inaktive Schüler, die die Schulbesuchszeit nicht  erfüllt 
  haben, werden nicht in die EA-Datei übertragen.
+ SHL: Erhebungsdatum geändert
+ SHL: Plausbilitätskorrekturen des Statistikamtes für EB-Datei übernommen.

### Import

+ Geändert:  SchulenBER_2012_09_17.csv (Vorlage für Import der Berliner Schulen)

### Skripte

+ geändert: RLP-Statistik SchuelerBewegung ABS 2012.xml:
  * entfallen sind: STALA-35600, STALA-36300-2, STALA-36300-3
  * neu: STALA-36300

### Berichte (neu oder geändert)

Klassenliste (Zensurenstatistik nach Punkten).rpt
Klassenliste (Zensurenstatistik nach Noten).rpt
Unfallanzeige (in word ausfüllbar).rpt
BER (Kurswahl).rpt
RLP-GY-Punktekreditkarte-2012.rpt
BBS-Schulbescheinigung.rpt
Bescheinigung über den Schulbesuch zweifach.rpt
Klassenliste (inklusive Zusatzklasse).rpt

## 6.0.94 628 (05.09.2012)

### Magellan

+ Neu: Die Landesstatistik Nordrhein-Westfalen 2012/2013 wird mit dieser Ausgabe freigegeben. Bitte 
beachten Sie das aktualisierte Dokument Landesstatistiken.pdf auf unserer Webseite:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf
+ Änderung: Import|Berlin|BS_Berufe.keys
+ Änderung: unter Schueler|Ausbildung wird der Name2 des Ausbildungsbetriebes angezeigt

### Magellan-Administrator

+ Magellan-Importformat: 
  * Anzeige des Schülers bei Importfehlern der Schüler-Laufbahn
  * Unterbinden des Importversuches, wenn Schüler-Laufbahn aufgrund der 
    Datenprüfung nicht importiert werden kann.
  * Schueler.Iport.csv:Anhand des Vornamens, Nachnamens und Geburtsdatums als bereits vorhanden 
    erkannte Schüler werden mit aufgelistet

### Magellan-Bibliothek

+ Direktes Hinzufügen von Lieferanten beim Anlegen neuer Exemplare ermöglicht
+ Bei der Klassensatzausleihe sind die Medien statt der Exemplare auswählbar  

### Magellan-Importformat Konverter

+ Konvertieren von IBIS Zeiträumen: Schüler ohne AustrittX Datum erhalten 
  automatisch zuvor berechnete Austrittsdatdatum der Klasse
+ Wenn in der IBISEKEY das Feld "ART" zur Ermittlung des "Verhältnis" bei 
  Schüler-Sorgeberechtigten nicht eingetragen ist, dann werden automatisch 
  folgende Werte berechnet: 
    Schüler < 18 Jahre = EB = Erziehungsberechtigte
    Schüler > 18 Jahre = AP = Ansprechpartner    
    
### Skripte

+ Korrigiert: Importiere SDTF.dws (Übertrag von Lehrern von daVinci nach Magellan)
+ Korrigiert: Prüfskripte für RLP-ABS
+ Korrigiert: Prüfskripte für SHL-ABS 

### Berichte (neu oder geändert)

Klassenliste (inklusive Zusatzklasse).rpt
SAC-BF-AS (B.03.05).rpt
SAC-BF-JZ (B.04.02).rpt
BER(Kurswahl.rpt
   
## 6.0.93 628 (22.08.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Beim Kopieren von Schülern als Bewerbern wird die "Interne ID" des Schülers bei der Kopie 
gespeichert. Damit ist es möglich zum Beispiel einen Schüler auch als Bewerber im Datenbestand zu 
führen und auch beide Datensätze ggfs. wieder zusammenzuführen. Zusätzlich kann die Funktion auch 
für das Überbrücken von Zeiträumen genutzt werden, beispielsweise wenn ein ehemaliger Schüler später
an Ihre Schule zurückkehrt.
+ Neu: Schüler, in deren Schülerfachdaten einem Fach eine "Zusatzklasse" zugewiesen wurde, können 
optional auch bei dieser Klasse unter Klassen|Zeitraum|Schüler eingeblendet werden.

Bitte beachten Sie für beide vorstehenden Neuerungen auch das neue Kapitel "Sonderfälle in der 
Schülerlaufbahn". Sie können das Handbuch aus Magellan unter Hilfe|Benutzerhandbuch aufrufen oder 
unter dem folgenden Link herunterladen:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan6.pdf
+ Korrektur: (nur mit Bundeslandauswahl Berlin) Auswahl des Tutors für die Maske SekII korrigiert 
+ Korrektur: Fachtafel kopieren/Fachtafel extrahieren
+ Korrektur: RLP: Plausibilität STALA-18510-1 geändert
+ Neu: Unter Abitur|Fachwahl kann die Fachkombinationsnummer mit ausgegeben und in die Schülerdaten 
übernommen werden
+ Neu: Abitur|Fachwahl: ausgeblendete Halbjahre werden nicht mehr mit markiert
+ Korrektur: (nur mit Bundeslandauswahl Berlin) Schüler als Bewerber kopieren
+ Korrektur: (nur mit Bundeslandauswahl Berlin) Funktionen des Bewerberverfahrens 

### Administrator

+ Neu: Berlin: Neue oder geänderte Schlüssel-Importdateien
+ Neu: SHL: Die Funktion "Kopiere Empfehlung" legt noch nicht im Verzeichnis enthaltene 
Schlüssel automatisch mit an
+ Korrektur am Magellan-Importformat Konverter:
  * Konvertieren von IBIS Zeiträumen
  * Extrahieren von Schlüsselwerten, wenn ein Gleichheitszeichen vorhanden  
+ Korrektur am Magellan-Importformat: 
  * Anzeige im Dialogfenster
  * Prüfung des Schülers führte auch zum Importversuch der Schülerdaten   

Bitte beachten Sie auch das aktualisierte Magellan-Import.pdf:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan-Import.pdf

### Bibliothek

+ Bestandsstatus pro Exemplar hinzugefügt
+ Standort pro Exepmlar hinzugefügt
+ Sammelzuweisung der Exemplare um neue Felder erweitert
+ Korrekturen und Verbesserungen an der Kurssatz-Ausleihe
+ Funktionalität "Hilfe|Systeminfo" bekannt aus Magellan, jetzt auch in Bibliothek
+ Anzeige der Versioninformation zur Anzeige in Magellan angepasst. 
 
### Berichte neu oder geändert

- SAC-BF-AS (B.03.05).rpt

## 6.0.92 628 (17.08.2012)

+ interner Test

## 6.0.91 627 (01.08.2012)

### Magellan

+ Fehler beim Datenabgleich Magellan-daVinci bei Übertrag der Fachtafeln behoben
+ NEU: Unter "Ansicht Klassen|Zeiträume|Schüler" können nun optional auch die Schüler mit 
angezeigt werden, die die angezeigte Klasse als "Zusatzklasse" unter  
"Ansicht Schüler|Zeugnis|Fächer" eingetragen haben.
+ Schüler einschulen: Fehler bei der Anzeige des Profils behoben
+ Ansicht Schüler|Zeugnis|Fächer: Fehler bei Sammellöschung bei der Anzeige des Profils behoben
+ Fehler beim Kopieren von Fachtafeln behoben
+ Fehler bei der Landesstatistik Schleswig-Holstein behoben. Bitte 
beachten Sie auch das aktualisierte Dokument Landesstatistiken.pdf auf unserer Webseite:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf

### Berichte neu oder geändert

- Klassenliste (Sorgeberechtigte Mobil und Geburtsdatum).rpt

## 6.0.90 627 (28.07.2012)

### Magellan

+ Fehler beim Aufruf der Statistik für Schleswig-Holstein behoben
+ Ansicht Schüler/Bewerber: Fehler bei Sammelzuweisung behoben: Profil wird jetzt korrekt angezeigt.
+ Ansicht Schüler|Zeugnis|Arbeits- und Sozialverhalten: Diverse Fehler behoben.  

### Magellan-Administrator

+ Fehler im Schlüsselverzeichnis "Berufe" für Berlin behoben

## 6.0.89 627 (20.07.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Die Landesstatistik Schleswig-Holstein 2012/2013 wird mit dieser Ausgabe freigegeben. Bitte 
beachten Sie das aktualisierte Dokument Landesstatistiken.pdf auf unserer Webseite:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf
+ Neu: "Ansicht Schüler|Zugang/Abgang" / "Ansicht Bewerber|Zugang": Neues Feld "Empfehlung" für die 
Zugangsempfehlung

### Magellan-Bibliothek

+ Neu: Ansicht "Bücher/Medien"|Daten 1: Neues Feld "Status" für den Bestandsstatus eines Exemplars.

## 6.0.88 626 (18.07.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Einlesen des Gemeindekennzifferverzeichnis inkl. Verbandsgemeinden Rheinland-Pfalz 
+ Neu: Postleitzahl- und Gemeindekennzifferverzeichnis für die Schweiz
+ Neu: Unter Ansicht "Abitur" gibt es eine neue Registerkarte "Fachwahl" zur Erfassung der Fachwahlen.
der Schüler. Dies ermöglicht auch die Fachwahlüberpüfung gemäß der Fachwahlverordnung. 
Beachten Sie dazu auch das aktualisierte Magellan-Benutzerhandbuch.
Folgende Fachwahlverordnungen stehen mit dieser Version zur Verfügung.
  - BER-FW-APO-2011 (Berlin)
  - NIE-FW-APO-2010 (Niedersachsen)
  - SHL-FW-APO-2010 (Schleswig-Holstein)          

### Berichte neu oder geändert

BER (Kurswahl).rpt
SAC-BF-AS (B.01.03).rpt
SAC-BGJ-AS mit HS (A.01.10).rpt
SAC-BF-JZ (B.04.02).rpt
SAC-FS-JZ (C.01.02).rpt
SAC-FS-AS (C.01.11).rpt
SAC-BVJ-AS mit HS (A.01.08).rpt
SAC-BS-JZ (A.02.01).rpt
SAC-BVJ-AS mit HS (A.01.08).rpt
SAC-FO-FHReife (D.01.05).rpt
SAC-FO-AZ (D.01.04).rpt
SAC-FO-JZ (D.01.02).rpt

## 6.0.87 624 (12.07.2012)

+ interner Test (Installation unter Windows 2000)

## 6.0.86 624 (09.07.2012)

### Magellan
+ Korrektur: die Einstellung unter Extras|Optionen|Dokumente|Dateinamenkonventionen werden 
gespeichert

### Magellan-Administrator

+ Neu: IBIS-Konvertierung und Import (Dokumentation siehe Magellan-Import.pdf)
+ Neu: Magellan-Importformat überarbeitet und erweitert(Dokumentation siehe Magellan-Import.pdf)
Download: https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan-Import.pdf
+ Neu: NRW-Schulverzeichnis erweitert, einlesbar über Magellan-Importformat|Schulen

## 6.0.85 624 (06.07.2012)

+ interner Test

## 6.0.84 624 (28.06.2012)

### Statistik

+ Neu: Die Landesstatistik Rheinland-Pfalz 2012/2013 wird mit dieser Ausgabe freigegeben. Bitte 
beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf

### Magellan

+ Neu: Unter Stueber S.|Magellan 6|Importe|Nordrhein-Westfalen steht zwei dem Magellan-Importformat 
entsprechende Schulenlisten zur Verfügung
   - Schulverzeichnis NRW (mit Grundschulen).csv
   - Schulverzeichnis NRW (ohne Grundschulen).csv  
+ Korrektur: Eintrag aus Schüler|Daten3|Profil wird im Assistenten der Fachtafelzuweisung angezeigt
+ Neu: Seriendruckfeld "Bemerkungen" ergänzt für Personen, Lehrer, Schüler und Bewerber 
+ Neu: Seriendruckfelder im Bewerbermenü erweitert um:
  Grundschuleintritt, Profil, Konfession, RelTeilnahme, RelWunsch, Staatsangehoerigkeit1, 
  Staatsangehoerigkeit2, Muttersprache, Verkehrssprache, Sprachgruppe, Personalnr, Bemerkung, 
  MerkmalA1, MerkmalA2, MerkmalA3, MerkmalA4, MerkmalA5, MerkmalA6, MerkmalS1, MerkmalS2, MerkmalS3,
  MerkmalS4, MerkmalS5, MerkmalS6, MerkmalS7, MerkmalS8, MerkmalS9, MerkmalS10, MerkmalB1, 
  MerkmalB2, MerkmalB3, MerkmalB4, MerkmalT1, MerkmalT2, MerkmalT3, MerkmalT4  
+ Neu: Schüler|Laufbahn|Abschluss|Abschlussnote mögliche Werte erhöht
+ Neu: Im Assistent zum Fachtafelzuweisen steht die Spalte "Bildungsgang" zur Verfügung
+ Korrektur: Anzeige der Bestandteile für die Lizenz Praktikumsbetriebe

### Skripte

+ Korrektur: BAW-APO-BGY-2010-G9
+ Korrektur: SAR-APO-BGY-2007
+ Korrektur: SHL-APO-2010
+ Korrektur: SAC-APO-BGY-2011
+ Korrektur: NRW-APO-BK-2011
+ Korrektur: BAW-APO-2010-G9

### Berichte neu oder geändert

SAC-FO-FHReife (D.01.05).rpt
BER-KO-ABI (Schul Z 324)(02.11).rpt
SHL-HS-AS.rpt
SHL-RS-AS.rpt
BER-BOS-FHReife (Schul Z 532)(06.05).rpt
RLP-GY-JZ (2spaltig und mit Wahl- oder Pflichtfächern Variante 2).rpt

## 6.0.83 624 (13.06.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Ansicht "Schüler"/"Bewerber": Auf der Registerkarte "Zugang/Abgang" ist beim Schulbesuch bei 
der Auswahl der Schule die Anzeige erweitert worden. Neben der Anzeige der Schulform und Schulnummer 
kann die Ansicht jetzt auch gruppiert werden.
+ Neu: Das Verzeichnis "Bildungsgänge" ist um das Feld "Bezeichnung 2" erweitert worden. Zudem 
können jetzt bei den Feldern "Bezeichung" bzw. "Bezeichnung2" 240 statt bisher 100 Zeichen 
abgespeichert werden. 
+ Neu: Über "Extras|SMS Protokoll" kann jetzt ein Protokoll der versendten SMS aufgerufen werden 
+ Neu: Beim Seriendruck über Microsoft Word werden bei der Auswahl des Dateityps Dateien mit den 
Endungen *.doc und *.docx bzw. *.dot und *.dotx jeweils in einem Filter angezeigt.
+ Neu: Über "Extras|Optionen" kann man auf der Registerkarte "Einstellungen" mit der Option 
"Berechnete Felder im Abitur" einstellen, ob die die berechneten Felder in der Ansicht "Abitur" 
nicht editierbar sind. 
+ Neu: In der Ansicht "Abitur" wird nun für das Bundesland Nordrhein-Westfalen auch der Durchschnitt
der ersten 3 Prüfungsfächer mit angezeigt.
+ Neu: In der Ansicht "Schüler" können auf der Registerkarte "Daten 3" bis zu 6 Wahlfächer
festgehalten werden.
+ Neu: Ansichten "Schüler"/"Bewerber": Neue Spalte "Profil" verfügbar.
+ Korrektur: Menü Betriebe: beim Wechsel zwischen den Datensätzen über die Pfeiltasten werden die 
Eingaben automatisch gespeichert

### Magellan-Administrator

+ Korrektur:Import und Export der Zugriffsrechte für Haushalt&Inventar
+ Neu: unter Datenimporte|Schlüsselverzeichnisse importieren können auch einzelne Schlüsseldateien 
importiert werden

### Skripte

+ Korrektur: Zuweisen von Kategorietafeln (Zuweisen der Inhaltetafeln für SchuelerASV nachgetragen)  
+ Korrektur: RLP-APO-BGY-1999
+ Korrektur: BER-APO-2011   
+ Korrektur: SAC-APO-BGY-2011
+ Korrektur: BER-APO-KO-2011
+ Korrektur: NRW-APO-BK-2011
+ Korrektur: BER-APO-FOS-2006
+ Korrektur: SHL-APO-2010
+ Korrektur: BAW-APO-BGY-2010-G9
+ Neu: Neue Berufschulskripte für die Schweiz

### Berichte neu oder geändert

- SAC-BG-ABI (E.01.06).rpt
- SAC-BF-JZ (B.04.02).rpt
- BER-FOS-FHReife (Schul Z 511)(05.06).rpt
- SHL-GY-FHReife (2011).rpt
- BER-GY-JZ (Schul Z 251)(07.10).rpt
- BER-GY-ZAS (Schul II 929-11a)(01.09).rpt
- SAC-BG-ABI (E.01.06).rpt
- SAC-BS-AS (A.02.05).rpt
- BER-GY-JZ (Schul Z 251)(07.10).rpt
- Klassenliste Schüler-Notenmatrix (mit Fachniveau).rpt
- Schulbescheinigung (mit Klasse und vorauss. Ende einfach).rpt
- SAC-FO-FHReife (D.01.05).rpt

## 6.0.82 624 (11.06.2012)  

+ interner Test

## 6.0.81 623 (11.05.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

+ interner Test

## 6.0.80 622 (08.05.2012)

+ Magellan-Administrator: Fehler beim Löschen der Magellan-Datenbank behoben.

## 6.0.79 622 (02.05.2012)

+ interner Test

## 6.0.78 622 (19.04.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Unter Stueber S.|Magellan 6|Importe|Berlin steht eine dem Magellan-Importformat entsprechende
Schulenliste zur Verfügung (SchulenBER.csv) 
+ Neu: Verzeichnisse|Arbeits- und Sozialverhalten|Kategorie: Bezeichnungslänge auf 300 Zeichen 
erhöht
+ Neu: ViewSchueler2 für eine Anbindung an Access auf alle Felder der Tabelle Schueler 
erweitert 
+ Neu: beim Fachdatenkopieren (Versetzen, Wechsel, Endnote fortschreiben, Fortschreiben) wird der 
Wert der Spalte Schüler|Zeugnis|Fächer|Niveau übernommen
+ Neu: In der Beispieldatenbank wurde für die Klasse 5a (Demozeitraum) ein Beispiel für die Karte 
Arbeits- und Sozialverhalten(siehe Verzeichnisse|Arbeits-und Sozialverhalten) angelegt

### Skripte

+ Korrektur: NRW-APO-BK-2011 (Hinweis zur Abweichungsprüfung)

### Magellan-Administrator

+ Korrektur: Doppelte Schaltfläche beim Import entfernt

## 6.0.77 621 (13.04.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Korrektur: Menü Personen

### Skripte

+ Korrektur: NIE-APO-G9-2010
+ Korrektur: NIE-APO-G8-2010
+ Korrektur: BER-APO-KO-2011

### Berichte (neu oder geändert)

BER-ABI (Schul II 929-3)(01.09).rpt
BER-GY-ZAS (Schul II 929-11a)(01.09).rpt
NIE-GY-ABI (2010).rpt
BER-GY-ZAS (Schul II 929-11a)(01.09).rpt
BER-GY-ABI (Schul Z 306)(01.09).rpt

## 6.0.76 620 (03.04.2012)

+ interner Test

## 6.0.75 620 (31.03.2012)

### Magellan

+ Neu: Neue Ansicht "Schülergruppen" für Rheinland-Pfalz 

## 6.0.74 620 (29.03.2012)

### Magellan

+ Neu: In der Ansicht "Mandanten" kann auf der Registerkarte "Daten 2" ein Logo gespeichert werden.
+ Neu: Berlin|Ansicht "Schüler"/"Bewerber": Die Registerkarte "Daten 2", "Daten 3" und "Daten 4" werden 
jetzt zusätzlich mit angzeigt
+ Neu: Berlin|Ansicht "Schüler": Per Doppelklick auf das Klassenkürzel kann man in die Ansicht "Klassen"
der enstprechende Klasse wechseln. 
+ Neu: Berlin|Ansicht „Bewerber“, Maske „Grundstufe“: Das Feld „Einschulungsantrag“ inkl. dem 
Feld "von Grundschule" kann analog zur Ansicht "Schüler" eingetragen werden.

## 6.0.73 620 (28.03.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Korrigiert: Zugriffsverletzung im Bewerbermenü
+ Änderung: unter Bewerber/Schüler|Daten4|Banken wird die ID nicht mehr angezeigt

### Berichte (neu oder geändert)

+ Schülerpersonalblatt incl. Schuleintritt und -austritt (mit Vorbildung).rpt
+ BER-GY-ZAS (Schul II 929-9)(12.08).rpt
+ BER-KO-ABI (Schul Z 324)(02.11).rpt
+ Betriebe (Anzahl Auszubildene pro Zeitraum).rpt

## 6.0.72 619 (27.03.2012)
 
### Magellan

+ Korrigiert: Benutzerrechte zuweisen/Synchronisiere Zugriffsrechte wurden um die Rechte für die 
Tabelle Klassenorganisationen ergänzt 

## 6.0.71 619 (22.03.2012)

### Skripte

+ Korrigiert: BER-APO-KO-2011
+ Korrigiert: BER-APO-2010
+ Korrigiert: BER-APO-2011
+ Korrigiert: SAR-APO-BGY-2007

### Magellan-Administrator

+ Korrigiert: Beim Wiederherstellen der mit Firebird 2.1 gesicherten Sicherheitsdatenbank 
„Security2.fdb“ erzeugte Firebird 2.5 eine Fehlermeldung, wenn es sich um Sonderzeichen wie Umlaute 
in Kürzel, Vorname oder Nachname des Benutzers handelt. 

### Magellan

+ Korrektur: für Berlin -> Bewerber|Grundstufe|Sorgeberechtigte: Entfernentaste inaktiv behoben
+ Änderung: für Berlin -> Bewerber|Grundstufe: Felder BerlinPass und Anmeldestatus linksbündig 
+ Korrektur: für Berlin -> Schüler|Grundstufe|Merkmal B3 zweimal vorhanden behoben
+ Änderung: für Berlin -> Klasse|Daten1|Schulform wieder eingeblendet

## 6.0.70 619 (08.03.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Firebird

+ Neu: Ab der Version 6.0.70 wurde Magellan für den Einsatz von Firebird 2.5 optimiert. Wir 
empfehlen neben dem Serviceupdate auch die Firebird-Version zu aktualisieren. Für Nutzer von 
Firebird 1.5 oder 2.1 muss zur Übernahme der Benutzerdaten eine Sicherung und Wiederherstellung der 
Sicherheitsdatenbank durchgeführt werden. Bitte lesen Sie dazu  die Hinweise in unserer 
Magellan-Installationsanleitung (Kapitel "Update von Firebird 2.1 auf Firebird 2.5").

Download Magellan6SetupInfo.de.pdf: 
https://download.stueber.de/doc/de/schulverwaltung/support/Magellan6SetupInfo.de.pdf

Download Firebird 2.5:
https://download.stueber.de/bin/de/magellan/v6/Firebird-2.5.1.26351_1_Win32.exe
  
### Skripte

+ Korrigiert: Zuweisen von Bewerberstammdaten.dws 
+ Korrigiert: SHL-Statistik-ABS: Prüfskript DATEA 2011.xml (EA33) und Magellan.exe
+ Korrigiert: SHL-APO-2010: Durchschnittnote wird korrekt berechnet 
+ Korrigiert: SHL-APO-2010: Mehr als 20 Fächer können geprüft werden
+ Korrigiert: Synchronisiere Zugriffsrechte/Benutzerrechte zuweisen (ASVTypen u.a.)

### Magellan

+ Korrigiert: Schüler|Ausbildung|Neuen Kontakt anlegen: der OK-Button bleibt inaktiv
+ Korrigiert: Schüler|Bearbeiten|Sammelzuweisung|Religionsteilnahme
+ Neu: die Datenübergabe für den Word Seriendruck wird auch für Word 2010 64 Bit unterstützt 
+ Korrigiert: Länge der Telefonnummer und Faxnummer unter Schüler|Ausbildung 
+ Korrigiert: Länge der Telefonnummer und Faxnummer unter Schüler|Sorgeberechtigte 
+ Neu: es kann jedem Fach ein übergeordnetes Fach aus dem gleichen Verzeichnis unter 
Magellan|Verzeichnisse|Fächer|Spalte:"Hauptfach" zugeordnet werden

### Magellan-Klassenbuch

+ Korrigiert: Schülerfilter für die Fehlzeitenerfassung
+ Korrigiert: Einlesen von daVinci-Dateien überarbeitet

### Installation

+ Neu: Stüber-Produkte werden alle in einem Stüber Systems-Verzeichnis  abgelegt (bestehende Pfade 
bleiben erhalten, nur für Neuinstallationen)

### Berichte(neu oder geändert)

+ SHL-GY-AZ (A3).rpt
+ Klassenliste Schüler-Notenmatrix (mit Verhalten und Mitarbeit).rpt
+ Klassenliste Schüler-Notenmatrix.rpt
+ BER-BS-AS (MSA  Schul Z 502).rpt
+ BER-BS-HJZ (Schul Z 500).rpt
+ BER-BS-AS (Schul Z 501).rpt
+ Bewerberpersonalblatt.rpt
+ BER-GY-ZAS (Schul II 929-9)(12.08).rpt
+ BER-GY-ABI (Schul Z 306)(01.09).rpt
+ BER-GY-ZAS (Schul II 929-9)(12.08).rpt

## 6.0.69 619 (02.03.2012)

+ interner Test

## 6.0.68 618 (09.02.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Korrigiert: Belegung der F3-Taste durch die Suchfunktion
+ Korrigiert: Doppelklickverbindung zwischen Schüler|Sorgeberechtigten und dem Sorgeberechtigten
+ Korrigiert: Doppelklickverbindung zwischen Schüler|Ausbildung und dem Betrieb
+ Korrigiert: Sammelzuweisung|Feld AbgangAm
+ Korrigiert: Extras|Optionen|Ein-/Ausblenden|Berufsschuldaten
+ Korrigiert: Schüler|Ausbildung|Ausbilderkontakt unter Schüler hinzufügen
+ Korrigiert: Bewerber|Seriendruck: es wird auf Betriebekontakte verwiesen statt auf Ausbilder
+ Korrigiert: Im Seriendruckassistenten werden nur die Dateinamen der Vorlagen gezeigt, nicht die 
Pfade
+ Korrigiert: Abitur|Qualifikation: das Meldungsfenster schließt automatisch sobald die Simulation 
aufgerufen wird
+ Korrigiert: Problem beim Ausführen des Statistikassistenten behoben (Feld Ausbilder)
+ Neu: Unter Schüler|Sorgeberechtigte wird die jeweilige Mobilnummer mit angezeigt
+ Neu: Schleswig-Holstein: neue Verzeichnisse fürs Arbeits- und Sozialverhalten (Typen, Arten, 
Inhaltetafel, Inhaltetafelkategorien, Kategoriegruppen). Diese neuen Verzeichnisse können bei den 
Schülern unter Zeugnis|Arbeits- und Sozialverhalten genutzt werden.
Typen: unterscheidet zum Beispiel zw. Fachlichen Leistungen und Allgemeinem Lern- u. Sozialverhalten
Arten: unterscheidet zum Beispiel zwischen Arbeits- und Lernverhalten/Sozialverhalten/Deutsch
/Biologie...
Inhaltetafel:  unterscheidet zwischen den Unterrichtsthemen der einzelnen Klassen, zum Beispiel 
Deutsch Klasse 8, Deutsch Klasse 7
Inhaltetafelkategorien: enthält die einzelnen Unterrichtthemen, zum Beispiel für Deutsch Klasse 8 
Kategoriegruppen: kann zum Gruppieren der Kategorien genutzt werden. Beispiel: Kategoriegruppe zur 
Art Deutsch: "Beim Schreiben". Kategorien wären dann zum Beispiel: Texte planen, Texte überarbeiten 
usw.
Alle vorbereiteten Punkte können als Kategorietafel zusammengestellt und gesammelt den Schülern 
eines Jahrgangeszugewiesen werden. Die Bewertung kann nach Typ (Fachliche Leistung/allg. Lern- und 
Sozialverhalten)getrennt erfolgen.
+ Korrigiert: Zeugnisbemerkung editieren per Doppelklick
+ Korrigiert: inkrementelle Suche beim Klassenlehrer einer Klasse
+ Korrigiert: Anzeige der Ausbildungskarte bei Lizenzen ohne Modul Berufsschule/Praktikumsbetriebe
+ Korrigiert: Ein- und Ausblenden der Berufsschuldaten unter Klassen|Daten
+ Korrigiert: Berlin|Bewerber|Sek I: Wechsel von der Sek I-Maske in die Auswahlliste, Aufruf des 
Bewerberverfahrens
+ Korrigiert: Berlin|Bewerber|Sek I|Aufnahmekriterien: vier Felder und Ranking werden gespeichert 
vor dem Wechsel auf die Karte Zugang
+ Korrigiert: Berlin|Bewerber|Sek I|Aufnahmekriterien: vier Felder und Ranking werden gespeichert 
vor dem Wechsel in anderen Menüpunkt
+ Korrigiert: Berlin|Bewerber|Sek I|Aufnahmekriterien: Ranking und Summe werden ohne Werte 
zurückgesetzt
+ Korrigiert: Berlin|Bewerber|Sek I|Aufnahmekriterien|Punkte und Summe: Bei abweichenden Eingaben 
werden entspr. Meldungen ausgegeben
+ Korrigiert: Berlin|Schüler|Auswahlliste: wenn keine Standardmaske gewählt ist, wird die aus der 
Liste gewählte Maske für übernommen
+ Korrigiert: Löschen der FachtafelFächerzeilen durch die Entf-Taste behoben
+ Korrigiert: Schüler|Ausbildung|Details eingeblendet
+ Korrigiert: Extras|Optionen|Rechtschreibkorrektur: "Rechtschreibkorrektur während der Eingabe"

### Skripte

+ Korrigiert: SAC-APO-BGY-2010: Rundungsfehler bei der Durchschnittsnote korrigiert
+ Korrigiert: RLP-APO-2006: Prüfung der Leistungskurse angepasst
+ Korrigiert: SAR-APO-2007: Berechnung der Endnote korrgiert
+ Korrigiert: Importiere DWH Magellan.dws
+ Korrigiert: SHL-Statistik DATEA 2011.xml (EA85)

### Magellan-Administrator

+ Neu: ohne CheckIn-Lizenz ist die Karte unter Server-Verbindung|Verbindungen verwalten|Karte 
CheckIn ausgeblendet

### Berichte (neu oder geändert)

BER-GY-ZAS (Schul II 929-9)(12.08).rpt
BER-GY-ABI (Schul Z 306)(01.09).rpt
BER-GY-ZAS (Schul II 929-9)(12.08).rpt
SAC-BF-HJI (B.04.01).rpt
SAC-BF-HJI (B.01.01).rpt
SAC-BVJ-AS mit HS (A.01.08).rpt
SAC-BGJ-AS ohne HS (A.01.11).rpt
BER-GES-AZ (Schul Z 203)(04.08).rpt 
SAC-BVJ-AS mit HS (A.01.08).rpt
SAC-BGJ-AS ohne HS (A.01.11).rpt
SAC-BGJ-AS mit HS (A.01.09).rpt
SAC-BS-HJI (A.01.04).rpt
SHL-GY-HJZ (Profil).rpt
NRW-BKO-ABI (Anlage D33).rpt
SAC-BVJ-HJI (A.01.03).rpt
SAC-BG-ABI (E.01.08).rpt
Klassenliste (Betriebe mit Auszubildenden nach Gemeinden).rpt
SHL-GEMS-AS.rpt
Schülerpersonalblatt incl. Schuleintritt und -austritt (mit Vorbildung).rpt
Schülerpersonalblatt incl. Schuleintritt (mit Vorbildung).rpt
Schülerpersonalblatt incl. Schuleintritt (Betriebe).rpt
Schülerpersonalblatt (ohne Vorbildung).rpt
Schülerpersonalblatt (nur mit Eltern und Vorbildung).rpt
Schülerpersonalblatt (A5 - Laufbahn).rpt
Schülerpersonalblatt (mit Vorbildung).rpt
RLP-FO-HJZ (2012).rpt
SAC-BG-ABI (E.01.08).rpt
SAC-BF-AS (B.04.06).rpt
SAC-BF-AS (B.04.05).rpt
SAC-BVJ-HJI (A.01.03).rpt
NIE-GY-ABI (2010).rpt

## 6.0.67 617 (09.01.2012)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

Info: es wird parallel eine neue MyMagellan-Version (6.0.7) veröffentlicht.

### Magellan

+ Neu: Unter Abitur|Prüfung(Tabelle SchuelerAbi) wurden neue Felder zum erfassen einer zweiten mdl. 
Leistung für das 1. bis 5. Prüfungsfach ergänzt
+ Neu: Unter Verzeichnisse|Fächer (Tabelle Faecher) wurde eine neue Spalte ergänzt, diese soll 
künftig für Merkmale für den Zeugnisdruck genutzt werden
+ Korrektur: NIE-APO-G8-2010: Die Einbringung der Besondernen Lernleistung wurden korrigiert. Wenn 
die BL eingebracht werden soll, wird das 4.PF nicht mitgewertet, stattdessen wird 4fach (2s+m)/3 
für den Bereich II übernommen.
+ Korrektur: NIE-APO-G9-2010: Die Einbringung der Besondernen Lernleistung wurden korrigiert. Wenn 
die BL eingebracht werden soll, wird das 4.PF nicht mitgewertet, stattdessen wird 4fach (2s+m)/3 
für den Bereich II übernommen.
+ Korrektur: BER-FOS-2006: Abitur|Prüfung: Berechnung der Summe korrigiert, wenn für die 
Prüfungsfächer zur Vornote eine mdl. und auch eine schriftl. Prüfung abgelegt wird
+ Neu: Neue Bewerber- und Schülermasken für Berlin. Beachten Sie dazu auch das aktualisierte 
Magellan-Benutzerhandbuch.
+ Korrektur: Zuweisung der Masken korrigiert
+ Korrektur: Übernahme der Pfade im Willkommensassistenten und Zuweisen des Bundeslandes korrigiert
+ Korrektur: Löschen von Beispiellehrern mit Bezug zum Klassenbuch korrigiert
+ Korrektur: BER-APO-KO-2011
+ Neu: BER-APO-2011
+ Neu: Unter Schüler|Bearbeiten|Sammelzuweisung steht das Feld "Abgang am" zur Verfügung
+ Neu: Unter Schüler|Ausbildung wird auf BetriebeKontakte verwiesen, statt auf das Feld Ausbilder
+ Neu: Unter Bewerber|Ausbildung wird auf BetriebeKontakte verwiesen, statt auf das Feld Ausbilder

### Magellan-Berichte

+ Korrektur: individuell augewählte Region und Berichtsart wird korrekt in der Registry gespeichert

### Magellan-Administrator

+ Korrektur: Löschen des Datenbankinhalts an die Datenbankversion 616/617 angepasst

### Berichte (neu oder geändert)

+ BER-GS-AS (Schul Z 100)(09.05).rpt
+ SHL-GEMS-AS.rpt
+ BER-GY-AZ (Schul Z 303)(12.07).rpt
+ BER-GY-ABI (Schul Z 306)(01.09).rpt
+ SAC-BS-AS (A.02.04).rpt
+ RLP-GY-FHReife (Jahrgangstufe 12).rpt
+ RLP-GY-FHReife (Jahrgangstufe 11).rpt
+ Unfallanzeige (in word ausfüllbar).rpt
+ RLP-RSPLUS (HJZ-AS-AZ und 5.-10. Klasse).rpt
+ BER-GY-JZ (Schul Z 302)(12.07).rpt
+ Schüler (Zeitraumübergreifende Notenübersicht).rpt

## 6.0.66 616 (11.12.2011)   

* Betaversion für Berliner Masken

## 6.0.65 615 (29.11.2011)

### Magellan

+ Korrektur: Hinzufügen und Ändern von Fächern im Menü Abitur|Qualifikation korrigiert
+ Korrektur: Registryschlüssel zur Position der Spalte "mündliche Note" unter Schüler|Zeugnis|
Leistung korrigiert
+ Korrektur: Anzeige des Typs unter Sorgeberechtigte|Auswahlliste an den Eintrag unter 
Sorgeberechtigte|Daten angepasst
+ Korrektur: Anzeige des Verzeichnisses Staatsangehörigkeiten beim Wechseln von Schülern korrigiert
+ Korrektur: Unter Hilfe|Lizenz wird das Statistikmodul angezeigt
+ Korrektur: Worddateien mit den Endungen dotx und docx werden beim Seriendruck angezeigt
+ Korrektur: Benennung von gespeicherten Schülerdateien (PDF oder Word)korrigiert
+ Änderung: Anzeige der Sorgeberechtigten nach Anlegereihenfolge
+ Korrektur: Verzeichnisse|Verordnungen|Skript wird das Verzeichnis angezeigt
+ Neu: Magellan Live Message ist ab dieser Version verfügbar.

### Magellan-Berichte

+ Korrektur: Anzeigeproblem behoben und Textdatei erweitert

### Magellan-Administrator

+ Korrektur: Einlesen des Postleitzahlverzeichnisses für Deutschland korrigiert
+ Korrektur: Import der Schlüssel korrigiert

### Statistik

+ Korrektur: Prüfskripte und Magellan.exe für RLP-ABS korrigiert
+ Korrektur: Prüfskripte und Magellan.exe für RLP-BBS korrigiert
+ Korrektur: Prüfskripte und Magellan.exe für SHL-ABS korrigiert

### Berichte (neu oder geändert)

+ RLP - Lehrer (Abwesenheitsstatistik nur Krank).rpt (ausführbar für alle Benutzer)
+ RLP - Lehrer (Abwesenheitsstatistik).rpt (ausführbar für alle Benutzer)
+ RLP-GS-AS (1. Klasse – 1 seitig - dynamisch 2012).rpt
+ BER-GY-JZ (Schul Z 250)(05.08).rpt
+ SAC-BG-HJZ (E.01.04).rpt
+ RLP-GS-HJZ_JZ (3. und 4. Klassen-2 seitig dynamisch 2012).rpt
+ RLP-GS-AZ (3. und 4. Klasse - 2 seitig - dynamisch 2012).rpt
+ SAC-BG-ABI (E.01.08).rpt
+ SAC-BS-JZ (A.02.01).rpt
+ SAC-BS-AS (A.02.04).rpt
+ SAC-BS-AZ (A.02.02).rpt
+ SAC-BS-AZ (A.02.03).rpt
+ SAC-BG-HJZ (E.01.03).rpt
+ SAC-BG-HJZ (E.01.01).rpt
+ SAC-FO-FHReife (D.01.06).rpt
+ RLP-GS-AZ (1. Klasse – 1 seitig - dynamisch 2012).rpt
+ RLP-GS-AS (1. Klasse – 1 seitig - dynamisch 2012).rpt
+ SAC-FS-HJZ (C.01.03).rpt
+ BER-GY-AZ (Schul Z 303).rpt
+ Schüler (Zeitraumübergreifende Notenübersicht).rpt

## 6.0.64 615 (29.08.2011)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Korrektur: Fehler beim Bewerber-Seriendruck behoben
+ Neu: Berücksichtigung der Installation für die Schweiz

### Statistik

+ Rheinland-Pfalz Korrekturen

## 6.0.63 614 (17.08.2011)

### Magellan-Klassenbuch

+ Neu: Das Magellan-Klassenbuch ist ab sofort als Zusatzmodul verfügbar

### Magellan

+ Korrektur für Ansicht "Berufsschule": BER-BBS-Matrix-2007
+ Korrektur: Fehler beim Import von Stundentafeln aus daVinci 5 bzw. daVinci 6 behoben
+ Korrektur: Fehler beim Zuweisen von Fachtafeln behoben
+ Korrektur: Anzeigefehler im Menü Abitur|Qualifikation behoben, Fachstatus und Unterrichtsart 
werden wieder angezeigt und können ausgewählt werden
+ Korrektur: Menü Bewerber: Legt man einen neuen Bewerber an (Vorname, Nachname) und drückt auf Ok, 
steht der Focus im Anschluss auf Geschlecht statt Anrede.

### Statistik

+ Rheinland-Pfalz Korrektur: RLP-BBS-Plausibilitäten
+ Rheinland-Pfalz Ergänzung: RLP-ABs-Plausibilität Stala_185010
+ Schleswig-Holstein Neu: Die Landesstatistik 2011/2012 wird mit dieser Ausgabe freigegeben. Bitte 
beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf


## 6.0.62 614 (16.08.2011)

+ interner Test

## 6.0.61/62 614 (19.07.2011)

+ Änderung: SQL-Update-Skript zur Datenbankversion 614 wurde angepasst

## 6.0.60 614 (15.07.2011)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Neu: Beim Zuweisen (einzeln oder per Sammelzuweisung) kann ein Häkchen für "Zeugnisbemerkung 
fortschreiben" gesetzt werden. Die markierten Bemerkungen werden beim Fortschreiben oder Versetzen 
mit in den Folgezeitraum übernommen. 
+ Korrigiert: Das Feld Ausbildung unter Daten 1 wird beim Aufruf der Ansicht mit korrekt mit Daten 
gefüllt 
+ Korrigiert: Unter Sorgeberechtigte|Daten|Anrede wurden Anreden korrigiert, jetzt: Frau Prof. Dr., 
Herr Prof. Dr.
+ Korrigiert: Problem beim Senden von Serienmails über Microsoft Outlook behoben
+ Neu: Zeugnisbemerkungen können zum Übernehmen in den neuen Zeitraum beim Versetzen oder 
Fortschreiben markiert werden
+ Korrigiert: Serienmailfunktion funktioniert mit Outlook
+ Korrigiert:Legte man einen neuen Bewerber an (Vorname, Nachname) und drückte auf Ok, stand der 
Focus
im Anschluss auf Geschlecht statt Anrede.
+ Korrigiert: Wenn man in Magellan ein Fach aus dem Fächerverzeichnis löscht, blieb bei den Schülern
unter Schüler|Zeugnis|Fächer eine leere Zeile übrig.
+ Korrigiert: in den Schülerfachdaten oder in den Fachtafeln verwendete Fächer können nicht gelöscht
werden  (wurde mit der 6.0.61 wieder zurückgesetzt)

### Magellan-Bibliothek

+ Korrektur: Als nicht ausleihbar markierte Medien können nicht ausgeliehen werden

### Administrator
+ Korrigiert:  Unter Server-Verwaltung|Verbindungen verwalten|Unterkarte "CheckIn" wird der 
Datenbankpfad korrekt gespeichert

### Abitur

+ Neu: BER-APO-KO-2011

### Berichte

+ Korrigiert: Im Berichte-Explorer wurde die Zuordnung der Berichte zu den Kategorien und 
 Bundesländern überarbeitet
 
### Statistik

 + Berlin Neu: Die Landesstatistik(Abiturerfassung für ABS und BBS) 2011/2012 wird mit dieser 
 Ausgabe freigegeben. Bitte 
beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf
 

## 6.0.59 613 (14.06.2011)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

+ Rheinland-Pfalz: Die Landesstatistik 2011/2012 für Rheinland-Pfalz wird mit dieser Ausgabe 
freigegeben. Bitte beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Landesstatistiken.pdf

### Magellan

+ Änderung(Nachtrag): Beim Kopieren eines Schülers als Bewerber wird für den Bewerber ein Verweis 
auf die Sorgeberechtigten des Schülers angelegt
+ Änderung(Nachtrag): Unter Schüler|Zeugnis|Fächer können keine Fächer mehr nur mit der ENTF-Taste 
gelöscht werden
+ Neu: Schlüsselverzeichnis "Fachniveaus"
+ Neu: Fachtafel ergänzt um Felder "Kurs" und "Niveau"
+ Neu: Zeugnis/Fächer: Neues Feld "Niveau" (kann als Pendelwert/-note für das Saarland genutzt 
werden oder für das Benotungsniveau in SHL (H, R, G))
+ Neu: Zeugnis/Noten: Unterrichtsart und Fachstatus zusätzlich sichtbar. Neue Felder "Zusatz Note 
1", "Zusatz Note 2", "Zusatz Note 3" (einblendbar unter Layout) 
+ Neu: Zeugnis/Noten/Nortenübersicht: Neue Felder " "Zusatz Note 1", "Zusatz Note 2", 
"Zusatz Note 3", "Niveau" werden mit angezeigt
+ Neu: Registerkarte Schüler/Zeugnis/Arbeits- und Sozialverhalten   (Benutzerrechte analog 
Schülerfachdaten)
    - Über Optionen ein-/ausblendbar
    - Bei BBS automatisch ausgeblendet
    - Kategorietafeln können zugewiesen und extrahiert werden (analog Fachtafeln)
+ Neu: Schlüsselverzeichnis für Arbeits- und Sozialverhalten:
    - Kategorien (analog Fächer)
    - Arten  (Verzeichnis innerhalb des Verzeichnisses Kategorien)
    - Bewertungen (analog Noten)
    - Kategorientafeln (analog Fachtafeln)                                                                                                
+ Neu: Ansicht "Abitur/Prüfung"
  +  Feld "Merkmal" für PF1 - PF5 
  +  Feld "Ausschluss Mündliche Prüfung" 
+ Korrigiert: Beim Extrahieren der Fachtafel wird der Faktor  mit in die Fachtafel übernommen
+ Korrigiert: beim Einfügen einer neuen Fachzeile bleibt die Position leer
Skripte:
+ Korrektur: Abiturskript SHL-APO-2010
+ Korrektur: Abiturskript SHL-APO-2007

### Berichte

+ Korrigiert: SHL-GY-FHReife (Profil).rpt
+ Korrigiert: SHL-GY-FHReife (2011).rpt
+ Korrigiert: SHL-GY-AZ (A3).rpt
+ Korrigiert: SHL-GY-ABI (2011).rpt
+ Korrigiert: SHL-GY-ABI (Profil).rpt


## 6.0.58 612 (31.05.2011)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Korrektur: Abiturskript SHL-APO-2010
+ Korrektur: Abiturskript SHL-APO-2007
+ Korrektur: Abiturskript NIE-APO-G9-2010
+ + Korrektur: Abiturskript NIE-APO-G8-2010 
+ Neu: Für den Punkt "Layout anpassen" wird der ursprüngliche Feldname mit angezeigt.
+ Korrektur: Unter Schüler|Zeugnis|Zeugnis|Zeugnisbemerkung|Hinzufügen|Aus Verzeichnis auswählen 
kann inkrementell nach dem Kürzel der Zeugnisbemerkung gesucht werden.
+ Korrigiert: Skripte BER-APO-FOS-2006, bitte beachten Sie, dass unter Abitur|Qualifikation|Layout 
die Spalte "Summe2" statt "Summe" aktiviert sein muss
+ Korrigiert: In den Ansichten Bewerber und Schüler wird die Position der Spalte Geburtsdatum 
gespeichert.
+ Korrigiert: Unter Hilfe|Systeminfo wird jetzt korrekt das Betriebssystems ausgegeben
+ Korrigiert: Beim Versetzen von Schülern wird beim "Übernehmen der Fachdaten" der Wert für "Endnote
fortschreiben" übernommen

### Administrator

+ Neu: Beim Synchronisieren von Benutzerrechten (Ausgelöst durch:Aufruf eines Benutzers|OK)  wird 
überprüft, ob der Benutzer in der security2.fdb angelegt ist. Wird er nicht gefunden,erscheint eine 
Meldung und man kann per "Kennwort ändern" ein neues Kennwort zuweisen und gleichzeitig den Benutzer
in der security2.fdb anlegen lassen.
+ Korrektur (Skripte Benutzerrechte zuzweisen, Zugriffsrechte synchronisieren): Rechtegruppen 
Kollegium1, Kollegium2, Kollegium3 und Kollegium4

### Haushalt&Inventar

+ Korrigiert:  In der Auswahlliste der Haushaltsstellen kann nach Kürzeln (bestehend aus Ziffern 
oder Zeichen) gruppiert werden.

### Berichte

Bitte beachten Sie die Hinweise im Modul ### Magellan:Berichte! 
Die nachstehenden Berichte sind neu, ergänzt oder korrigiert worden:
+ Korrigiert: SHL-GY-FHReife (Profil).rpt
+ Korrigiert: SHL-GY-FHReife (2011).rpt
+ Korrigiert: SHL-GY-AZ (A3).rpt
+ Korrigiert: SHL-GY-ABI (2011).rpt
+ Korrigiert: SHL-GY-ABI (Profil).rpt
+ Korrigiert: SHL-GY-Abi (Leistungskarte Profil).rpt
+ Korrigiert: SHL-GY-Abi (Leistungskarte 2011).rpt
+ Korrigiert: SHL-ABI-Meldung-MdlAbitur (Profil 2011).rpt
+ Korrigiert: SHL-ABI-Meldung-MdlAbitur (Profil).rpt
+ Neu: SAC-BS-AS (B.01.02).rpt
+ Neu: SAC-BS-AS (B.01.02).rpt
+ Neu: SHL-ABI-Meldung-MdlAbitur (Profil 2011).rpt
+ Korrigiert: BER-BF-AS (Z 522a)(04.11).rpt
+ Korrigiert: SHL-ABI-Meldung-MdlAbitur (Profil 2011).rpt
+ Korrigiert: BER-BF-AS (Z 522a)(04.11).rpt
+ Erweitert: BAW-BBS-AS (2011).rpt
+ Erweitert: Schülerausweis ohne Photo.rpt
+ Neu: RLP-RSPLUS (HJZ-AS-AZ und 5.-10. Klasse).rpt
+ BER-BS-HJZ (Schul Z 500).rpt
+ Erweitert: Medienvorgänge mit Signatur.rpt
+ Erweitert: BER-KO-AZ (Schul Z 321)(03.11).rpt
+ Korrigiert: Klassenlehrerliste mit Räumen.rpt
+ Korrigiert: NIE-GY-AS (Kurshalbjahr G8).rpt


## 6.0.57 611 (10.05.2011)

### Magellan
+ Korrektur: Fehler beim Einschulen der Schüler behoben
+ Korrektur: Für die Bezeichnung der Fächerthemen und die Bezeichnung der Fächerthemenunterpunkte 
stehen jeweils 200 Zeichen zur Verfügung
+ Korrektur: Serienmail "An alle Sorgeberechtigten der markierten Bewerber"   
+ Korrektur: Fehlermeldung beim Wechsel von Bewerber zu Schüler wurde behoben.
+ Korrektur: Unter bestimmten Umständen kann es sein, dass in der Tabelle "MedienExemplare"
    das Feld "Status" nicht initialisiert wurde. Dieses Feld benötigt einen
    Standardwert. Dieser Wert wird jetzt im SQL-Update 600.DDL gesetzt.
+ Korrektur: Unter Extras|Statistik wurde die Auswahl der Zeiträume korrigiert    
+ Korrektur: für das Einschulen neuer Schüler wurde die Vorgabe für "Schulbesuchjahre" und 
"Ausbildungsjahre" geändert

    
### Magellan:Administrator:
+ Korrektur: Anpassungen der Anzeige von Ansichten für den StatistikAdmin
+ Korrektur: im Magellan-Importformat heißen die Felder für den ZugangAm und AbgangAm der Lehrer neu 
ZugangDatum und AbgangDatum
    
### Magellan:Center:
+ Korrektur: Es können auch Daten für Benutzer mit der Rechtegruppe Schulleitung2 verteilt werden

### Berichte

Bitte beachten Sie die Hinweise im Modul ### Magellan:Berichte! 
+ geändert: RLP-GY-FHReife (Jahrgangstufe 11-13).rpt
+ Neu: SHL-GY-FHReife (2011).rpt
+ Neu: SAC-FS-AS (C.01.11).rpt
+ Neu: SAC-BS-AS (A.02.04).rpt
+ Neu: SAC-BS-JZ (A.02.01).rpt
+ Neu: SAC-FS-AS (C.01.13).rpt
+ Neu: SAC-BS-AS (A.01.08).rpt
+ Neu: SAC-BS-AS (A.01.06).rpt
+ Neu: SAC-FS-AS (C.01.05).rpt


## 6.0.56 611 (05.04.2011)

### Magellan

+ Korrektur des Skriptes "Synchronisiere ABI", die Merkmale aus Schüler|Zeugnis|Fächer|Merkmale 
werden korrekt übernommen.
+ Korrektur: Für die Berlin steht das Abiturverordnungsskript BER-APO-2010 zur Verfügung.
+ Neu beim  Daten für das Abitur synchronisieren:Unterrichtsart= Besitzt ein Fach bei einem Schüler 
unterschiedliche Unterrichtsarten, so können diese Einträge wahlweise auch getrennt synchronisiert 
werden.
+ Neu: Im Assistenten beim Synchronisieren von Abiturdaten werden die Gruppierungen, Sortierungen 
oder Filterungen gespeichert.
+ Korrektur: Feldlänge beim Seriendruck an Betriebe des Bewerbers (Betriebe_Internet) angepasst.
+ Neu: Das Feld "Umschulung" wird in der Schüler-Auswahlliste angezeigt
+ Korrektur: Unter Schüler|Zugang/Abgang|Bereits besuchte Schulen|Abschluss werden aus dem 
Verzeichnis "Abschlüsse(extern)" alle Kategorien(keine, ABS, BBS oder ABS+BBS) von Abschlüssen 
angezeigt
+ Korrektur: Das Feld Betriebe_Internet kann jetzt korrekt für den Seriendruck aus den Menüs 
Bewerber, Schüler oder Betriebe ausgegeben werden
+ Korrektur: das Prüfskript "BER-Statistik SchuelerABS 2010.xml"  wurde überarbeitet
+ Korrektur: Meldung beim Abbruch der Anmeldung wurde entfernt
+ Neu: Unter Schüler|Zeugnis|Details kann jetzt auch der Prüfungsvorsitzende per Sammelzuweisung 
verteilt werden

### Magellan:Administrator

+Neu: (Datenimport|Magellan-Importformat|Schüler)
Existiert in einem der Zeiträume in der Datenbank bereits ein Schüler/Bewerber mit gleichem 
Vornamen, Nachnamen und Geburtsdatum, wird der Schüler/Bewerber erneut mit eingelesen. Zur 
Unterscheidung wird für den  Schüler-/Bewerberdatensatz ein Unterstrich ( „_“) vor dem Nachnamen 
ergänzt. 
Beispiel: Aus dem doppelt erkannten „Fritz, Müller“ wird „Fritz, _Müller“.
Bei der Sortierung in den Auswahllisten nach dem Nachnamen werden diese Schüler/Bewerber als erste 
Datensätze angezeigt.
Sie können sich dann entscheiden den Datensatz zu löschen oder den Nachnamen wieder abzuändern.
Wichtig: Es erfolgt keine Aktualisierung der Schüler-/Bewerberdaten durch erneutes Einlesen, sondern  
die Datensätze werden neu  angelegt.
Bitte beachten Sie dazu auch das geänderte Magellan-Import.pdf:
https://download.stueber.de/doc/de/schulverwaltung/dokumentation/Magellan-Import.pdf
+ Korrektur: In der Benutzerverwaltung können jetzt auch Benutzer gelöscht werden, die nur in der 
Magellan-Datenbank existieren, nicht aber in der security2.fdb
+ Korrektur: Für das Magellan-Schülerimportformat wurde das Feld Behinderungsart in "Behinderung" 
korrigiert 

### Magellan:Bibliothek

+ Korrektur: Problem beim Übernehmen von gefilterten Schüler-Datensätzen als Ausleiher wurde behoben

### Berichte

Bitte beachten Sie die Hinweise im Modul ### Magellan:Berichte! 
+ Neu: SAC-FS-JZ2 (C.01.02).rpt 
+ Neu: SAC-FS-JZ1 (C.01.02).rpt 
+ Korrigiert: RLP - Lehrer (Abwesenheitsstatistik).rpt 
+ Korrigiert: RLP - Lehrer (Abwesenheitsstatistik nur Krank).rpt 
+ Neu: Notfallzettel.rpt 
+ Neu: BER-GS-JZ (Schul Z 103)(11.05).rpt 
+ Korrigiert: BER-GY-JZ (Schul Z 251)(05.08).rpt 
+ Neu: BER-GS-JZ (Schul Z 100)(09.05).rpt 
+ Neu: Anmeldeschein (weiterfuehrende Schulen).rpt 
+ Neu: Bescheinigung Schulbesuch (mit Wochenstunden-Schul II 912).rpt 
+ Korrigiert: Anmeldebogen 5 Klasse.rpt 
+ Korrigiert: Klassen (Fax an Betriebe der Schueler).rpt 
+ Neu: SAC-BS-AZ (A.02.02).rpt 
+ Neu: SAC-BS-AS (A.02.04).rpt neu
+ Neu: Mandant (Anzahl Schueler nach Bundesland und Zeitraum).rpt
+ Korrektur: RLP-GY-FHReife (Jahrgangstufe 13).rpt


## 6.0.55 611 (18.02.2011)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Korrektur des Skriptes "Synchronisiere ABI", die Merkmale aus Schüler|Zeugnis|Fächer|Merkmale 
werden korrekt übernommen.
+ Korrektur: neu angelegte Fachtafeln können korrekt zugewiesen werden.
+ Beim Neuanlegen eines Bewerberes, der bereits als Schüler in der Datenbank vorhanden war und daher
 kopiert wird, wird jetzt das Geburtsland auch übernommen.
+ Spaltenbreite der Auswahlfelder Abschluss1 und Abschlussart angepasst

### Magellan:Administrator:

+ Das Passwort unter Datenbank|Administrator-Kennwort wird verschlüsselt angezeigt 

### Magellan:Bibliothek

+ Korrektur: der Mahnungen, wenn der Ausleiher inaktiv gesetzt wurde aber das Datum der Ausleihe 
noch in der Zukunft liegt.
+ Änderung: Bericht Mahnungen.rpt verbessert
+ Korrektur: beim Hinzufügen von Schülern

### MyMagellanCenter

+ Korrektur beim Einlesen von Werten in das Feld Zeugnis.Merkmal 

### Abiturverordnungen

+ Niedersachsen: Die Abiturverordnung 2010 für Niedersachsen wird mit dieser Ausgabe freigegeben. 
Bitte beachten Sie das aktualisierte Dokument Landesanpassung.
+ Schleswig-Holstein: SHL-APO-2010.dws Die Abiturverordnung 2010 für Niedersachsen wird mit dieser 
Ausgabe freigegeben. 
Bitte beachten Sie das aktualisierte Dokument Landesanpassung.

### Berichte

Bitte beachten Sie die Hinweise im Modul ### Magellan:Berichte! 
+ Der Bericht "Klassenliste Schüler-Notenmatrix (mit Verhalten und Mitarbeit).rpt" wurde korrigiert
+ Der Bericht "RLP-GY-JZ (2spaltig und mit Wahl- oder Pflichtfächern Variante 2)" wurde erstellt.
+ Der Bericht "SHL-GY-Abi (Leistungskarte 2011).rpt" wurde erstellt.
+ Der Bericht "Gesamtliste (Anzahl Schüler pro Wohnort und Ortsteil nach Jahrgang).rpt" wurde 
erstellt.
+ Der Bericht "Unfallanzeige (in word ausfüllbar).rpt" wurde korrigiert
+ Der Bericht "Gesamtliste (Anzahl Schüler pro Wohnort und Ortsteil nach Jahrgang).rpt" wurde 
erweitert (zusätzlich Summen pro Stadt).
        
## 6.0.54 610 (19.01.2011)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan 

+ Markierung des aktuellen Zeitraumes beim Aufruf des Schlüsselverzeichnisses Zeiträume korrigiert
+ Zeugnisbemerkungen können aus dem Verzeichnis per Doppelklick ausgewählt werden
+ Schüler mit mehreren Betriebszugehörigkeiten werden nur noch in dem aktuellen
Betrieb unter Auszubildende ausgegeben
+ Anmeldung zum Übertrag von Daten in das DataWarehouse korrigiert
+ inkrementelle Suche im Assistenten "Fachtafel zuweisen" ergänzt 
+ Problem beim Seriendruck(Kürzellänge Staatsangehörigkeit1 und 2) behoben
+ flexible Breite für die Bezweichnung in den Auswahlfeldern Ausbildung|Beruf + Ausbildung
|Bildungsgang ergänzt
+ Bei der Synchronisation werden keine ausgeschulten Schüler mehr berücksichtigt
+ Korrektur des Pfades zur Update.Info-Datei

### Administrator

+ Korrektur: Beim Entfernen der Benutzer werden die Rechte entsprechend entzogen
+ Korrektur der Benutzerrechtzuweisung
+ Korrektur für den CSV-Import (Schueler|Feld Status)
+ Korrektur: Beim Zuweisen von Benutzerrechten bleibt der aktuelle Benutzer markiert 

### Bibliothek 

+ Die Rechtegruppe Bibliothekar hat zusätzlich zum sysdba (Administrator) das 
+ Recht unter Extras|Optionen auf den nachstehenden Karten Einstellungen vorzunehmen. Für alle 
  anderen Anwender sind diese Unterkarten ausgeblendet:
- Ausleihe
- Quittung
- Mahnwesen
- Dokumente 
+ Korrektur: Korrekturfunktion um "Korrektur fälschlich ausgewiesener Exemplarstatus" erweitert. 
+ Neu: Filterfunktion bei Vorgängen und Historie (testweise) eingeschaltet. 
MyMagellan Center:
Änderungen für MyMagellan werden gesondert in der MyMagellan-LiesMich-Datei beschrieben:
https://download.stueber.de/bin/de/magellan/v6/Magellan6.Liesmich.txt
+ Korrektur: Problem bei der Speicherung der Fensterposition behoben
 
 
## 6.0.53 (19.10.2010)

+ Korrektur: Problem behoben beim Anlegen von neuen Benutzern.
+ Neu: In der Ansicht "Schüler" bzw. "Bewerber" können jetzt Serienemails über "Bearbeiten|
Serienemails" versendet werden.
+ Neu: In der Ansicht "Bewerber" können die eingebenen Stammdaten eines Bewerber über "Bearbeiten|
Als Vorlage speichern" als 
  Vorlage gespeichert werden. Hierbei werden alle eingegeben Stammdaten mit Ausnahme der Felder 
  - "Nachname", "Vorname", "Geburtsdatum", "Geburtsort", "Bemerkung"
  - Daten der Registerkarte "Sorgeberechtigte"
  - Daten der Registerkarte "Extras" 
  Bei der Neuanlage ein Bewerbers kann nun optional eine Vorlage als Kopiervorlage ausgewählt werden.
  Das Umbenennen und Löschen von erstellten Vorlagen erfolgt in der Ansicht "Bewerber" über 
  "Bearbeiten|Vorlagen bearbeiten"
+ Neu: Unter "Extras|Optionen" kann auf der Registerkarte "Rechtschreibung" die Rechtschreibprüfung 
aktiviert werden. Sie 
  kann beim Erstellen von Zeugnisbeurteilungen  (z.B. bei Grundschulen) und Zeugnisbemerkungen 
  angewendet werden. 
+ Korrigiert: Fehler im Statistikmodul RLP 
+ Korrigiert: Ansicht "Abitur": Anzeigefehler beim Schließen der Simulationsfensters.
+ Korrigiert: Ansicht "Schüler", Register "Zeugnis/Fächer": Anzeigefehler bei Auswahlanzeige in der 
Spalte "Lehrer".
+ Neu: Im Dialaogfenster "Optionen" kann man auf der Registerkarte 
"Dokumente/Dateinamenkonventionen" die neue Einstellung
  "[Datum,Uhrzeit] Name - Berichtsname" bzw. "[Datum,Uhrzeit] Name - Vorlagenname" wählen. In 
  beiden Fällen wird 
  beispielweise bei einem Schüler neben Datum und Uhrzeit auch Nachname + Vorname des Schüler und 
  Klassenkürzel im Dokumentnamen
  gespeichert 
+ Neu: Die Pfad zu den Serviceupdatepaketen haben sich verändert:
  - Magellan 6 Setup: https://download.stueber.de/bin/de/magellan/v6/Magellan6.msi
  - Magellan 6 Liesmich: https://download.stueber.de/bin/de/magellan/v6/Magellan6.Liesmich.txt
  - Magellan 6 UpdateInfo: https://download.stueber.de/bin/de/magellan/v6/Magellan6.updateinfo

### Änderungen für SHL-BBS-Statistik

+ Magellan.exe - Korrektur: Ausgabe von BBS Statistikdaten
+ Katalog      - 026BS_Bildungsgaenge.keys: Korrektur Zeichenlänge zu groß
+ Katalog      - 072BS_SchuelerMerkmale.keys: Korrektur Zeichenlänge zu groß 
+ Skripte      - SHL-Statistik DATSB 2010.xml: Korrektur, Klammerfehler

## 6.0.52 (17.09.2010)

+ Korrigiert: Fehler im Statistikmodul RLP behoben

## 6.0.51 (15.09.2010)

+ Neu: Berlin: Magellan bietet eine Schnittstelle für das eGovernment-Teilprojekt ""Bereitstellung 
der Schülerdaten 2010"
+ Neu: In Drop-Down-Menüs kann mit den Pfeiltaste nach rechts und links navigiert werden
+ Korrigiert: Problem unter Klassen|Zeiträume|Hinzufügen von Zeiträumen ist behoben
+ Korrigiert: Abitur|Qualifikation|Merkmal: mit der Taste Entf wird nur noch ein Zeichen nach rechts
 gelöscht
+ Korrigiert: Berufsschule|Matrix|Merkmal: mit der Taste Entf wird nur noch ein Zeichen nach rechts
 gelöscht
+ Korrigiert: Schüler|Zeugnis|Fächer|Merkmal: mit der Taste Entf wird nur noch ein Zeichen nach 
 rechts gelöscht
+ Korrigiert: ABS-Neuanlage-RLP: Fehler in der Plausibilitätsmeldung für den Zusatz zur 
2.Fremdsprache für Realschule Plus in RLP
+ Korrigiert: BBS-Bewegung-RLP: Statt der Staatsangehörigkeiten 150 und 170 wurde die 133 ausgegeben
+ Korrigiert: BBS-Bewegung.RLP: Für Schüler in Sammelklassen (99) wurde die Schülerklassenstufe 
(MerkmalS6) nicht korrekt ausgegeben.
+ Korrigiert: BBSNeuanlage-RLP: Auslesen eines Dummy-Schülers führte zu Zugriffsverletzung.
+ Korrigiert: BBSBewegung-RLP: Plausi: STALA-37310 / MORGEN-110 - Korrektur Schl. 48 RH-Reife
+ Korrigiert: BBSLehrerNeuanlage Plausi: STALA-5800 korrigiert
+ Korrigiert: BBSNeuanlage Plausi: STALA-39700 entfernt, ist nicht mehr vorhanden
+ Korrigiert: BBSNeuanlage Migrationshintergrund: Korrektur bei der Ausgabe des Feldes 
"FoerderBedarf"
+ Korrigiert: BBSNeuanlage Korrektur der Ausgabe in Magellan passend zur Plausi STUEBER-7 zum Thema 
"Sonderberufe"    
+ Korrigiert: BBSNeuanlage Plausi: STUEBER-7: Korrektur zum Thema "Sonderberufe"
Hinweis für die Kunden zum Thema "Sonderberufe": 
In Magellan ist unter  "Klassen|Daten|Beruf" bei einer Klasse der Berufsschule immer ein Beruf 
einzutragen (bei BVJ optional), um eine korrekte Fehlererkennung zu gewährleisten. Wird einer der 
folgenden Sonderberufe eingetragen, dann wird die Ausgabe dieses Klassen-Berufs in der 
Statistikdatei SchuelerBbsNeuanlage.xml unterdrückt, das das StaLa dies erfordert. 
      96000100  Mithelfende im elterlichen Betrieb oder Haushalt
      97000100  Beschäftigungsverhältnis ohne Ausbildungsvertrag
      98000100  Nichtbeschäftigte (Arbeitslose)
      99000100  Berufsvorbereitungsjahr
      99000150  Schüler/-in in Sondermaßnahmen  Schüler/-in in Sondermaßnahmen
+ Korrigiert: BSNeuanlage Plausi: STALA-13205-2 Korrektur bei der Abfrage des Statusfeldes auf FSP2

## 6.0.50 (06.09.2010)

### Magellan

+ Korrektur: Fehler bei Installation behoben

### Magellan-Administrator

+ Korrektur beim Einlesen der Schlüsselverzeichnisse, Weitere Referenz für Klassenstufen 
(SchuelerSchulen.Klassenstufe) berücksichtigt. Ausserdem wurden gelöschte Datensätze nicht immer 
erkannt und konnten deshalb nicht eingefügt werden.  


## 6.0.49 (02.09.2010)

### Magellan:Administrator

+ Neu: "Benutzer duplizieren". Funktion kopiert einen Benutzer mit gleicher Kennung in anderen 
Mandanten
+ Neu: Zusätzlich zur Funktion "Benutzer duplizieren" wird beim Ausführen von "Benutzer editieren" 
jeder Benutzer gleicher Kennung angepasst. 
+ Korrigiert: Speicherproblem beim Ausführen von "Mandanten kopieren", gelöst durch den Einsatz von
FastMM4
+ Neu: Kopieren der Dokumente beim Ausführen von "Mandanten kopieren"
+ Korrigiert: Funktion "Mandanten Kopieren"; Feld "FahrstreckeKM" der Tabelle "Schüler" wurde nicht
als reelle Zahl interpretiert. 
 
### Magellan

+ Korrigiert: Fachtafeln: Fehler beim Kopieren von Fachtafeln(bereits vergebenes Kürzel wird erneut
genutzt) behoben.
+ Korrigiert: Fachtafeln: Fehler beim Kopieren von Fachtafeln mit 9 oder 10 Zeichen im Kürzel 
behoben.
+ Korrigiert: Fächer Verzeichnis: Sortieren nach Kürzel, bei doppeltem Kürzel ein Datensatz nicht 
anklickbar 
 
### Magellan:Bibliothek

+ Korrigiert: Ansicht "Schüler | Details" - Falsche Anzeige der Klasse und des Klassenlehrers 
korrigiert
+ Korrigiert:  Ansicht "Medien | Exemplare" - Beibehalten des aktuellen Mediums beim Löschen eines 
Exemplares
+Neu: Automatisches Speichern der Mahnungen, Quittungen und Vorgänge pro Lehrer, Schüler und 
Personen unterhalb im Magellan Dokumentenordners unterhalb eines \Bibliothek Unterordners.

### Rheinland-Pfalz Statistik

+ Bei der Datenprüfung in Magellan 6 werden im Listenfenster für die Plausibiltätsmeldungen nun 
zusätzliche Spalten angezeigt, z.B. Klasse.
+ Die Plausi STALA-27000 (BBS-Schüler-Neuanlage) wurde korrigiert. Hier wurden fälschlicherweise 
Berufe beanstandet die über eine 3,5-jährige Ausbildungszeit verfügen.
+ Die Plausi STALA 13100 (ABS-Schüler-Neuanlage) wurde an die aktuellen Neuzugangsschlüssel 
angepasst.
+ Im Magellan-Administrator wurde ein Fehler beim Einlesen der Schlüsseldateien korrigiert.
+ Fehlerkorrektur der Schlüsseldatei "012BS_Berufe.keys";
+ In der Schlüsseldatei "004AS_AbschlüsseIntern" und "004BS_AbschlüsseIntern" wurde der 
Gültigkeitszeitraum des Schlüssels 48 so korrigiert, dass dieser auch bei Bewegungsschülern als 
gültig gekennzeichnet wird
+ Die neue Plausi "STUEBER-12" macht bei den Bewegungsschülern auf einen falsch zugewiesenen 
Schlüssel "43" für FH-Reife aufmerksam.
+ Der Klassenstufenschlüssel "99" wird nun korrekt in die XML Datei (Schüler-BBS-Neuanlage)
übertragen
+ Plausi: STALA-37310 / MORGEN-110 - Korrektur Schl. 48 RH-Reife
+ Auslesen des WohnStaat korrigiert, Land wurde nicht ausgelesen  (BBSNeuanlage)
+ Berechnung des Abgängers ABS korrigiert, SChl. 48 statt 43 abfragen  (BBSNeuanlage)
+ Berechnung des Neuzugangs angepasst (BBSNeuanlage)
+ Plausi: STALA-26700-3 - Korrektur der Meldung (BBSNeuanlage)


## 6.0.48 (30.07.2010)

+ Das unter Magellan|Hilfe|Benutzerhandbuch hinterlegte PDF-Dokument wurde erweitert. 
+ Korrigiert: Fehler beim nachträglichen Verteilen von Fachlehrern per Fachtafel behoben.
+ Korrigiert: Problem beim Feld SchuelerEmail für den Seriendruck behoben.
+ Korrigiert: Fehler bei der Eingabe von Bewerbungsdaten bei neu angelegten Bewerbern behoben.
+ Korrigiert: Fehler beim Anlegen von Schülern behoben (Nutzung der vollen Feldlänge von Vor- und 
Nachnamen).
+ Korrigiert: Sortierung der Schülerzeiträume unter Schüler|Laufbahn erfolgt nach Zeitraum, danach 
nach Halbjahr.
+ Korrigiert: Fehler in der Doublettenprüfung für ausgeschulte namensgleiche Schülerdatensätze aus 
dem vorangegangenen Zeitraum behoben.
+ Neu: Seriendruck ist auch für nichteingeschulte Schüler möglich.
+ Korrigiert: Fehler beim Zuweisen der Versetzungsart unter Schüler|Laufbahn|Allgemein behoben.  


## 6.0.47 (06.07.2010)

+ Fehler bei Installation behoben


## 6.0.46 (05.07.2010)

+ Fehler beim Word-Seriendruck unter Office 2010 beseitigt.
+ Rheinland-Pfalz: Die Landesstatistik 2010/2011 für Rheinland-Pfalz wird mit dieser Ausgabe 
freigegeben. Bitte beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
ftp://ftp.stueber.de/stueber/docs/deu/magellan/ldanpass/Statistik.pdf
+ Schleswig-Holstein: Die Landesstatistik 2010/2011 für Schleswig-Holstein wird mit dieser Ausgabe 
freigegeben. Bitte beachten Sie das aktualisierte Dokument Statistik.pdf auf unserer Webseite:
ftp://ftp.stueber.de/stueber/docs/deu/magellan/ldanpass/Statistik.pdf


## 6.0.45 (25.06.2010)

+ Fehlende Skripte ins Setup eingefügt.


## 6.0.44 

+ Änderung: Das Skript SAC-APO-BGY 2010 für das Abitur 2010 an beruflichen Gymnasien an Sachsen 
wurde korrigiert 


## 6.0.43 (26.05.2010)

+ Neu: das Zeugnis SAC-BG-ABI (2010).rpt für das Abitur 2010 an beruflichen Gymnasien an Sachsen 
wurde eingebunden
+ Korrektur: Das Skript BER-KO-1987 wurde angepasst, die Anzahl Kurse aus Aufgabenfeld III werden 
korrekt gezählt und es können bis zu 40 Fächer in der Qualifikationskarte aufgeführt werden. 
+ Änderung: Unter Magellan|Datenbank|Kennwort ändern kann das Administratorenpasswort nicht mehr 
verändert werden, dieses kann ausschließlich im  Admninistratorenmodul verändert werden.   
+ Änderung: Unter Magellan|Datenbank|Kennwort ändern wird bei die Eingabe des Passwortes als 
Sternchen angezeigt 
+ Neu: Für das Synchronisieren von Berufsschülern in die Berufschulmatrix kann gewählt werden, ab 
welchem Jahrgang die Daten übernommen werden sollen. Dafür definieren Sie bitte unter Verzeichnisse|
Verordnungen in der Spalte  "Jahrgang ab" den ersten Jahrgang, normalerweise sollte hier eine 1 
eingetragen werden. Beim Synchronisieren wird der hier eingestellte Wert mit dem Jahrgang der 
Schüler-Klasse (also unter Klassen|Zeiträume|Allgemein|Jahrgang müsste ein 2 oder 3 stehen) 
verglichen.
+ Neu: Beim Schuljahreswechsel-Assistenten werden jetzt alle Klassenfelder übernommen, 
unzutreffendes kann dann in der Klassenkopie abgeändert werden.
+ Neu: Beim Fortschreiben und beim Versetzen von Schüler steht künftig aus die Spalte Beruf im 
Assistenten zur Auswahl.
+ Änderung: Unter Bewerber|Seriendruck wurde das Feld BewerberPunkte ergänzt.


## 6.0.42 (06.05.2010)

+ Neu: Das Skript SAC-APO-BGY 2010 für das Abitur 2010 an beruflichen Gymnasien an Sachsen wurde 
eingebunden 
+ Korrektur: In der Ansicht "Abitur" können Fächer beim Drucken der Prüfungslisten jetzt korrekt 
ausgewählt werden.
+ Korrektur: Problem(nach dem Update startete Magellan nicht, erst bei einer Reparaturinstallation) 
beim Setup wurde behoben.
+ Korrektur: Problem im Statistikmodul behoben.
+ Korrektur: Das Skript BER-APO-2007 kann jetzt auch mehr als 20 eingetragene Kurse verarbeiten.
+ Änderung: Der Bericht "Betriebe mit Auszubildenden.rpt" sortiert die Auszubildenden nach Klassen.
+ Neu: Bericht "Betriebe mit Auszubildenden(mit Parametern).rpt" , Markieren Sie im Betriebemenü 
einen beliebigen Betrieb und gehen auf die Karte 
"Auszubildende" (um die Klassenkürzel angezeigt zu bekommen). Rufen Sie dann den Bericht über 
Drucken|Bericht auf. Vor dem Druck oder vor der Seitenvorschau erscheint ein Parameterfenster, 
geben Sie das genaue Klassenkürzel ein. Als Ergebnis werden Ihnen in dem Bericht nur die Schüler 
der gewählten Klasse, die den Betrieb besuchen angezeigt. 


## 6.0.41 (30.03.2010)

+ Neu für Rheinland-Pfälzische Berufsschulen: beim Import der Schlüssel über "Administrator|
Datenimporte|Schlüssel importieren|Berufsbildende Schulen" werden zwei Schlüssel 
(HD= höherer Dienst, GD= gehobener Dienst) ins Verzeichnis Besoldungen eingelesen 
(Magellan|Verzeichnisse|weitere Schlüsselverzeichnisse|Besoldungen) mit eingelesen.
+ Korrektur: die Berichte RLP-Lehrer(Abwesenheitsblatt).rpt, RLP-Lehrer(Abwesenheitsstatistik).rpt 
und RLP-Lehrer(Abwesenheitsstatistik nur krank).rpt wird überarbeitet, bitte lesen Sie dazu auch die
Hinweise im Modul Magellan6::Berichte
+ Korrektur: Anzeige der Umbennung der Merkmale in der Auswahlliste der Klassen und Lehrer ist 
jetzt korrekt.
+ Neu: Zum Kopieren von Klassen in den nachfolgenden Zeitraum gibt es eine neue Funktion. Der 
Assistent kann aus Klassen|Bearbeiten|Schuljahreswechsel 
heraus gestartet werden.
+ Neu: Für die Fächerbezeichnung stehen statt 100 neu 200 Zeichen zur Verfügung.
+ Neu: Beim Eintrag der Lehrerfehlzeiten wird das Bis-Datum beim Eintrag des Von-Datums automatisch 
auf den gleichen Wert gesetzt. Beim Eintrag eines 
verkehrten Bis-Datums wird eine Meldung ausgegeben.
+ Neu: Unter Schüler|Drucken finden Sie den Bericht "Schülerliste (inaktive Schüler mit Felder min.
 1 Feld leer AbgangAm Abschluss1 Abschluss1Datum 
Abgangsart).rpt". Bitte beachten Sie die Hinweise für den Bericht im Modul Magellan6::Berichte.
+ Neu: Beim Einschulen von Schülern und dem Zuweisen von Fachtafeln wird bei der Auswahl der 
Schüler zusätzlich der Beruf mit angezeigt.


## 6.0.40  (17.03.2010)

+ Korrektur: Doublettenprüfung beim Anlegen von Schülern wurde überarbeitet.
+ Korrektur: Datensatzwechsel im Schülermenü wurde überarbeitet.


## 6.0.39 (15.03.2010)

+ Korrektur: Problem beim Aufruf von Verzeichnis|Fachtafeln behoben.
+ Neu Bewerber: In der Auswahlliste Bewerber wird jetzt neu auch der Geburtsort mit angezeigt.
+ Neu Bewerber: Wenn beim Anlegen eines neuen Bewerbers die Doublettenprüfung erscheint, können 
jetzt auch inaktive Schüler aus zurückliegenden 
  Zeiträumen als  Bewerber kopiert werden.
+ Bericht überarbeitet: Lehrer|Rheinland-Pfalz: RLP - Lehrer (Abwesenheitsblatt).rpt
+ Neu: Unter Verzeichnisse|Verordnungen|Jahrgang kann man durch Eintragen der Werte 10(für G8) 
und 11(für G9) das Synchronisieren ins Abiturmodul beeinflussen.
+ Neu für Rheinland-Pfälzische Berufsschulen: beim Import der Schlüssel über "Administrator|
Datenimporte|Schlüssel importieren|Berufsbildende Schulen"  werden Lehrerfehlgründe
(Magellan|Verzeichnisse|weitere Schlüsselverzeichnisse|Fehlgründe(Lehrer) mit eingelesen.
+ Neu: Ab den Versionen daVinci 5.0.55 und Magellan 6.0.39 ist ein eingeschränkter Abgleich zwischen
beiden Programmen möglich. Dafür müssen folgende Bestandteile vorhanden und auf dem aktuellen 
Stand sein:
   
    * daVinci= die daVinci-Programmdateien (davinci.exe, davinciA.exe, davinciC.exe) 
    * Magellan= im lokalen Programmverzeichnis muss die MagSDTFdaV5Sync.exe sein und die 
    *     Skriptdateien "Importiere daVinci5 SDTF.dws" und
      "Importiere daVinci5 SDTF.int" müssen vorhanden sein
    
    Bitte beachten Sie Folgendes:
    Unterschiede Abgleich daVinci 5-Magellan 6 zu daVinci 6-Magellan 6
    -------------------------------------------------------------------------
    * Fächer werden nicht abgeglichen, da sich die Fachkategorien geändert haben.
    * Lehrer-Soll-Schlüssel werden bei daVinci 5 aufgrund des Kürzels abgeglichen, bei daVinci 6 
    *     aufgrund der ID (mit daVinci 6 kann man also auch 
      geänderte Kürzel berücksichtigen)

    Unterschiede Abgleich daVinci5/Magellan5 zu daVinci5/Magellan6
    -------------------------------------------------------------------
    * Räume werden in beide Richtungen übertragen bei daVinci 5/Magellan 6
    * Lehrer-Soll-Schlüssel werden von Magellan 6 nach daVinci 5 übertragen (bei daVinci 5/
      Magellan 5 nur nach Magellan 5, aber nicht von Magellan 5 nach daVinci 5) 

+ Neu: Das Feld Schüler|Daten3|Personalnummer steht für Serienbriefe aus dem Schülermenü zur 
Verfügung.
+ Korrektur: Die Berechnung für das  rheinland-pfälzische Bewerberverfahren wurde korrigiert.
+ Neu: Die Religionsteilnahme kann jetzt per Sammelzuweisung für Schüler und Bewerber vergeben 
werden.


## 6.0.38 (08.02.2010)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Ansicht "Lehrer", Lehrerfehlzeit: Die Eingabe der Lehrerfehlzeit wurde um weitere Attribute 
erweitert. Damit können für berufsbildende Schulen in Rheinland-Pfalz alle Angaben für das 
Abwesenheitsblatt pro Lehrer erfasst werden.
+ Neu: Den Bericht "RLP - Lehrer (Abwesenheitsblatt).rpt" finden Sie unter Lehrer|Drucken|
Rheinland-Pfalz. Bitte beachten Sie dazu die Anmerkungen im Modul Magellan 6 Berichte.
+ Ansicht "Schüler": Bei der Übernahme von Schülern als Bewerber können nun auch ausgeschulte 
Schüler ausgewählt werden.
+ Ansicht "Bewerber": Bei der Doublettenprüfung gefundene existierende Schüler können übernommen 
werden, auch wenn der Status inaktiv ist. 
+ Korrektur des Excel-Export des Zeitraumverzeichnisse: Es werden jetzt alle Zeiträume übernommen, 
nicht nur der aktuell markierte Zeitraum.
+ Korrektur: Seriendruck funktioniert jetzt auch, wenn zuvor die Datensätze gefiltert wurden.
+ Seriendruck: Für den Seriendruck aus dem Schülermenü steht zusätzlich das Feld Schüler-ID zur 
Verfügung.
+ Korrektur: Unter Schüler|Fächer wird mit Entf nur die jeweilige Markierung, nicht die Zeile 
gelöscht.
+ Korrektur: Problem beim Anlegen oder Löschen von Datenbankverbindungen wurde behoben.
+ Korrektur: Sorgebrechtigte werden beim Kopieren von mehreren Schülern als Bewerber mit übernommen.
+ Neu: Die Notenarten wurden um die Notenart "Prozente" erweitert. Sie finden diese Notenart zur 
Auswahl unter Klassen|Daten|Beurteilungsart und auch im Verzeichnis Noten|Notenart.  


## 6.0.37 (02.12.2009)

+ Problembehebung in mehreren Assistenten (Markierung)
+ Problembehebung in der Bewerberberechnung
+ Installation überarbeitet für 64Bit-Systeme


## 6.0.33 (09.11.2009)

+ Beim Neuanlegen eines Sorgeberechtigten wird der Status auf aktiv gesetzt.
+ Der Installationsassistent wurde verändert. Es entfällt die benutzerdefiniert Installation. 
Stattdessen kann bei der Server-/Einzelplatzinstallation jeweils ein gesonderter Pfad für die 
Programmdateien, die Datenordner und den Datenbankordner angegeben werden.
+ Problem beim Zuweisen eines Schülerpassfotos wurde behoben. Das Zuweisen aus der Auswahlliste ist 
jetzt nicht mehr aktiv, das Passfoto soll bitte auf Daten1 zugeordnet werden.


## 6.0.29 (15.10.2009)

+ Problem beim Drucken korrigiert.

## 6.0.26 (05.10.2009)

> Die Datenstruktur von Magellan ist erweitert worden! Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend 
alle Arbeitsplatzrechner! Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue 
Datenstruktur durch einen Assistenten. [Weitere Infos finden Sie hier].

### Magellan

+ Ansicht „Abitur“, Registerkarte „Kursmatrix“: Neben der Besonderen Lernleistung könne jetzt auch 
die Präsentationsprüfung und das Projekt als Teil der Abiturprüfung berücksichtigt werden.
+ Korrigiert:: Anrede und Typ werden korrekt gespeichert, beim Anlegen eines Sorgeberechtigten aus 
dem Schülermenü.
+ Korrigiert: In den Emailfeldern der einzelnen Kategorien wird vor die Mailadressen kein  „mailto:“ 
automatisch erzeugt
+ Korrigiert: Statusanzeige aktiv/inaktiv im Schlüsselverzeichnis Klassen|Zeiträume|Zeitraum|
Klassenstufe 
+ Korrigiert: Beim Anlegen eines Schülers/Bewerbers ist nun als erstes nach dem Wechsel auf Daten1 
das Feld Anrede aktiviert
+ Korrigiert: Bei der Auswahl im Feld Geburtsland/Staatsangehörigkeit ist die Eingabe nur mit der 
Tastatur möglich

### MyMagellan-Center und MyMagellan

+ Korrigiert: Teilweise wurde beim Öffnen  des Moduls das Fenster nur kurzzeitig angezeigt und ließ 
sich dann nicht wiederherstellen. 
+ Korrigiert: Mym-Dateien speichern den Pfad  wieder korrekt.


## 6.0.23 (19.08.2009)

+ Fehler bei "Schüler einschulen" behoben.
+ Anzeigefehler bei "Kurslisten drucken" behoben.
+ Magellan-Bibliothek & Lernmittel: Verbesserung der Geschwindigkeit bei der Anzeige der 
Medienausleiher.
+ Fehler unter Klassen|Zeiträume behoben (betrifft die Felder: Elternsprecher, Klassensprecher, 
Wahlvertreter). 
+ Unter Mandanten werden die Lehrer im Feld Schulleiter pro Mandant angezeigt
+ Magellan-Bibliothek & Lernmittel: Für den Ausleihvorgang steht jetzt zusätzlich das Geburtsdatum 
der Ausleiher zur Verfügung.
