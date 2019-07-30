# Benutzerverwaltung

Die Benutzerverwaltung ist das Werkzeug des Administrators, um:

* den Benutzern allgemeinen Zugriffsrechte zuzuweisen,
* Spezielle Rechte zur Nutzung von MyMAGELLAN zuzuweisen und
* das MAGELLAN-Logbuch auszuwerten

Alle Benutzerdaten werden mit der Datenbankdatei abgespeichert.

## Registerkarte „Benutzerliste“

In der Benutzerliste ist jeder Benutzer ist durch seine Kennung, den Nachnamen, Vornamen, sein Lehrerkürzel (optional), seinen Mandanten, sein Kennwort und seinen Status definiert. Für jeden Benutzer können Sie seine Rechte in der Schulverwaltung, Bibliotheks & Lernmittel, Inventarisierung und für MyMAGELLAN, die dezentrale Notenverwaltung, festlegen. 

Einen neuen Benutzer können Sie über die Schaltfläche `Hinzufügen` anlegen, einen bestehenden durch Doppelklick auf den Benutzer auf der Karte „MAGELLAN Benutzerliste“ bearbeiten. Für bereits angelegte Benutzer können Rechte exportiert, angepasst und wieder importiert werden. Zum Beispiel, um einer Gruppe von Benutzer schnell und einfach ein neues Recht zu zuweisen oder den Teilnehmern am MyMAGELLAN-Verfahren einen neuen Ablagepfad für die mym-Datei zu hinterlegen.

Dafür stehen im unteren Bereich der Benutzerverwaltung auf der rechten Seite drei Schaltflächen zur Verfügung.
![Dies ist die Liste der Benutzer in der Benutzerverwaltung](/images/users_benutzerliste.png)

## Benutzer exportieren und importieren

Mit Hilfe eines Assistenten werden alle bereits angelegten Benutzer in eine CSV-Datei exportiert. Bitte geben Sie einen Speicherort und einen Dateinamen an, die Endung „.csv“ wird automatisch ergänzt.

![Die erzeugte Datei kann mit Excel geöffnet und bearbeitet werden.](/images/users_benutzer.exportieren.png)

> #### primary::Hinweis
>
> Auf diesem Weg können keine Benutzer neu angelegt werden, sondern es können für bereits angelegte Benutzer Werte geändert.


In der Datei sind Kopfzeilen und bereits erfasste Einstellungen. Diese Werte können ergänzt oder verändert werden:

Spaltentitel | Mögliche Werte
-------------------------- | --------------
Kennung | Enthalten ist die Benutzerkennung, dieser Wert ist nicht veränderbar
Status | Für die Teilnahme am MyMAGELLAN-Verfahren: Teilnehmer; (Kein Teilnehmer)
Schulverwaltung | Für den Zugriff auf MAGELLAN: (Kein Zugriff), Schulverwaltung 1, Schulverwaltung 2, Sekretariat 1,Sekretariat 2, Kollegium 1, Kollegium 2, Kollegium 3, Kollegium 4, Gast 1, Gast 2, Statistik-Administrator
Bibliothek/Lernmittel | (Kein Zugriff), Schulleitung, Bibliothekar, Kollegium, Gast
Medienkatalog | <Alle Kataloge> oder selbst im Schlüsselverzeichnis angelegte Kataloge (Modul Bibliothek/Lernmittel > Verzeichnisse > Schlüsselverzeichnis Kataloge)
MyMAGELLAN-Datei | Tragen Sie hier den Speicherpfad und den Dateinamen für die MyMAGELLAN-Datei ein, die später mit dem Modul MyMAGELLANCenter erzeugt wird, zum Beispiel:C:\MAGELLAN 6\MyMAGELLAN\Lehrer1.mym
Haushalt/Inventar | (Kein Zugriff), Schulleitung, Sekretariat, Gast
Verzeichnisse | Für die Editierbarkeit von Schlüsselverzeichnissen in MAGELLAN: Nicht editierbar, Editierbar
Aktiv | Ja, Nein, Kennzeichnung des Benutzers als Aktiv oder Inaktiv
Mandanten | Für das Benutzerrecht Mandanten-Administrator: Ja, Nein
Import/ Export | Für den Im- und Export: Ja, Nein
Drucken | Ja, Nein
Dokumente | Zum Zugriff auf die Dokumentenverwaltung: Ja, Nein
Berufsschule | Ermöglicht den Zugriff des Benutzers auf den Menüpunkt Berufsschule. Mögliche Werte: Editierbar, Nicht editierbar
Berufsschule-Prüfungsnoten | Regelt die Sichtbarkeit der Spalten Prüfungsnote und Prüfungsnote (Kontrolle) im Menüpunkt Berufsschule Unterkarte Matrix. Mögliche Werte sind: Kein Recht, Nur Prüfungsnote (Kontrolle), Prüfungsnote + Prüfungsnote (Kontrolle)

