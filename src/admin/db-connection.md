# Datenbank und Verbindungen

Dieses Kapitel richtet sich an Administratoren und soll einen Einblick in die MAGELLAN-Administration geben. Dazu werden der MAGELLAN-Administrator, das Versetzen in einen anderen Mandanten, das MyMAGELLAN Center, die Access-Anbindung, das Einspielen von Update, der MAGELLAN-DWH Explorer, der MAGELLAN-Skripteditor, das Ein- bzw. Ausblenden von Bereichen und anderes näher erläutert. Der MAGELLAN-Administrator beinhaltet folgende Funktionen für den Administrator:

* Server-Verwaltung
* Datenbankpflege
* Datensicherung


So starten Sie den MAGELLAN-Administrator :

1. Klicken Sie auf Start, dann auf Programme und dann auf STÜBER SYSTEMS.

2. Klicken Sie auf MAGELLAN 6 Administrator.

3. Tippen Sie Ihre Kennung und Ihr Kennwort ein und bestätigen Sie mit OK (Wenn Sie MAGELLAN neu installiert haben, dann tippen Sie unter Kennung „sysdba“ und das Kennwort „masterkey“ ein).

> #### warning::Wichtig
> Sie können sich nur als Administrator im MAGELLAN-Administrator anmelden.

## Server-Verwaltung

Die Server-Verwaltung starten Sie, indem Sie auf Ansicht und dann auf Server-Verwaltung klicken.

### Verbindungen verwalten

Über die Option Datenbank verwalten können Sie Ihre Datenbank registrieren. Sie haben hier die Möglichkeit, mehrere Verbindungen zu MAGELLAN-Datenbanken zu registrieren. Jeder Verbindung können Sie einen individuellen Namen mit der Verknüpfung zu einer MAGELLAN-Datenbank zuordnen. Sie haben so z.B. die Möglichkeit, zwischen mehreren MAGELLAN-Datenbanken zu wechseln ohne die Daten kopieren zu müssen. Im Fenster Verbindungen verwalten können Sie einerseits eine bereits bestehende Verbindung bearbeiten und andererseits eine neue Verbindung anlegen. Möchten Sie eine existierende Datenbankverbindung editieren, markieren Sie diese bitte in der Liste der registrierten Verbindungen und klicken auf die Schaltfläche Bearbeiten. Das Fenster Verbindung registrierten ist unterteilt in fünf Registerkarten.


* **Allgemein:** Auf der Registerkarte Allgemein kann man einen Alias hinterlegen, also eine Bezeichnung nach Wunsch. Man kennt dies von der Umwandlung einer offiziellen E-Mail-Adresse eines Internetproviders in einen E-Mail-Alias-Namen, der auch oft als Nickname bezeichnet wird. Bei der Anmeldung in MAGELLAN müssen Sie unter Datenbank nur noch den Alias-Namen der Verbindung einstellen, mit der MAGELLAN gestartet werden soll.

![Unterkarte "Allgemein"](/images/db_verbindung0.png)

![Nach der Registrierung weiterer Datenbankverbindungen können Sie diese bei der MAGELLAN-Anmeldung unter „Datenbank“ auswählen.](/images/db_mag_anmeldung.png)

So haben Sie die Möglichkeit, einfach zwischen mehreren MAGELLAN-Datenbanken zu wechseln. Dies ist z.B. vorteilhaft, wenn Sie Statistiken erstellen müssen. Andererseits kann es auch nützlich sein, eine Übungsdatenbank für neue Mitarbeiter anzulegen.

* **Datenbank:** Auf der Registerkarte „Datenbank“ wird im Feld „Protokoll“ der Wert „Lokal“ ausgewählt, wenn es sich um eine Einzelplatz- bzw. Serverinstallation handelt. Liegt hingegen eine Clientinstallation vor, tragen Sie hier „TCP/IP“ ein. In diesem Fall muss dann auch im Feld „Server“ mit dem Lupensymbol der Explorer geöffnet werden und die Serverbezeichnung ausgewählt werden. Im Feld „Dateipfad auf dem Server“ wird der lokale Pfad auf dem Server hinterlegt. Eine bekannte Fehlerquelle ist, dass man hier versehentlich einen Netzwerkpfad hinterlegt. Wichtig ist, dass hier auch bei einer Clientinstallation der lokale Pfad auf dem Server angegeben wird.

