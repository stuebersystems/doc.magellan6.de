# Importe und Exporte

## Datenimporte

Über Ansicht und dann Datenimporte gelangen Sie zu den Import-Möglichkeiten von MAGELLAN. Um Daten aus anderen Verwaltungsprogrammen zu importieren, müssen Sie je nach Verwaltungsprogramm die Option Daten aus anderen Verwaltungsprogrammen importieren oder Daten über MAGELLAN-Importformat importieren.

> #### warning::Wichtig!
>
> Eine ausführliche Beschreibung zum Import von Fremdprogrammen oder mit Hilfe unseres MAGELLAN-Importformates finden Sie in der gesonderten Dokumentation [„MAGELLAN-Import“](https://doc.magellan6-import.stueber.de/).



### Andere Verwaltungsprogramme importieren

Über die Option „Daten aus anderen Verwaltungsprogramme importieren“ können Sie folgende Verwaltungsprogramme importieren:

* BBS-Planung (Niedersachsen)
* BBZ/SEKI (Saarland)
* BUSS (Niedersachsen)
* ISIS (Rheinland-Pfalz)
* ISL-Schule
* Omnia
* Ostertun (Schleswig-Holstein)
* SIBANK (Niedersachsen)
* WinSchool

Dazu müssen Sie den Namen des Programms unter Auswahl markieren und dann auf `Start` klicken. Sollten Sie hier ein verbreitetes Verwaltungsprogramm nicht finden, so setzen Sie sich bitte mit STÜBER SYSTEMS in Verbindung. 


### Daten über das MAGELLAN-Importformat importieren

Über die Option „Daten über MAGELLAN-Importformat importieren“ können Sie Daten aus bestimmten Verwaltungsprogrammen und aus beliebigen Dateien importieren, die dem MAGELLAN-Importformat entsprechen. Folgende Verwaltungsprogramme können mit Hilfe des MAGELLAN-Importformates importiert werden:

* IBIS
* LUSD (Hessen)
* SchoolExpert
* SPlan

Eine ausführliche Beschreibung über den Aufbau des MAGELLAN-Importformates und zum Import von Fremdprogrammen über das MAGELLAN-Importformat finden Sie finden Sie in der Dokumentation [„MAGELLAN-Import“](https://doc.magellan6-import.stueber.de/.

### Schlüsselverzeichnisse importieren

Für MAGELLAN existieren Anpassungen an die Bestimmungen einzelner Bundesländer bzw. bestimmter Schularten. Diese Anpassungen richten sich u. a. danach, ob die jeweiligen Stellen der Statistikämter, Kultusministerien bzw. Schulträger entsprechende Datentransferformate usw. anbieten. Durch die Landesanpassung werden die Bereiche Statistik und Oberstufenverwaltung, als auch die Zeugnisse abgedeckt. Um eine MAGELLAN-Datenbank mit neuen Schlüsselverzeichnissen zu aktualisieren bzw. Schlüssel in eine leere MAGELLAN-Datenbank zu importieren, müssen Sie die Option „Schlüsselverzeichnisse importieren“ wählen.

Feld|Bedeutung
---|---
Importiere für folgendes Land/Bundesland|Wählen Sie Ihr Bundesland oder Land aus. <br/>Der Assistent bietet Schlüsselverzeichniskataloge aus dem gleichnamigen Verzeichnis im Verzeichnis Importe (standardmäßig auf Ihrem MAGELLAN-Serverrechern).
Importiere folgende Schlüssel|Es gibt die Auswahl Schlüssel für allgemeinbildende Schulen oder berufsbildende Schulen.<br/>Katalogedateien können mit 00_, AS_ oder BS_ beginnen. Für allgemeinbildende Schulen werden Dateien mit 00_ und AS_ importiert, für berufsbildende Schulen werden Dateien mit 00_ und BS_ importiert.
Importiere für den folgenden Mandanten |Wählen Sie den Zielmandanten aus
Importiere folgenden Katalog|Sie können eine einzelne Datei oder alle zutreffenden Datei einlesen lassen.

![Assistent zum Importieren von Schlüsselverzeichnissen](/images/admin.schluessel.einlesen.png)


#### Eigene Schlüsselverzeichnisse importieren

Unter `Datenimporte > Schlüsselverzeichnisse` importieren können von uns mitgelieferte *.keys-Dateien eingelesen werden. Damit Sie eigene Dateien importieren können, beschreiben wir nachstehend den notwendigen Aufbau der einzelnen Importdateien.

![Wählen Sie Bundesland, Art der Schlüssel und den Mandanten](/images/Import_Export.Schluesselimport.png)

**Importiere für folgendes Land/Bundesland:**

Je nach Auswahl werden die Schlüsseldateien aus dem gleichnamigen Verzeichnis auf Ihrem Serverrechner unter Stueber Systems|MAGELLAN 6|Importe ausgewählt. Legen Sie in den Verzeichnissen eigene Dateien in der richtigen Benennung und mit korrektem Aufbau ab, können diese mit importiert werden.

**Importiere folgende Schlüssel:**

Der Importassistent unterscheidet zwischen Schlüsseldateien für allgemeinbildende Schulen (AS\_xxx) oder für berufsbildende Schulen (BS\_xxx). Die Unterscheidung erfolgt durch den Dateinamen, beginnt der Dateiname mit 00_xxx wird die Datei in beiden Auswahlfällen importieren.

Ein Beispiel:

* 00_Faecher.keys: wird in jedem Fall eingelesen
* AS_Faecher.keys: wird bei Auswahl von „allgemeinbildende Schule“ eingelesen
* BS_Faecher.keys: wird bei Auswahl von „berufsbildende Schule“ eingelesen

**Importiere folgenden Katalog:**

Es können entweder alle keys-Dateien (AS_xxx und 00_xxx oder BS_xxx und 00_xxx ) importiert werden oder Sie wählen eine bestimmte Datei aus.

### Aufbau der Dateien

Den Aufbau der einzelnen Importdatei beschreiben wir im Abschnitt [Referenz > keys-Dateien](../reference/keys-dateien.md).

Jede dieser Dateien muss als CSV-Datei aufgebaut sein, d.h. sie besteht jeweils aus einer Kopfzeile und
ein oder mehreren Zeilen mit den zu importierenden Inhalten. Die einzelnen Felder sind durch
Semikolon getrennt und mit Anführungszeichen abgegrenzt.

Die Importdatei für Fachstatus (00_Fachstati.keys) kann z.B. folgenden Aufbau haben

````
"Kuerzel";"Schluessel";"Bezeichnung";"GueltigVon";"GueltigBis"
"1PF";"1PF";"1. Prüfungsfach";"01.08.2006";""
"2PF";"2PF";"2. Prüfungsfach";"01.08.2006";""
"3PF";"3PF";"3. Prüfungsfach";"01.08.2006";""
"1PFBLL";"1PFBLL";"1. Prüfungsfach und Besondere Lernleistung";"01.08.2006";""
````

Die Felder entsprechen dem sog. System Data Format (SDF), d.h. bei einem Semikolon, Komma, Sonderzeichen oder einem Leerzeichen im String wird der String in Anführungszeichen gesetzt, z.B. dieBezeichnung "1. Prüfungsfach und Besondere Lernleistung " wird 
;“ 1. Prüfungsfach und Besondere Lernleistung“;... und nicht ; 1. Prüfungsfach und Besondere Lernleistung;... geschrieben.
Besitzt der Inhalt selbst Anführungszeichen, so sind doppelte Anführungszeichen anzugeben. Welche Felder pro Datei eingelesen werden, ist den nachfolgenden Abschnitten pro Datei zu entnehmen.

> #### primary::Hinweis
>
> Zeilenumbrüche sind in einer CSV-Datei nicht erlaubt. Das Datenformat bestimmt jede Zeile als einen Datensatz. Ein Umbruch mitten in der Zeile kann nicht verarbeitet werden.
Ändern Sie bitte vor dem Import die Dateiendung in *.keys.



### Was passiert beim Schlüssel importieren?

Beim Einlesen von Schlüsselverzeichnissen wird folgendes der Reihe nach durchgeführt:

1. Alle noch nie verwendeten Schlüssel werden in den Zielverzeichnissen der Datenbank gelöscht.

2. Alle übrigen Schlüssel werden in der Datenbank mit einem älteren Datum versehen und damit als ungültig (graue Raute) markiert.

3. Nun wird geprüft welche Schlüssel eingelesen werden sollen, entscheidend ist dabei lediglich der Wert in der Spalte Schlüssel:

* Wird ein Schlüssel erkannt, wird nur das Gültig-Bis-Datum entfernt (Schlüssel ist wieder aktiv). Das gilt auch, wenn der Schlüsselwert mehrfach im Verzeichnis existiert.
* Wird ein Schlüssel nicht im Verzeichnis erkannt, wird er eingelesen und aktiv gesetzt.
Als Ergebnis haben Sie damit nur die korrekten Schlüssel als aktive Werte markiert. Verkehrte, aber bereits verwendete Schlüssel, bleiben in der Datenbank bestehen, werden aber als inaktiv gekennzeichnet.

> #### warning::Wichtig!
>
>**Was wird verändert?** Bei bestehenden Schlüsselzeilen in den Zielverzeichnissen wird weder Bezeichnung, noch Kürzel oder Schlüssel verändert, lediglich das Gültig-von- und das Gültig-bis-Datum wird angepasst.
>
>**Vom Importkatalog wird nur die erste Zeile eingelesen?** Dann fehlen vermutlich die Schlüssel in der Datei. Die erste Zeile wird eingelesen, alle nachkommenden Zeilen werden anhand des Kürzels und des Schlüssels geprüft und erst dann eingelesen. 
Dabei zählt der Schlüssel vor dem Kürzel, im neuen Schlüssel und in der ersten bereits eingelesenen Zeile ist der Schlüssel leer, das wird als gleicher Wert erkannt, daher wird der Import der zweiten und aller weiteren Zeilen übersprungen.
Lösung: bitte die Kürzelwerte auch als Schlüsselwerte für den Importkatalog einfügen.
>
>**Kuerzel:** dieser Wert muss pro Zeile gefüllt werden, darf aber nur einmalig innerhalb eines Verzeichnisses verwendet werden.Zeichenlänge pro Feld: Die Gesamtzeichenlänge darf nicht überschritten werden.




### Postleitzahlverzeichnis importieren

Mit der Option „Postleitzahlverzeichnis importieren“ können Sie ein bestehendes Postleitzahlverzeichnis gegen ein neues (z.B. einer anderen Schule) austauschen oder eine leeres Postleitzahlenverzeichnis füllen. Bitte lesen Sie dazu den Abschnitt „Postleitzahl- und Schlüsselverzeichnisse importieren“ auf der Seite 35.

## Datenexporte

Über „Ansicht“ und „Datenexporte“ gelangen Sie zu den Export-Möglichkeiten von MAGELLAN.

### Postleitzahlverzeichnis exportieren

Um ein Postleitzahlverzeichnis zu exportieren, müssen Sie die Option „Postleitzahlverzeichnis exportieren“ anwählen. Sie können so das Postleitzahlverzeichnis einer MAGELLAN-Datenbank in eine andere MAGELLAN-Datenbank übernehmen.

### Mach exportieren

Diese Funktion ermöglich die Übergabe ausgewählter Daten an die Mach-Schnittstelle.

## Access-Anbindung an die Firebird-Datenbank

### Grundlagen

Möchten Sie Bescheinigungen, Listen oder Zeugnisse drucken, so bietet Ihnen MAGELLAN standardmäßig die Ausdruckmöglichkeit über Crystal Reports an. 
Alternativ können Sie auch Abfragen oder Berichte unter Microsoft Access erstellen. Hierzu müssen Sie auf Basis einer ODBC-Verbindung eine Verknüpfung zwischen Access und der Firebird-Datenbank herstellen, um mit Access auf die Daten zugreifen zu können. Für Access müssen die folgenden Schritte berücksichtigen, die in den nachfolgenden Abschnitten dieses Kapitels ausführlich erläutert werden:

1. Schritt: Erstellen einer ODBC-Verbindung zu Firebird-Datenbank
2. Schritt: Ein neue Access-Datenbank anlegen
3. Schritt: Berichte erstellen



> #### success::Wichtig
>
> Um einen unbefugten Zugriff per Access auf die MAGELLAN-Datenbank zu verhindern, muss auf die Anzahl der Benutzer von Access bereits über das Betriebssystem eingeschränkt werden.

### 1. Schritt: ODBC-Verbindung zur Firebird-Datenbank erstellen

Um eine ODBC-Verbindung zu erstellen, müssen Sie über die Systemsteuerung Ihres Rechners eine neue ODBC-Datenquelle einrichten.

Unter Windows NT/Windows 2000 gehen Sie dazu wie folgt vor:

1. Öffnen Sie das Windows-Startmenü.

2. Klicken Sie auf Systemsteuerung.

3. Klicken Sie auf Verwaltung.

4. Klicken Sie auf Datenquellen ODBC.

Unter Windows 95/98/ME gehen Sie dazu wie folgt vor:

1. Öffnen Sie das Windows-Startmenü.

2. Klicken Sie auf Systemsteuerung.

3. Klicken Sie auf ODBC Datenquellen 32-Bit.
Abbildung 256: Dialogfenster „ODBC-Datenquellen-Administrator“

![ODBC-Datenquellen-Administrator](/images/Import_Export.ODBC2.png)

Im Dialogfenster „ODBC-Datenquellen-Administrator“ können Sie nun unterschiedliche Möglichkeiten wählen, um eine ODBC-Verbindung aufzubauen.

#### Benutzerabhängige ODBC-Datenquelle

Bei der benutzerabhängigen ODBC-Datenquelle wird die Einrichtung pro Benutzer abgespeichert. Sie müssen pro MAGELLAN-Benutzer auf dem Rechner die Einrichtung vornehmen. Sie haben den Vorteil, dass Sie in diesem Fall auch die in MAGELLAN eingetragenen Kennungen direkt mit abspeichern können. Beim Aufruf der Access-Berichte müssen Sie dann nicht mehr die Kennungen pro Benutzer ändern.

1. Klicken Sie im Dialogfenster ODBC-Datenquellen-Administrator auf die Registerkarte Benutzer-DSN.

2. Klicken Sie auf Hinzufügen.

3. Wählen Sie im Dialogfenster Neue Datenquelle erstellen den Namen „Firebird/InterBase(r) driver“ aus und klicken Sie dann auf Fertigstellen.

4. Füllen Sie im Dialogfenster „Firebird ODBC Setup“ mindestens die folgenden Felder aus:

* **DSN:** Geben Sie hier eine freie festzulegenden Namen für Ihre ODBC-verbindung an. Für die weiteren Betrachtungen wählen wir hier die Bezeichnung „MAGELLANAccess“.

* **Database:** Hier geben Sie den lokalen Pfad der MAGELLAN-Datenbank an, analog zur Installation von MAGELLAN. Dies ist entweder der lokale Pfad der MAGELLAN-Datenbank auf Ihrem Einzelplatzrechner (z.B. LOCALHOST:C:\Users\Public\Documents\Stueber Software\MAGELLAN 6\Datenbank\MAGELLAN6.fdb) oder der lokale Pfad des Servers inkl. Servernamen der MAGELLAN-Datenbank auf einer Arbeitsstation im Netzwerk (z.B. MeinServer: C:\Users\Public\Documents\Stueber Software\MAGELLAN 6\Datenbank\MAGELLAN6.fdb)

* **Client:** Hier geben Sie bitte den folgenden Pfad zur Treiberdatei fbclient.dll an (C:\WINDOWS\system32\fbclient.dll)
Database Account: Hier können Sie einen Benutzer aus der Benutzerverwaltung von MAGELLAN angeben. Standardmäßig ist dies „sysdba“. Geben Sie hier keinen Wert an, werden Sie beim ersten Aufruf eines Access-Berichtes aus MAGELLAN automatisch nach dem Benutzer gefragt.

* **Password:** Hier können Sie ein zum Benutzer passendes Kennwort aus der Benutzerverwaltung von MAGELLAN angeben, der das Recht zum Drucken hat. Standardmäßig ist dies „masterkey“ für den Benutzer „sysdba“. Geben Sie hier keinen Wert an, werden Sie beim ersten Aufruf eines Access-Berichtes aus MAGELLAN automatisch nach dem Kennwort gefragt.

* **Character Set: **Hier müssen Sie den Zeichensatz WIN1251 einstellen.


![Das Dialogfenster „FirebirdODBC Setup“](/images/fb-odbc.png) 

### 2. Schritt: Neue Access-Datenbank anlegen

Nachdem Sie die ODBC-Verbindung im ersten Schritt erstellt haben, müssen Sie jetzt eine Access-Datenbank anlegen, welche mit der neuen ODBC-Verbindung eine Verknüpfung zur MAGELLAN-Datenbank aufbaut. Die Vorgehensweise wird exemplarisch unter Microsoft Access 2000 vorgestellt:

1. Starten Sie Microsoft Access.

2. Klicken Sie auf `Datei` und dann auf `Neu`.

3. Wählen Sie im Dialog `Neu` auf der Registerkarte `Allgemein `die Option `Datenbank` und klicken Sie dann auf `OK`.

4. Speichern Sie die neue Datenbank unter einem Namen ab, z.B. unter` C:\Stueber Software\MAGELLAN 6\Datenbank\MAGELLAN6.mdb`.

5. Wählen Sie unter `Objekte `den Bereich `Tabellen`. Hier sind noch keine Tabellen eingetragen.

6. Klicken Sie im weißen Bereich der Anzeigefläche der Tabellen auf die rechte Maustaste und klicken Sie dann auf `Tabellen verknüpfen`.

7. Wählen Sie im Dialogfenster `Verknüpfen `den Dateityp `ODBC Databases ()` aus.

8. Wählen Sie im Dialogfenster `Datenquelle `auswählen die neu definierte Datenquelle `MAGELLANAccess` auf der Registerkarte `Computerdatenquellen` aus.

9. Im Dialogfenster `Tabellen verknüpfen` werden Ihnen jetzt alle Tabellen der MAGELLAN-Datenbank zur Auswahl angeboten. Markieren Sie hier durch Mehrfachmarkierung alle Tabellen, die nicht den Präfix „tbl“ (z.B. tblLehrer) besitzen. Wenn Sie das Kennwort der ODBC-Verbindung nicht bei jedem Aufruf eines Access-Berichts später eingeben wollen, müssen Sie zusätzlich das Optionsfeld `Kennwort speichern` anwählen. Klicken Sie abschließend auf `OK`.

Während der Erstellung der Tabellenverknüpfungen werden Sie bei einigen Tabellen aufgefordert, eindeutige Datensatzbezeichner auszuwählen. Hier können Sie jeweils auf `Abbrechen `klicken, da diese Einstellungen für das Drucken nicht relevant sind.

Die Access-Datenbank MAGELLAN6.mdb ist jetzt erstellt und besitzt über die Tabellen einen direkten Zugriff auf die originale Firebird MAGELLAN-Datenbank MAGELLAN6.fdb.

> #### danger::Achtung!
>
>  Beim Erstellen der Verknüpfungen zu der Tabelle „Schueler“ unter Microsoft Access erhalten Sie von Access die Rückmeldung, dass eine Verknüpfung nicht möglich ist. Die Tabellen „Schueler“ und „Lehrer“ enthalten mehr als 32 Datenbankindizes. Microsoft Access kann maximal 32 Datenbankindizes verarbeiten. Eine Verknüpfung über den von uns mitgelieferten aktuellen Firebird Open Source Treiber erzeugt daher die korrekte Fehlermeldung. Sie können in der MAGELLAN-Datenbank anstelle der Tabellen „Schueler“ bzw. „Lehrer“ das View „Schueler2“ bzw. „Lehrer2“ verwenden. Beim Verknüpfen von Views werden in Access keine Indizes erzeugt, so dass es keine Probleme mehr gibt. Die beiden View „Schueler2“ bzw. „Lehrer2“ verweisen auf alle Felder der Tabelle „Schueler“ bzw. „Lehrer“.



### 3. Schritt: Berichte in der Access-Datenbank anlegen

In der neu erzeugten Access-Datenbank können Sie jetzt entsprechende Abfragen oder Berichte erstellen. Grundlage für die Erstellung ist die MAGELLAN-Datenbankstruktur, welche ausführlich im elektronischen Dokument „MAGELLAN-Datenstruktur.pdf“ beschrieben ist. Dieses Dokument können Sie unter support@stueber.de anfordern. Zur Erstellung von Berichten unter Access ist auf die umfangreiche Literatur zum Thema Access zu verweisen.

