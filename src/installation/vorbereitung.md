# Update-Planung: Wird die Datenstruktur angepasst oder nicht?

Das ist der erste Punkt, der vor der Planung der Updates geprüft werden sollte. Wird nach dem Update die Datenstruktur um neue Felder oder Tabellen erweitert, müssen vorübergehend alle Magellan-Nutzer von der Datenbank abgemeldet werden.

Die Versionsnummer besteht aus einem Teil, der die Ausgabe der Software kennzeichnet und einem Teil, der die Ausgabe der Datenbankversion kennzeichnet. Die Versionsnummer finden Sie im Programm unter `Hilfe > Info über`.
Beispiel:
**Version 6.5.5 664**

Versionsnummer für die Software|Versionsnummer der Datenbank
---|---
6.5.5|644

![Die Versionsnummer finden Sie unter Extras > Info über](/images/update01.png)


Vergleichen Sie die letzten drei Stellen mit der im Newsletter oder im Abschnitt [Was ist neu?](http://doc.magellan6.stueber.de/changelog.html) angegebenen Version. Ist die Datenbankversionsnummer dort höher angegeben, lesen Sie bitte den Abschnitt ["Updates mit Datenstrukturerweiterung"](https://doc.magellan6.stueber.de/installation/vorbereitung.html#updates-mit-datenstrukturerweiterung)!

> #### primary::Wichtig
>
> Wir informieren über neue Ausgaben über unseren [Newsletter](http://www.stueber.de/newsletter.php). 

## Updates ohne Datenstrukturerweiterung

Bitte aktualisieren Sie immer als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Sie können das aktuelle [msi-Paket](ftp://ftp.stueber.de/pub/bin/de/magellan/v6/magellan6.msi) von unserer Webseite herunterladen und direkt per Doppelklick starten oder dazu ein Tool zur Softwareverteilung nutzen.

## Updates mit Datenstrukturerweiterung

Bitte aktualisieren Sie auch hier immer als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner!

Beim ersten Start von Magellan erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Sie müssen dazu wie folgt vorgehen:

Schritt|Aktion
-|-
1.Schritt|Melden Sie sich als sysdba in Magellan an. 
2.Schritt:|Alle anderen Benutzer müssen Magellan verlassen haben!        
3.Schritt:|Der Assistent zur Konvertierung erscheint, führen Sie zuerst die Sicherung Ihrer Datenbank aus!

> #### warning::Wichtig!
>
> Eine Sicherungskopie der Datenbank kann immer nur auf dem Server angelegt werden. Sie können die Aktion zwar vom Clientrechner aus starten, aber der Ablagepfad muss auf dem Server sein. 
>Sie haben zwei Möglichkeiten diesen Pfad einzugeben:
Als Netzwerkpfad: `\\Mein_Server\...\MAGELLAN 6\Datenbank\Backup\20180323.fbk`
Oder als lokaler Pfad aus Sicht des Servers: `C:\Users\Public\Documents\Stueber Systems\Magellan 6\Datenbank\Backup\20180323.fbk`
>
>Beide Varianten legen die Sicherung auf dem Server an. Da Sie sich zuvor an der Datenbankverbindung angemeldet haben, ist der Serverrechner bereits bekannt,  mit `C:/`ist in diesem Fall nicht Ihr lokales Laufwerk gemeint, sondern das Laufwerk `C:` Ihres Serverrechners.

![Beispielpfade](/images/update/pfad.zur.sicherung.png)

**4.Schritt:** Führen Sie die Konvertierung aus. Sollten Sie mehrere Strukturanpassungs-Updates übersprungen haben, werden diese der Reihe nach vom Assistenten durchgeführt. Schließen Sie den Assistenten.
**5.Schritt:** Rufen Sie den Magellan-Administrator auf. Synchronisieren Sie die Zugriffsrechte der Benutzer (Datenbankpflege > Datenbank prüfen, Option: Zugriffsrechte synchronisieren).

> ####### primary::Hinweis
>
> Falls es Probleme gibt, lesen Sie bitte  [**hier**](https://doc.magellan6.stueber.de/installation/probleme-beim-update.html) weiter!**