![Unterkarte "Datenbank"](/images/db_verbindung1.png)

* **Data Warehouse:** Auf der Registerkarte „Data Warehouse“ ist der lokale Pfad auf dem Server anzugeben, wo die Datawarehouse-Datenbank abgelegt ist. Dies gilt für Einzelplatz- bzw. Serverinstallation ebenso wie für Clientinstallation.

![Unterkarte "Data Warehouse"](/images/db_verbindung2.png)


* ** Datenordner:** Auf der Registerkarte „Datenordner“ können Sie für die Ordner „Dokumente“, „Skripte“, „Berichte“, „Vorlagen“ sowie „Importe“ mittels der Lupensymbole jeweils den Explorer öffnen und den entsprechenden Pfad aussuchen, wo diese Ordner abgelegt wurden. Arbeiten Sie an Ihrer Schule im Netzwerk, ist es wahrscheinlich, dass alle diese Datenordner auf dem Server liegen und auch alle User auf die Dokumente auf dem Server zugreifen sollen. Es gibt aber dennoch die Möglichkeit, hier auf andere Datenordner zuzugreifen, beispielsweise auf lokal liegende.

![Unterkarte "Datenordner"](/images/db_verbindung3.png)


Möchten Sie eine neue Datenbankverbindung einrichten, klicken Sie bitte in der Liste der registrierten Verbindungen auf die Schaltfläche `Hinzufügen`. Das Fenster Verbindung registrierten öffnet sich. Bei der Eingabe ist so zu verfahren als wenn man eine bestehende Verbindung bearbeitet. Hat man die Eingabe beendet, steht in der Liste der registrierten Verbindungen diese neue Verbindung zur Auswahl. 

Hat man sich nun mehrere Datenbankverbindungen angelegt, ist es sinnvoll, einen Standard-Alias zu hinterlegen im Auswahlfeld `Standard-Alias` für die MAGELLAN-Anmeldung. Diese dort eingetragene MAGELLAN-Verbindung wird dann beim Programmstart im Anmeldefenster voreingestellt.

### Verbindungen testen

Mit der Option Verbindungen testen können Sie eine eingestellte MAGELLAN- und Netzwerk-Verbindung testen, die Sie zuvor unter Datenbank verwalten eingerichtet haben. Im Fenster Verbindungen testen geben Sie auf der Registerkarte Datenbank-Verbindung zunächst der MAGELLAN-Alias-Name ein. Auch das entsprechende Protokoll und für den Fall, dass es sich um eine Clientinstallation handelt, der Servername müssen ausgewählt werden. Melden Sie sich bitte mit Benutzer und Kennwort an und klicken auf die Schaltfläche Testen. Im Fenster Ergebnis erhalten Sie ein Protokoll über den Testlauf. Wird Ihnen eine Fehlermeldung angezeigt, sollten Sie Ihre Eingaben noch einmal überprüfen.

## Die Paths-Datei

Beim Start von MAGELLAN werden Informationen aus Dateien gelesen. Diese Dateien werden an einem betriebssystemspezifischen Ort pro Installation erwartet oder MAGELLAN liest den Inhalt der Paths-Datei (MAGELLAN.paths) aus.

Der Vorteil einer Paths-Datei ist, dass Sie mehreren Nutzern die identischen Einstellungen in einem Arbeitsschritt an einem zentralen Ort zur Verfügung stellen können. Beim Einrichten einer neuen Arbeitsplatzinstallation genügt es die Installation durchzuführen und die MAGELLAN.paths im Programmverzeichnis abzulegen.

Folgende Dateien werden beim Programmstart gelesen:

Datei | Inhalt
------------ | ------
MAGELLAN.lic | enthält die Lizenzierungsdaten
MAGELLAN.opt |	enthält die MAGELLAN-Optionseinstellungen
MagInv.opt |	enthält die MAGELLAN-Haushalt&Inventar-Optionseinstellungen
MagBib.opt |	enthält die MAGELLAN-Bibliothek-Optionseinstellungen
MAGELLAN.evm |	enthält die Pfade zur Datenbank und den Datenordnern