Anschließend: Klicken Sie auf die Schaltfläche` Benutzer importieren` um die veränderte Benutzerliste wieder zu importieren. Bitte führen Sie zum Abschluss den Punkt `Datenbankpflege > Datenbank überprüfen > Zugriffsrechte synchronisieren` aus.

## Export nach Excel/HTML

Über diese Schaltfläche können Sie eine Excelliste oder eine HTML-Datei mit den Benutzerdaten erzeugen. Bitte beachten Sie, dass diese Dateiformate nicht wieder direkt eingelesen werden können, dafür nutzen Sie bitte die Schaltfläche `Benutzer exportieren`.

## Registerkarte „Allgemein“

Wählen Sie bitte als erstes im Feld `Mandanten` einen Wert, anschließend wird Ihnen im Feld `Lehrer` die Lehrerliste Ihres Mandanten angeboten. Beim Anlegen eines Benutzers wird aufgrund der Kürzelauswahl der Vor- und Nachname automatisch vorbesetzt.

![Legen Sie hier die Grunddaten des Benutzers fest](/images/users_benutzer.editieren.png)

> #### danger::Achtung!
>
> Die Kürzel der Lehrer dürfen keine Umlaute oder „ß“ enthalten. Bitte passen Sie die Kürzel der Kollegen vorab in MAGELLAN an. Sollten Sie bereits einen Benutzerzugang für einen Kollegen mit einem Umlaut im Kürzel angelegt haben, genügt es nicht das Kürzel in MAGELLAN unter Lehrer zu ändern. Löschen Sie bitte den Benutzer unter `MAGELLAN Administrator > Benutzerverwaltung`, ändern anschließend das Kürzel in MAGELLAN unter `Lehrer > Daten1 > Kürzel` und legen abschließend den Benutzerzugang für den Lehrer erneut an.
Wenn Sie unter Kennwort das Benutzerkennwort eintragen, kann dieses Kennwort gleichzeitig als MyMAGELLAN-Kennwort übernommen werden, wenn Sie das Optionsfeld `Kennwort als MyMAGELLAN-Kennwort übernehmen` markiert haben.
Geben Sie bitte ein achtstelliges Passwort ohne Sonderzeichen für den neuen Nutzer an.

## Registerkarte „Rechte“

![Legen Sie die Rechte für den Benutzer fest](/images/users_rechtekarte.png)

### Allgemeine Rechte

Rechtegruppe | Rechte
-------------------------- | ------
Mandanten-Administrator | Administratorenrechte, aber kein Zugriff auf den MAGELLAN-Administrator, dafür aber Zugriff auf das MyMAGELLAN Center für den jeweiligen Mandanten. Das Verwenden dieses Rechtes erhöht alle Schulverwaltungsrechte.
Import/Export | Zusätzlich zum Schulverwaltungsrecht kann die Möglichkeit des Importes und Exportes (Seriendruck, Excelexport, Schuldatentransferformat) gesteuert werden.
Drucken | Zusätzlich zum Benutzerrecht kann das Drucken ermöglicht werden
Dokumentenverwaltung | Zusätzlich zum Benutzerrecht die Möglichkeit auf die Dokumentenverwaltung zuzugreifen
Berufsschule | Regelt zusätzlich zum Benutzerrecht den Zugriff des Nutzers auf den Menüpunkt Berufsschule
Berufsschule-Prüfungsnoten | Regelt zusätzlich zum Benutzerrecht die Sichtbarkeit der Spalten Prüfungsnote und Prüfungsnote (Kontrolle) im Menüpunkt Berufsschule auf der Registerkarte Matrix
Administratorenrechte | Keine Zugriffseinschränkungen (Administratorenkennung mit Benutzer: sysdba)

### Rechte für die Schulverwaltung