Diese Dateien liegen je nach Betriebssystem an folgenden voreingestellten Speicherorten:

Betriebssystem | Pfad
------------------- | ----
Windows 2000 | C:\Dokumente und Einstellungen\All Users\Anwendungsdaten\Stueber Software\MAGELLAN 6
XP | C:\Dokumente und Einstellungen\All Users\Anwendungsdaten\Stueber Software\MAGELLAN 6
Vista | C:\ProgramData\Stueber Software\MAGELLAN 6
Windows 7/8 | C:\ProgramData\Stueber Software\MAGELLAN 6
Windows Server 2008 | C:\ProgramData\Stueber Software\MAGELLAN 6

Möchten Sie abweichende Speicherorte für diese Dateien angeben, zum Beispiel damit alle MAGELLAN-Arbeitsplatzinstallationen auf dieselben Dateien zugreifen, sind folgende Schritte nötig:

1. Richten Sie einen Arbeitsplatz bitte vollständig ein, damit von diesem Arbeitsplatz die Dateien MAGELLAN.evm, MAGELLAN.lic und die Optionsdateien kopiert werden können.

2. Wählen Sie einen Speicherort für die Konfigurationsdateien aus. Die Dateien können in einem gemeinsamen Verzeichnis liegen oder Sie wählen für MAGELLAN.evm, MAGELLAN.lic und die Optionsdateien (MAGELLAN.opt, MagInv.opt, MagBib.opt) drei getrennte Verzeichnisse und speichern dort die Dateien.

3. Erstellen Sie mit einem Texteditor eine neue Textdatei und kopieren den nachfolgenden Text in diese Datei. Passen Sie die Pfade bitte auf Ihre angelegten Verzeichnisse an, diese können sich lokal auf dem Rechner oder in Ihrem Netzwerk befinden.

Beispiel:

```` xml
<?xml version="1.0" encoding="UTF-8" standalone="yes"?>
<Preferences>
<Paths>
<Entry Name="MAGELLANEnvironmentFolder" Value="D:\Mein Verzeichnis"/>
<Entry Name="MAGELLANOptionsFolder" Value="D:\Mein Verzeichnis"/>
<Entry Name="MAGELLANLicenseFolder" Value="D:\Mein Verzeichnis"/>
</Paths>
</Preferences>
````

4. Speichern Sie diese Textdatei und benennen die Datei anschließend in „MAGELLAN.paths“ um.

5. Legen Sie diese Datei pro Arbeitsplatzinstallation im Programmverzeichnis ab. Beim Programmstart von MAGELLAN wird geprüft, ob sich eine Datei mit diesem Namen im Programmverzeichnis befindet und gegebenenfalls ausgelesen.

## Datenbankpflege

Die Datenbankpflege starten Sie, indem Sie auf `Ansicht` und dann auf `Datenbankpflege` klicken.

### Datenbank konfigurieren

Die Option Datenbank konfigurieren ermöglicht Ihnen die individuelle Anpassung der Eigenschaften Ihrer Datenbank. Sie können hier einen allgemeinen Schreibschutz festlegen und die Art der Zwischenspeicherung beeinflussen.

### Datenbank überprüfen

Aktion|Bemerkung
--|--
Generatoren synchronisieren| Mit der Option „Datenbank prüfen“ können Sie die „Generatoren synchronisieren“. Die ID-Nr.-Vergabe im Programm geschieht durch besagte Generatoren und wird ohne Einflussmöglichkeit automatisch fortlaufend generiert. Bearbeitet man allerdings die Datenbank manuell über ein bestimmtes Werkzeug, d.h. fügt IDs hinzu, funktioniert das automatische Hochzählen des Generators an dieser Stelle eventuell nicht mehr. <br/><br/>Beispiel: <br/>Man hat Schüler neu angelegt. Der Generator hat die Schüler-IDs 1-10 vergeben. Nun aber bearbeiten Sie die Firebird-Datenbank mit einem dafür geeigneten Programm, z.B. „EMS IB Manager for Firebird“. Sie tragen in diesem Programm in Ihre MAGELLAN-Datenbank einen Schüler ein und vergeben für diesen die ID 11. Wenn Sie nun MAGELLAN aufrufen und dort weiterhin Schüler neu erfassen möchten, wird eine Fehlermeldung auftreten. Der Grund hierfür ist, dass die MAGELLAN-Generatoren korrekterweise bei ID 10 stehen und nun als nächste ID die Nummer 11 vergeben möchten. Diese ID existiert aber bereits in der Datenbank. Die Generatoren synchronisiert man also dann, wenn man händisch in der Datenbankstruktur ID-Eintragungen vorgenommen hat. 
Zugriffsrechte synchronisieren| Ein weiterer Punkt lautet „Zugriffsrechte synchronisieren“. Dies ist erforderlich, wenn man die MAGELLAN-Datenbank „MAGELLAN6.fdb“ mit der Benutzer-Datenbank synchronisieren möchte. Die im Programm angelegten Benutzerdaten, die Sie im MAGELLAN-Administrator definieren können, werden nicht komplett in der MAGELLAN-Datenbank MAGELLAN6.fdb gespeichert, sondern sie werden auch in der Datenbank C:\Programme\Firebird\Firebird_2_0\security2.fdb (Standardordner für Firebird 2) auf dem Server gespeichert. Wenn man die MAGELLAN-Datenbank mitsamt den Benutzerrechten auf einem anderen Rechner nutzen will, muss man diese Firebird-Datenbank mit kopieren und auf dem neuen Rechner über das Administratoren-Tool die Zugriffsrechte synchronisieren. Dann kann man wieder mit den angelegten Benutzern weiterarbeiten.
Anrede setzen|Setzt für Schüler, Bewerber, Lehrer und Personen die Anrede anhand des Geschlechtes auf Herr oder Frau, wenn das Geschlecht gesetzt ist. Es werden nur noch nicht vorhandene Anreden gesetzt. 
Gemeinden synchronisieren|Setzt für Schüler, Betriebe, Lehrer udn SChulen die Gemeindekennziffern anhand der PLZ und des Orts, wenn diese Angaben nicht zu mehreren Gemeinden führen. Es werden nur noch nicht vorhandene Gemeinde gesetzt.
Klassenzeiträume korrigieren|Korrigiert Klassenzeiträume die gegebenenfalls  durch den Import z.b. von Daten aus IBIS in bestimmten Zeiträumen keinerlei Schüler enthalten. Diese überflüssigen Daten werden herausgefiltert und gelöscht.
Unterstriche in Schülernamen entfernen|Entfern beim Vornamen der Schüler Unterstriche, die gegebenenfalls duch den Import mit hineingekommen sind.
Schüler-Passfotos löschen|Sie können alle Passbilder der inaktiven Schüler aus der Datenbank (aller Schüler, aller Zeiträume, aller Mandanten) entfernen. Die Größe der Datenbank reduziert sich nach dem Sichern und Wiederherstellen Ihrer Datenbank.
Barcodes generieren|Es werden Barcodes für dei neuen Barcodefelder bei Schüler, Lehrer und Personen generiert. Diese Funktion betrifft nur Datensätze, die noch keine Barcodes haben. Barcodes werden in MAGELLAN ab der Einführung der Funktion automatisch für neue Datensätze angelegt, Sie haben so die Möglichkeit für Bestandsdaten die Barcodes nachträglich zu erzeugen.




### Datenbankinhalt löschen

Um die bestehende Datenbank zu leeren, können Sie die Option „Datenbank löschen“ wählen. Die Option benötigen Sie insbesondere, wenn Sie die Daten in der standardmäßig mitgelieferten Beispiel-Datenbank durch die Eingabe eigener Daten ersetzen wollen.

> info::Tipp
> Beim Neueinstieg in MAGELLAN sollten Sie bitte die Schlüsselverzeichnisse und auf das Postleitzahlverzeichnis mit leeren, damit Sie im Anschluss diese Verzeichnisse mit den aktuellen Werten für Ihr Bundesland und Ihre Schulart füllen können.