Rechtegruppe | Rechte
----------------------- | ------
Schulleitung 1 | Zugriff auf alle Daten außer auf die Datenbankstruktur und die Benutzerverwaltung
Schulleitung 2 | Wie Schulleitung 1, aber mit der Einschränkung, keine Fächer oder Noten der Schüler zu ändern
Sekretariat 1 | Zugriff auf alle Daten außer auf die Datenbankstruktur und Benutzerverwaltung
Sekretariat 2 | Wie Sekretariat 1 aber mit folgenden Einschränkungen: Darf nur Fächer der Schüler sehen (d.h. Schüler/Zeugnis/Leistungen + Schüler/Zeugnis/Details + Zeugnisbemerkungen/-Formulare nicht sichtbar)
Kollegium 1 | Die Noten und Zeugnisdaten der Schüler, die unterrichtet werden, dürfen erfasst bzw. geändert werden. Ansonsten bestehen nur Leserechte.<br/>Wenn Lehrer Klassenleiter 1 oder 2 oder Tutor ist, darf er die o.g. Daten aller Schüler seiner Klasse verändern (auch wenn er diese nicht unterrichtet).<br/>Das Menü „Lehrer“ zeigt nur die eigenen Personaldaten an. Kollegiumsrechte müssen zugewiesen sein, damit man MyMAGELLAN-Dateien bearbeiten kann. Welche Voraussetzungen hierfür des Weiteren gegeben sein müssen, erfahren Sie im Abschnitt „Das MyMAGELLAN Center“ unter „Voraussetzungen“.
Kollegium 2 | Wie Kollegium 1, zusätzlich auch Laufbahndaten und Fehlzeiten des Schülers editierbar
Kollegium 3 | Wie Kollegium 2, aber keine Zeugnisformulare der Schüler editierbar
Kollegium 4 | Wie Kollegium 2, aber keine Zeugnisformulare und Zeugnisbemerkungen editierbar
Kollegium 5 | Wie Kollegium 2, zusätzlich auch das Abiturmenü für alle Schüler editierbar
Gast 1 | Leserechte. Schreibzugriff ist nicht möglich. Das Menü „Lehrer“ zeigt nur die eigenen Personaldaten
Gast 2 | Leserechte. Schreibzugriff ist nicht möglich. Das Menü „Lehrer“ zeigt die Personaldaten aller Lehrer an.
Statistik-Administrator | Wie Schulleitung 1, zusätzlich können die folgenden Punkte ausgeführt werden: im Administratormodul „Schlüsselverzeichnisse importieren“, „Mach-Export“, den Abgleich zwischen MAGELLAN und daVinci, Starten des DWH-Explorers

> #### primary::Hinweis
>
> Je Benutzer kann für die Schulverwaltung insbesondere festgelegt werden, ob der Benutzer das zusätzliche Recht besitzt, die Verzeichnisse in MAGELLAN zu editieren. Kann er die Verzeichnisse nicht editieren, so wird das Menü „Verzeichnis“ für Benutzer in MAGELLAN ausgeblendet. Er kann somit keine Schlüssel in den Verzeichnissen ändern. Im Standardfall hat ein Benutzer kein Recht Verzeichnisse zu editieren, das dies im Regelfall nur von einem ausgewählten kleinen Personenkreis durchgeführt werden soll.

### Bibliotheksrechte

Rechtegruppe |	Rechte
------------ | ------
Bibliothekar |	Zugriff auf alle Daten der Bibliotheksverwaltung
Schulleitung | wie Bibliothekar, aber kein Zugriff auf die Optionsunterkarten: Ausleihe, Quittung, Mahnwesen und Dokumente.
Kollegium | wie Schulleitung
Gast | nur Leserechte

> #### danger::Achtung!
>
> Beim Anlegen der Kennung bitten wir Sie, auf Abkürzungen wie „Do“ und „If“ zu verzichten, da diese Kürzel gleich lautend mit Programmierbefehlen sind und von Firebird fehl interpretiert werden. Es gibt noch weitere so genannte „reservierte“ Worte, die Sie in der Dokumentation [„MAGELLAN-Scripting“](https://doc.magellan-scripting.stueber.de/) in Kapitel „Die Skriptsprache“ nachschlagen können.
Die Benutzer können ihr Passwort in MAGELLAN unter `Datenbank > Kennwort` ändern selbst anpassen. Dafür werden mindestens 8 Zeichen erwartet. Sollte die Schaltfläche Kennwort ändern inaktiv bleiben, ist der Benutzer als Datenbankadministrator(„sysdba“) angemeldet. Dieses Kennwort kann nur im MAGELLAN-Administrator verändert werden.

## Registerkarte „MyMAGELLAN“

![Sie können auf dieser Karte festlegen, ob der Benutzer Noten mit MyMAGELLAN erfassen darf, ein MyMAGELLAN-Kennwort besitzt und den späteren Speicherort seiner MyMAGELLAN-Datei angeben.](/images/users_mymagkarte.png)

Alle Rechteangaben eines Benutzers zu MyMAGELLAN werden aus Gründen der Übersichtlichkeit hier nochmals aufgelistet.

![Hier sehen Sie eine Übersichtsliste alle Teilnehmer von MyMAGELLAN.](/images/users_mymag.liste.png) 

## Registerkarte „Logbuch“

Im Logbuch werden alle An- und Abmeldung pro Benutzer protokolliert.

![Das Logbuch protokolliert all An- und Abmeldung in MAGELLAN](/images/users_logbuch.png) 