Nach dem Leeren werden automatisch die ID-Generatoren der Datenbanktabellen zurückgesetzt, damit der erste neue Schüler als Beispiel mit der ID 1 angelegt werden kann.

### Beispieldaten aktualisieren

Mit dieser Funktion können Sie die Datumsangaben der Beispieldaten Ihrer Datenbank auf das aktuelle Jahr aktualisieren.

### Firebird 1.5/2.1 Sicherheitsdatenbank konvertieren

Wenn Sie in der Version 5 (Firebird 1.5) oder in der Version 6 (Firebird 2.1) eine Sicherungskopie mit dem Punkt „Sicherungskopie erstellen Ihrer Passwortdatenbank (security.fdb) erzeugt haben, können Sie die dabei erzeugt security.fbk mit dieser Aktion konvertieren. Bei der Konvertierung wird die Datenstruktur der Passwortdatenbank auf das ab Firebird 2.5 gültige Format verändert. Führen Sie anschließend bitte den Punkt Datenbankpflege|Datenbank überprüfen|Zugriffsrechte synchronisieren aus, anschließend können sich die Nutzer mit den gewohnten Zugängen an der Datenbank anmelden.

### Mandanten kopieren

Um alle mandantenbezogenen Daten eines Mandanten aus einer MAGELLAN-Datenbank A (=Ausgangsdatenbank) in eine MAGELLAN-Datenbank B (=Zieldatenbank) zu kopieren, gehen Sie wie folgt vor:

1. Starten Sie den MAGELLAN-Administrator, indem Sie das Windows-Startmenü öffnen und dann auf Programme|STÜBER SYSTEMS|MAGELLAN 6 Administrator klicken.

2. Wählen Sie Datenbankpflege und klicken Sie dort auf Mandanten kopieren.

3. Klicken Sie im Assistenten auf Weiter.

4. Wählen Sie den zu kopierenden Mandaten der Ausgangdatenbank aus. Geben Sie anschließend die Verbindungsdaten die Zieldatenbank an und klicken Sie dann auf Weiter.

5. Klicken Sie auf Start um mit dem Kopiervorgang zu beginnen.

Vor dem Kopieren der mandantenbezogen Daten in eine andere MAGELLAN-Datenbank müssen folgenden Voraussetzungen erfüllt sein:

* Ausgangs- und Zieldatenbank müssen die gleichen Zeiträume besitzen.
* Der zu kopierenden Mandant darf noch nicht in der Zieldatenbank existieren.
* Das Kürzel des zu kopierenden Mandanten darf noch nicht als Kürzel für einen Mandanten der Zieldatenbank verwendet worden sein.

> info::Hinweis
> Über die Funktion „Mandanten kopieren“ können Sie die Inhalte zweier Mandanten aus verschieden MAGELLAN-Datenbanken zu einer einzigen MAGELLAN-Datenbank mit zwei Mandanten zusammenführen. Auf diese Weise können beispielweise zwei Schulen mit bisher getrennt arbeitenden MAGELLAN-Datenbanken auf einer einzigen MAGELLAN-Datenbank arbeiten und die Vorteile einer SchoolCentral-Lösung nutzen.

### Bundesland ändern

Um das im Rahmen der Installation über den Willkommensassistenten eingestellt Bundesland nachträglich zu verändern, können Sie hier optional ein anderes Bundesland auswählen.

## Datensicherung


Über „Ansicht“ und „Datensicherung“ kommen Sie zu den Datensicherungsmöglichkeiten in MAGELLAN. In dieser Funktion wird das Sicherungstool der Firebird-Datenbank ausgeführt. Sie können mit diesem Tool Sicherungskopien der Schulverwaltungsdatenbank (MAGELLAN.fdb) und der Datawarehouse-Datenbank (MAGELLANDWH.fdb) erstellen.

> #### danger::Achtung!
>
> Wir empfehlen eine tägliche Sicherung Ihrer Datenbank! Bitte verwenden Sie dazu den entsprechenden Punkt im MAGELLAN-ADMINISTRATOR oder den unten beschriebenen Weg per Windows Taskplaner. Diese von Firebird mit angebotene Funktion kann auch erfolgen, während der Firebird-Dienst läuft und MAGELLAN verwendet wird. Es werden die Daten Ihrer MAGELLAN.fdb in eine neue Datei mit der Endung *.fbk geschrieben, hieraus kann eine neue Datenbank aufgebaut werden. Anders als bei einer Sicherung per Kopie der Datenbank (die nie bei laufendem Firebird-Dienst erfolgen darf) erhalten Sie Rückmeldungen zur Qualität der gesicherten Daten.
> Sie sollten in Abständen, zum Beispiel vierteljährlich, mit einer wiederhergestellten Datenbank weiterarbeiten. Dazu stoppen Sie den Firebird-Server-Manager in der Systemsteuerung Ihres Serverrechners, tauschen die Datenbanken (z.B. C:\Users\Public\Documents\Stueber Software\MAGELLAN 6\Datenbank) aus und starten den Firebird-Server-Manager erneut.
>
> Das Herstellen einer Sicherungskopie und anschließende Wiederherstellen dieser Sicherungskopie hat eine reparierende und zugleich komprimierende Funktion. Die wiederhergestellte Sicherungskopie ist stets kleiner als die Ausgangsdatenbank, da Lücken in der Datenbank beseitigt werden und so die Datenmenge „abgespeckt“ wird.

### Aufruf  "Firebird Sicherheitsdatenbank 2.1/2.5" 
(nur bis Ausgabe 6.5.0)

Dieser Aufruf wird ausschließlich für Sicherungen der Passwortdatenbank (security.fdb oder security2.fdb) als Voraussetzung für den Versionswechsel von Firebird (von 1.5 auf 2.1 und vorn 2.1 auf 2.5) benötigt. 
 
Weitere Informationen finden Sie in der Dokumentation für den [Umstieg von MAGELLAN 5 auf MAGELLAN 6](https://doc.magellan6.stueber.de/installation/umstieg-von-5-auf-6.html) und in den Anleitungen zur [Aktualisierung von Firebird](https://doc.magellan6.stueber.de/installation/firebird-aktualisieren.html).
![](/images/db.sicherheitsdatenbank_sichern.png)

### Sicherungskopie erstellen

Der nachstehend beschriebene Assistent kann eine Sicherung Ihrer Datenbank erstellen. 

![Sicherung einer Datenbank](/images/sicherung/sicherungskopie.herstellen.png)


Wir beschreiben in der nachstehenden Tabelle die Eingabeoptionen:

Gruppe|Feld|Bedeutung
---|---|---
Verbindung|Welche Verbindung soll gesichert werden?|Es wird Ihnen eine Liste Ihrer unter Server-Verwaltung angelegten Datenbankanbindungen gezeigt. Mit der Auswahl der Verbindung, wählen Sie auch die der Verbindung zugeordnete Datenbank aus, die Felder unter dem Punkt "Datenbank" werden automatisch aus den Verbindungsinformationen gefüllt.
Datenbank|Protokoll|wird aus den Einstellungen der unter Server-Verwaltung angelegten und im Schritt zuvor ausgewählten Verbindung befüllt
Datenbank|Server|wird aus den Einstellungen der unter Server-Verwaltung angelegten und im Schritt zuvor ausgewählten Verbindung befüllt
Datenbank|Datei|wird aus den Einstellungen der unter Server-Verwaltung angelegten und im Schritt zuvor ausgewählten Verbindung befüllt
Anmeldung|Benutzer|Tragen Sie bitte die sysdba-Kennung ein!
Anmeldung|Kennwort|Tragen Sie bitte Ihr sysdba-Passwort ein!
Sicherung|Sicherung|Tragen Sie hier bitte einen lokalen Pfad auf Ihrem MAGELLAN-Server ein, damit dort die Sicherungskopie erzeugt werden kann. Wir empfehlen die Sicherung in das Backupverzeichnis im Datenbankordner abzulegen. <br/>Der Pfad könnte dafür wie folgt aussehen:<br/>`C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup`<br/><br/>Der Name der Sicherung wird vom Programm ergänzt und beinhaltet: <br/>` [Datum, Uhrzeit]Verbindungsname - Benutzer.fbk`<br/> Beispiel: <br/>[2017-06-26, 14-07-16] Magellan.local - sysdba.fbk<br/><br/>Wenn Sie das Modul MAGELLAN ADMINISTRATOR auf dem MAGELLAN-Server aufrufen, steht Ihnen die Schaltfläche zur Auswahl per Datenexplorer zur Verfügung.
Fortschrittsanzeige|Fortschrittsanzeige|Setzen Sie das Häkchen um detaillierte Auskunft über die Sicherung zu erhalten. Ohne Häkchen erfolgt die Sicherung um ein Vielfaches schneller!
Ergebnis|Ergebnis|In diesem Feld erhalten Sie eine Rückmeldung über gewählte Aktion!

### Sicherungskopie wiederherstellen

Der nachstehend beschriebene Assistent kann aus einer Sicherung Ihrer Datenbank eine neue Datenbankdatei aufbauen. 

![Sicherung einer Datenbank wiederherstellen](/images/sicherung/sicherungskopie.wiederherstellen.png)


Wir beschreiben in der nachstehenden Tabelle die Eingabeoptionen:




Gruppe|Feld|Bedeutung
---|---|---
Verbindung|Verbindung|Um eine Sicherung wiederherstellen zu können, muss eine Firebirdserver zur Verfügung stehen. Diesen wählen Sie indirekt mit der Verbindung aus. Welche Sicherung wirklich wiederhergestellt werden soll, legen Sie im Bereich Sicherung fest.<br/> Mit der Auswahl der Verbindung, wählen Sie auch die der Verbindung zugeordnete Datenbank aus, die folgenden Felder werden automatisch aus den Verbindungsinformationen gefüllt.
Datenbank|Protokoll|wird aus den Einstellungen der unter Server-Verwaltung angelegten und im Schritt zuvor ausgewählten Verbindung befüllt
Datenbank|Server|wird aus den Einstellungen der unter Server-Verwaltung angelegten und im Schritt zuvor ausgewählten Verbindung befüllt
Datenbank|Datei|wird aus den Einstellungen der unter Server-Verwaltung angelegten und im Schritt zuvor ausgewählten Verbindung befüllt
Anmeldung|Benutzer|Tragen Sie bitte die sysdba-Kennung ein!
Anmeldung|Kennwort|Tragen Sie bitte Ihr sysdba-Passwort ein!
Sicherung|Sicherung|Tragen Sie bitte den Pfad zu Ihrer wiederherzustellenden Sicherungsdatei ein!<br/>Beispiel: `C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup\[2017-06-26, 14-07-16] Magellan.local - sysdba.fbk`
Sicherung|Wiederherstellung|Tragen Sie bitte einen lokalen Pfad auf Ihrem MAGELLAN-Server ein, der Dateiname der neuen Datenbank wird vom Programm ergänzt!<br/> Sie können auf diesem Weg keine bestehende Datenbank überschreiben, bitte wählen Sie eine noch nicht verwendete Bezeichnung! <br/>Beispiel: `C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup\neu.MAGELLAN6.fdb`
Fortschrittsanzeige|Fortschrittsanzeige|Setzen Sie das Häkchen um detaillierte Auskunft über die Sicherung zu erhalten. Ohne Häkchen erfolgt die Sicherung um ein Vielfaches schneller!
Ergebnis|Ergebnis|In diesem Feld erhalten Sie eine Rückmeldung über gewählte Aktion!




> #### primary::Hinweis
>
>  Wenn Sie von einem Client aus die Sicherung der Datenbank auf dem Server durchführen, haben Sie nicht die Möglichkeit, durch Anklicken des Lupensymbols (Schaltfläche mit den drei Punkten) den Pfad auszusuchen. Sie können lediglich manuell den entsprechenden Pfad eintragen. 
Wenn keinen Speicherort und keinen Dateityp angeben wird die Sicherungskopie ohne Dateiendung im Verzeichnis System32 abgelegt.
> Eine Sicherungskopie kann im laufenden Betrieb von MAGELLAN durchgeführt werden. Von der Sicherungskopie sind alle Dokumente, Word-Vorlagen und Berichte ausgenommen.




### Einbinden der Sicherung in den Windows Taskplaner

Sie können die Aktion "Datenbanksicherungskopie erstellen" mit in den Taskplaner des Serverrechners einbinden. Damit könnten Sie sicherstellen, dass diese Aktion automatisch einmal täglich ausgeführt wird. Gehen Sie dafür bitte folgendermaßen vor:

Erstellen Sie mit dem Texteditor eine neue Datei und kopieren den nachfolgenden Text hinein. 

> #### warning::Wichtig!
>
> Bitte beachten Sie, dass die Pfade bei Ihrer Installation abweichen können!


````
"C:\Program Files (x86)\Firebird\Firebird_2_5\bin\gbak.exe" -v -t -user SYSDBA -password masterkey -y "C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup\MAGELLAN6_%date:~0%.log" "C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\MAGELLAN6.FDB" "C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup\MAGELLAN6_%date:~0%.FBK" pause
````

> #### warning::Wichtig!
>
> Seit Windows Server 2012 muss zusätzlich der Parameter gesetzt werden:
````
"C:\Program Files (x86)\Firebird\Firebird_2_5\bin\gbak.exe" -backup -v -t -user SYSDBA -password masterkey -y "C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup\MAGELLAN6_%date:~0%.log" "C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\MAGELLAN6.FDB" "C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup\MAGELLAN6_%date:~0%.FBK" pause
````



Speichern Sie diesen Text und passen die drei Pfade den Gegebenheiten auf Ihrem Serverrechner an. Wir beschreiben nachstehend die Bedeutung der einzelnen Punkte:

Hinweis    | Bedeutung
---------- | -------------
Pfad zur gbak.exe | Der erste Pfad führt zur gbak.exe, die die Datensicherung Ihrer Magellan6.fdb erstellt. Der von uns angebebene Pfad entspricht dem Standardinstallationspfad, könnte bei Ihnen aber abweichen.
 -user und -password | Anschließend ist die Administratorenanmeldung an Ihrer Datenbank in der Datei enthalten, wenn Sie ein anderes Passwort verwenden, tragen Sie dieses anstelle von „masterkey“ein. 
 -y und Pfad|Dieser optionale Pfad legt Ihnen pro Sicherung eine Logdatei mit dem Tagesdatum mit den Meldungen an. 
 Pfad und Dateiname der *.fdb |Der nachfolgende Pfad verweist auf Ihre Datenbank. Liegt Ihre Datenbank an anderer Stelle, passen Sie diesen Pfad bitte an.  
Ablagepfad der Sicherungskopie|Als letzte Information wird der Ablagepfad für die Sicherungskopie mit angegeben. Sie könnten sich einen gesonderten Unterordner "Backup" erstellen, müssten auf diesen dann im Pfad verweisen.
Pfad und Dateiname der *.fbk | Der Dateiname wird automatisch mit Magellan6_aktuelles Datum.fbk angegeben. Durch das Datum im Namen wird sichergestellt, dass die Sicherungskopie des Vortages nicht täglich überschrieben wird.
pause | Programmfenster im Vordergrund oder unsichtbar: Wenn Sie "pause" weglassen, dann läuft die Sicherung im Hintergrund ab, mit pause können Sie den Fortschritt im Vordergrund verfolgen. Wenn Sie eine Logdatei erstellen lassen, können Sie auf diesen Parameter verzichten.

Wenn alle Angaben angepasst sind, speichern Sie die Datei und benennen sie anschließend in "MagellanBackup.bat"um. Legen Sie diese Datei bitte auf Ihrem Server im Datenbankordner ab.

> #### danger::Achtung!
>
>  Führen Sie die Datei zum Test bitte per `Doppelklick` oder `Rechtsklick > Ausführen` aus.

Hat es funktioniert? Dann richten Sie im Taskplaner bitte einen neuen Task ein, der täglich zu einer bestimmten Zeit diese Datei ausführt. Gehen Sie dazu auf dem Server unter `Start > Programme > Zubehör > Systemprogramme > Geplante Tasks`.



