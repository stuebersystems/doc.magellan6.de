# Gymnasiale Oberstufe

Die Oberstufe stellt den schwierigsten Teil der Schulorganisation dar. MAGELLAN und DAVINCI stellen sehr ausgefeilte Funktionen für die gesamte Oberstufenorganisation zur Verfügung. Damit die Berechnungen korrekt durchgeführt und die entsprechenden Zeugnisse richtig ausgedruckt werden können, müssen Sie einige wenige aber wichtige Schritte beachten.
 
In DAVINCI KURSPLAN können Sie die Schüler-Fachwahlen inkl. Fachwahlüberprüfung erfassen und per Automatik die Kurse blocken sowie die Schüler auf Kurse verteilen. MAGELLANs Vorschlagsautomatik sagt Ihnen, welche Kurse der Schüler für die maximale Punktzahl einbringen sollte. MAGELLAN errechnet die Abiturqualifikation und druckt die Abiturzeugnisse. Fachwahlüberprüfung und Abiturqualifikationsberechnung basieren auf Skripten, die Sie mit Hilfe des MAGELLAN-Skripteditors bearbeiten können, was aber in der Regel nicht notwendig ist. Weitere Informationen zu diesen Skripten finden Sie in der Dokumentation [MAGELLAN-Scripting](https://doc.magellan-scripting.stueber.de/).

> #### warning::Wichtig!
>
> Eine ausführliche Beschreibung der Gymnasialen Oberstufe finden Sie in der Dokumentation [Landesanpassungen](https://doc.la.stueber.de/). Dort können Sie auch nachlesen, für welche Bundesländer entsprechende Berechnungsskripte vorliegen. In diesem Handbuch werden nur die wichtigsten Schritte erläutert.

## Aufgaben

Zur Oberstufenorganisation gehören folgende Aufgaben:

1. Stammdaten und Schlüsselverzeichnisse einrichten
2. Schüler-Fachwahlen eingeben sowie Kursangebot und Kursblockungen erstellen
3. Zulassung zur 12 überprüfen (nur in einigen Bundesländern)
4. Abiturzulassung überprüfen
5. Gesamtqualifikation für schriftlichen Prüfungsbereich (Abiturnote) berechnen
6. Fachhochschulreife berechnen
7. Zeugnisbemerkungen eingeben und Zeugnisse drucken

Schritt 1 muss in DAVINCI und MAGELLAN durchgeführt werden. 
Schritt 2 wird in DAVINCI-Kursplan oder MAGELLAN durchgeführt, alle weiteren Schritte ausschließlich in MAGELLAN. Auf die Berechnung der Fachhochschulreife in Schritt 6 wird hier verzichtet, da sie ausführlich in der Dokumentation [Landesanpassungen](https://doc.la.stueber.de/) erläutert ist.
Optional können Sie die Schülerfachwahlen auch in MAGELLAN eingeben, allerdings ist die Eingabe in DAVINCI-Kursplan wesentlich effizienter. In MAGELLAN können Sie die Fächer der Oberstufe analog zu anderen Jahrgangsstufen eingeben, indem Sie erst auf Ansicht „Schüler“ und dann für die einzelnen Schüler auf der Registerkarte „Zeugnis“ die Registerkarte „Fächer“ wählen und dort die Fächer eingeben. Um die Oberstufendaten des jeweiligen Schülers in MAGELLAN anzuzeigen, klicken Sie in MAGELLAN links in der Symbolleiste auf „Abitur“.

## Stammdaten und Schlüsselverzeichnisse einrichten


Die halbjährlich erworbenen Noten der Oberstufe samt der Fächer und weiteren Informationen (zum Beispiel Merkmale, Fachstatus, Unterrichtsarten) sollen per Assistent auf die Karte `Abitur > Qualifikation` in den korrekten Spalten (E1 bis Q4, eventuell regionale Abweichungen möglich) synchronisiert werden. Anschließend sollen skriptbasierte Berechnungen ausgeführt werden. Das Synchronisieren der Halbjahresdaten in das Menü `Abitur `und die anschließenden Berechnungen per Skript, gelingen nur, wenn die Daten entsprechend vorbereitet sind. Bitte schauen Sie sich dazu die nachstehenden Hinweise für die Vorbereitung der Stammdaten und Schlüsselverzeichnisse an.


### Verzeichnis Zeiträume

Bitte überprüfen Sie unter `Verzeichnisse > Zeiträume > Art`, dass die Art `1.Halbjahr` oder `2.Halbjahr` korrekt für jede Zeile gefüllt ist.

### Eingaben für Klassen

Die Oberstufe besteht aus den Jahrgängen 11, 12 und 13. In MAGELLAN und DAVINCI sind Klassen und Jahrgänge gleichbedeutend. In MAGELLAN werden die Daten halbjahresbezogen abgelegt. Sie definieren also drei Klassen 11, 12 und 13 mit je zwei Zeiträumen bzw. Halbjahren. Folgende Angaben sind bei der Eingabe der Oberstufenjahrgänge neben den Halbjahren wichtig:

Eingabefeld | Eingabe
--------------- | -------
Klassenart | Oberstufenjahrgang (Leistungs- und Grundkurse) oder Oberstufenjahrgang (nur Kurse). Möchten Sie Schüler für die Fachwahlkarte synchronisieren, können Sie für die Klasse auch die Klassenart „Standard mit Oberstufensynchronisation“ verwenden, hierbei werden nur die Schülerdaten übergeben, keine Fach- oder Leistungsdaten.
Jahrgang | 11, 12 oder 13 [bei G9] bzw. 10, 11 oder 12 [bei G8] (pro Zeitraum der Klasse notwendig)
Beurteilungsart | Benotung durch Punkte (oder Noten)

### Verzeichnisse Unterrichtsarten und Fachstatus

Voraussetzung für die Fachwahlüberprüfung und die Abiturqualifikationsberechnung ist, dass Sie in der Oberstufe bei den Fächern des Schülers die entsprechende Unterrichtsart und den entsprechenden Fachstatus eingegeben haben. Welche Unterrichtsarten und Fachstatus von den mitgelieferten Skripten in Abhängigkeit vom jeweiligen Bundesland verwendet werden, wird in der Dokumentation [Landesanpassungen](https://doc.la.stueber.de/) ausführlich je Skript erläutert.

### Verzeichnis Fächer

> Geben Sie für jedes Fach, das Sie in der Oberstufe verwenden, Fachkategorie und Aufgabenbereich an:

* Klicken Sie auf `Verzeichnisse > Fächer` und machen Sie im Verzeichnis der Fächer die entsprechenden Eingaben in den Spalten „Kategorie“ und „Aufgabenbereich“.
* Alternativ können Sie diese Angaben auch in DAVINCI vornehmen und die Daten dann nach MAGELLAN übernehmen.

in der Dokumentation [Landesanpassungen](https://doc.la.stueber.de/) finden Sie eine entsprechende Anleitung, für welches Bundesland pro Fach welche Einstellungen bei Fachkategorie bzw. im Aufgabenbereich vorgenommen werden müssen.


### Verzeichnis Abschlussjahrgänge

![Hier definieren Sie den Abiturjahrgang mit der Kategorie „Abitur“](/images/gym_oberstufe/gym_oberstufe01.png)

Sie können in MAGELLAN unter `Verzeichnisse > Abschlussjahrgäng`e Abschlussjahrgänge definieren. In unserem Fall ist dies ein Abiturjahrgang. Damit können Sie jedem Schüler in der Rubrik „Abitur“ den entsprechenden Abiturjahrgang zuordnen. Dieser Vermerk hat keinen Einfluss auf Abschluss- oder Qualifikationsberechnungen, sondern dient dazu, später alle Schüler eines bestimmten Abiturjahrgangs z.B. für Ausdrucke herausfiltern zu können.

> #### warning::Wichtig!
>
> Geben Sie bei der Definition des Abiturjahrgangs im Fenster „Verzeichnisse der Abschlussjahrgänge“ unter „Kategorie“ unbedingt „Abitur“ an.

### Verzeichnis Verordnung 


![Verzeichnis der Verordnungen](/images/gym_oberstufe/gym_oberstufe02.png)

Sie müssen für jeden Schüler die Abiturordnung angeben, die für ihn relevant ist. Dazu müssen Sie im Schlüsselverzeichnis „Verordnungen“ die jeweilige Fachwahlverordnung und/oder Abiturprüfungsordnung definieren. Bitte prüfen Sie vorab, ob es ein Prüfskript für Ihre Region und Verordnung gibt. 

> #### danger::Achtung!
>
> Alle verfügbaren Skripte finden Sie in der Dokumentation ["Landesanpassungen"](https://doc.la.stueber.de/)  im Abschnitt ["Alle Skripte im Überblick"](https://doc.la.stueber.de/alle_skripte_im_uberblick.html). 

Um Ihre Prüfskript in MAGELLAN zu hinterlegen,  klicken Sie dazu auf `Verzeichnisse > Verordnungen` und geben Sie dort die Verordnung an.

Welche Eintragungen für Ihre Region oder für Ihr Skript erwartet werden, [beschreiben wir für jedes verfügbare Skript  in unserer Landesanpassung](Bitte richten Sie sich genau nach der Anleitung für Ihr Skript!). 

Spalte | Bedeutung
-------------- | ---------
Kürzel | Kurzbezeichnung der Verordnung (max. 10-stellig)
Bezeichnung | Bezeichnung der Verordnung
Kategorie | Geben Sie hier „Abitur“ ein, für die Prüfungsverordnung der Qualifikationsberechnung. Diese Verordnung können Sie für die Qualifikationsüberprüfung auf den Registerkarten `Ansicht Abitur > Qualifikation` und `Ansicht Abitur > Prüfung` verwenden. Wenn Sie hier `Fachwahl` eingeben, können Sie diese Verordnung für die Fachwahlüberprüfung auf der Registerkarte `Ansicht Abitur > Fachwahl` verwendet.
Typ|[Bitte richten Sie sich genau nach der Anleitung für Ihr Skript!](https://doc.la.stueber.de/allgemeines_spezielle_einstellungen_pro_skript.html)
Ab Jahrgang | Geben Sie hier den Jahrgang an, ab der die Oberstufenverordnung gilt, mögliche Eingaben sind Jahrgang 10(G8) oder 11(G9). Nach dieser Eingabe werden die Daten in unterschiedliche Spalten im Abiturmodul synchronisiert.
Notenart 11-13 | Geben Sie hier an, ob Sie in der Oberstufe Punkt- oder Notenwerte (z.B. in Nordrhein-Westfalen) vergeben möchten. [Bitte richten Sie sich genau nach der Anleitung für Ihr Skript!](https://doc.la.stueber.de/allgemeines_spezielle_einstellungen_pro_skript.html)
Gültig von | Gültigkeitsdatum von, ohne Bedeutung für die Berechnungen
Gültig bis | Gültigkeitsdatum bis, ohne Bedeutung für die Berechnungen
Skript | Geben Sie hier den Namen des Skripts für diese Abiturprüfungsordnung ein. Das Skript enthält auch die Berechnung der Fachhochschulreife. Alle verfügbaren Skripte befinden sich im MAGELLAN-Verzeichnis SKRIPTE.

###  Fachwahlen oder Halbjahresdaten synchronisieren

![Dialogfenster zum Synchronisieren der Daten für das Abitur](/images/gym_oberstufe/gym_oberstufe03.png)

Bevor Sie die Fachwahlen bzw. Abiturqualifikationen überprüfen können, müssen Sie die Daten der Schüler synchronisieren, indem Sie in MAGELLAN auf Abitur klicken und dann auf die Schaltfläche `Schüler synchronisieren` im MAGELLAN-Fenster klicken.

Beim Synchronisieren geschieht Folgendes: 
 Klassenart ""MAGELLAN prüft die Klassenart der gewählten Schüler und synchronisiert entweder nur die Schülerdaten ins Menü `Abitur `oder die Schülerdaten, Schülerfachdaten und in den Halbjahren erfassten Leistungen.

#### Schüler für Fachwahlen synchronisieren

Die Fachwahlen der Schüler werden vor dem Eintritt in die Oberstufe erfasst. Dafür müssen nur die Schüler (also ohne Fachdaten oder Noten) ins Menü `Abitur` übernommen werden. Dieser Unterschied wird mit der Klassenart vorgenommen, stellen Sie bei den Klassen bitte "Standard mit Oberstufensynchronisation" ein.

![Klassenart für die Fachwahl](/images/gym_oberstufe/oberstufe01.png)

#### Schüler für Berechnungen synchronisieren

MAGELLAN extrahiert für die markierten Schüler die Fachdaten der Halbjahre 11/1 bis 13/2 (bei G9) bzw. 10/1 bis 12/2 (bei G8) und ordnet die Daten in den Spalten E1 bis Q4 auf der Qualifikationskarte im Menü Abitur an. Ob die Schülerdaten passend nach dem G8- oder G9-System angeordnet werden, legen Sie im Verzeichnis `Verordnungen` in der Spalte Jahrgang an. Was genau Sie dort eintragen, beschreiben wir pro Berechnungsskript in der Dokumentation [Landesanpassungen](https://doc.la.stueber.de/).



![Klassenart für die Oberstufenberechnungen](/images/gym_oberstufe/oberstufe02.png)


> #### warning::Wichtig!
>
> Für das Erfassen der Fachwahlen der Schüler, müssen vor dem Synchronisieren keine Fächer auf der Registerkarte Ansicht `Schüler > Zeugnis > Fächer` eingetragen werden. Sind dort aber bereits Fächer erfasst gewesen, können Sie die Fächer beim Synchronisieren auch zusätzlich mit in die Fachwahlen übertragen lassen. Wählen Sie dafür vor der Synchronisation die Option `Extras > Optionen > Einstellungen > Abgleich Qualifikationen/Fachwahl im Abitur`.

Damit die Schüler mit allen Fächern und Noten aus den einzelnen Jahrgängen korrekt übernommen werden können, sind folgende Angaben in MAGELLAN notwendig.


| Eintragung         | Anmerkung                                |
|--------------------|------------------------------------------|
| Zeitraumart        | Im Verzeichnis der Zeiträume muss das Feld „Art“ mit dem Wert „1. Halbjahr“ bzw. “2. Halbjahr“ oder für Schulen, die mit Trimestern arbeiten mit „1. Trimester“, „2. Trimester“ oder „3. Trimester“gefüllt sein. |
| Klassenart         | Unter `Klasse > Daten` muss im Feld `Klassenart` die Auswahl `Oberstufenjahrgang (Leistungs- und Grundkurse)` oder `Oberstufenjahrgang (nur Kurse)` getroffen sein.<br/>Sie können auch die Art `Standardklasse mit Oberstufensynchronisation` wählen, hierbei werden aber lediglich die Schüler für den Punkt `Abitur > Fachwahl` übertragen, also keine Schülerfachdaten oder Leistungsdaten. |
| Jahrgang           | Bei jeder Klasse/Jahrgang muss auf der Registerkarte `Zeiträume` für jeden Zeitraum das Feld `Jahrgang` mit dem Wert „11“, „12“ oder „13“ angegeben werden. |
| Abschlussjahrgänge | Bitte legen Sie unter `Verzeichnisse > Abschlussjahrgänge..` die Abschlussjahrgänge an. Es genügt dabei die Angabe des Kürzels, der Bezeichnung und der Kategorie (Abitur). |
| Verordnungen       | Richten Sie bitte unter `Verzeichnisse > Verordnungen` pro verwendeter Abiturverordnung oder Fachwahl eine Zeile entsprechend der Anleitung in der Dokumentation [Landesanpassung](https://doc.la.stueber.de/)ein. |
| Fachstatus         | Sind die markierten Schüler bereits zuvor einmal synchronisiert worden sein können, kann man für die erneute Synchronisation entscheiden, ob der Fachstatus pro Fach im Bereich Abitur durch die Synchronisation überschrieben werden soll oder nicht. Sollen die im Abiturbereich eingetragenen Fachstatus erhalten bleiben, so haken Sie bitte per Mausklick die Option Eingetragene Fachstatus nicht überschreiben an. |
| Unterrichtsart     | Gibt es ein Fach in der Oberstufe bei einem Schüler mit unterschiedlichen Unterrichtsarten, entscheiden Sie mit dieser Option, ob das Fach auch in mehreren Fachzeilen in den Abiturbereich übertragen werden soll. |



 ![Abiturjahrgang und Prüfungsordnung sind Pflichtangaben, die weiteren Angaben sind optional](/images/gym_oberstufe/gym_oberstufe04.png)
 
> #### warning::Wichtig!
>
>  Damit die Fachdaten und Noten bei G8- oder G9-Schülern in die korrekten Spalten auf der Qualifikationskarte übernommen werden, muss unter `Verzeichnisse > Verordnungen > Jahrgang` eine 10 (für G8) oder eine 11 (für G9) angegeben werden.
> Beim Synchronisieren wird auch der jeweilige Fachlehrer aus der `Ansicht Schüler > Zeugnis > Fächer` in der Spalte `Lehrer` in die `Ansicht Abitur > Qualifikation` übernommen. Dabei werden jeweils die Informationen der Fachlehrer des letzten Zeitraums übertragen.
> Sollte ein Schüler einen Oberstufenjahr wiederholen und ein Fach oder mehrere Fächer im zweiten Anlauf nicht mehr belegen, müssten Sie diese Fächer bitte von Hand aus der Registerkarte `Ansicht Abitur > Qualifikation` entfernen.

Klicken Sie nach dem Synchronisieren auf die Schaltfläche `Abitur `in der Symbolleiste links im MAGELLAN-Fenster. Es werden alle synchronisierten Schüler auf der Registerkarte „Auswahl“ angezeigt. Per Doppelklick auf den gewünschten Schüler oder über einen Klick auf die Registerkarte `Qualifikation `wechseln Sie zur Abiturzulassung. Auf dieser Registerkarte finden Sie die Fächer und Notenwerte der Oberstufenhalbjahre, falls Sie diese Angaben bereits in MAGELLAN auf der Registerkarte Ansicht `Schüler > Zeugnis > Fächer` gemacht haben sollten. Andernfalls können Sie Fächer und Notenwerte für die Oberstufenhalbjahre auch hier eingeben. Sollte die 11 in Ihrem Bundesland nicht in Leistungs- und Grundkursen unterrichtet werden, erscheinen die Fächer der besseren Übersicht wegen trotzdem unterschieden nach den Leistungs- und Grundkursen der Jahrgangsstufen 12 und 13. Intern macht MAGELLAN für die Noten der 11 keine Unterscheidung in Leistungs- und Grundkurse.

## Die Fachwahlüberprüfung

Nachdem Sie die Schüler in die Ansicht „Abitur“ synchronisiert haben, kann die Fachwahl erfasst werden.

### Abgleich der Karte Qualifikation und Karte Fachwahl im Menü Abitur

Unter `Extras > Optionen > Einstellungen` kann die Option `Abgleich Qualifikation/Fachwahl` im Abitur gewählt werden.

> #### danger::Achtung!
>
> **Wir empfehlen diese Option nicht zu wählen!** Die Qualifikationskarte wird später aus den Daten der Halbjahre mit den belegten Fächern und den dazugehörigen Noten befüllt. Die Fachwahl kann durchaus Fächer beinhalten, die später nicht belegt werden.
  
Folgende Aktionen werden durch diese Option beeinflusst:


| Aktion                                   | Ergebnis                                 |
|------------------------------------------|------------------------------------------|
| Synchronisieren von Schülern ins Menü Abitur | Gibt es für die synchronisierten Schüler bereits Fachdaten im Menü `Schüler > Zeugnis > Fächer`, werden diese auf die Karten `Qualifikation `und `Fachwahl `übernommen. |
| Ein Fach wird ergänzt                    | Wird ein Fach auf der Karte Qualifikation oder auf der Karte Fachwahl neu angelegt, wird das Fach automatisch auf der anderen Karte ergänzt. Das gilt auch durch das Ergänzen per Fachwahltafel auf der Karte Fachwahl oder durch erneutes Synchronisieren der Schüler in das Abiturmenü. |
| Ein Fach wird gelöscht                   | Wird ein Fach auf der Karte Qualifikation oder auf der Karte Fachwahl gelöscht, wird das Fach automatisch auf der anderen Karte entfernt. |
| Unterrichtsart, Fachstatus o.ä. wird verändert | Ist ein Fach durch den Abgleich auf beiden Karten angelegt worden und es wird eine der zusätzlich zur Verfügung stehenden Eigenschaften geändert, wird die Änderung auch auf der anderen Karte mit abgebildet. |
| Bereits bestehende Fächer                | Bereits bestehende Fächer auf der Karte `Fachwahl `und `Qualifikation `werden durch das Setzen der Option `Abgleich Qualifikation/Fachwahl im Abitur` nicht automatisch abgeglichen. Die Option wirkt sich auf neu angelegte oder neu synchronisierte Fächer aus. |




Anschließend können Sie für jeden Schüler dessen Fachwahlen auf der Registerkarte Ansicht `Abitur > Fachwahl` eintragen und gleichzeitig auf Korrektheit prüfen. Alternativ können Sie an dieser Stelle auch die Daten nach DAVINCI übertragen und dort die Fachwahl durchführen. Anschließend können die Fachwahlen wieder nach MAGELLAN zurücksynchronisiert werden.

![ Registerkarte „Fachwahl“ zur Eingabe der Schüler-Fachwahlen](/images/gym_oberstufe/gym_oberstufe05.png)

Grundsätzlich wird hier

1. die Fachwahl des Schülers eingetragen (siehe nachfolgenden Abschnitt „Fachwahl eintragen“),
2. die Fachwahl auf Basis einer Fachwahlverordnung auf Gültigkeit überprüft (siehe nachfolgenden Abschnitt „Fachwahl prüfen“)
3. die gültige Fachwahl abschließend zu den Fächern des Schülers übernommen (siehe nachfolgenden Abschnitt „Fachwahl zu den Fächern des Schülers “)

> #### primary::Hinweis
>
> Die Fachwahleingabe kann auch in DAVINCI KURSPLAN erfolgen. Dort ist die Fachwahleingabe etwas ausführlicher und komfortabler: Es können zusätzlich die Stundenzahlen der einzelnen Halbjahre eingegeben werden. Das zugrundeliegende Skript, d.h. das Regelwerk, ist in beiden Fällen das gleiche: MAGELLAN verwendet für die Fachwahlüberprüfung das DAVINCI Fachwahl-Skript.

### Fachwahl eintragen

Das Eintragen der Fächer für die Fachwahl kann sowohl rein manuell pro Fach erfolgen oder wesentlich komfortabler per Zuordnung von Fachwahltafeln.

#### Fachwahltafeln zuordnen

Durch die Verwendung von Fachwahltafeln können Sie Kopiervorlagen definieren, die Sie über den Assistenten für die Zuweisung Fachwahltafel ein oder mehreren Schüler gleichzeitig zuweisen können.

So definieren Sie eine Fachwahltafel:

1. Wählen über `Verzeichnisse > Fachtafeln` das Verzeichnis der Fachtafeln aus.

2. Legen Sie auf der Registerkarte `Fachtafeln `über `Neue Zeile` eine neue Fachwahltafel an. Achten Sie dabei auf den Eintrag „Fachwahltafel“ in der Spalte `Art`.

3. Tragen Sie für die Fachwahltafel auf der Registerkarte Fachwahltafel – Fächer“ die Fächer der Fachwahltafel mit deren Eigenschaften ein.




#### Empfehlung zum Anlegen einer Fachwahltafel

Die nachstehenden Hinweise eine Empfehlung, damit Sie möglichst wenig nach dem Zuweisen noch pro Schüler anpassen müssen. Zusätzlich sind für Berechnungsskripte und Zeugnisberichte bestimmte Eintragungen Voraussetzung für korrektes Funktionieren, einige Angaben können Sie hiermit bereits sicherstellen.

Eintrag|Hinweis
---|---
**Fach**|Legen Sie in der Fachwahltafel jedes in der Oberstufe wählbare Fach als nur eine Zeile an. Es gibt nur eine Zeile für Deu,  nicht Deu als GK und Deu als LK usw. <br/>Das ist besonders wichtig, wenn Sie im Anschluss einen Kurswahlbogen nutzen möchten, Berichte sind für eine Höchstzahl von Zeilen ausgelegt, anderenfalls gelingt die korrekte Darstellung eventuell nicht mehr.  
**Unterrichtsart**|Weisen Sie jedem Fach die am ehesten zutreffende Unterrichtsart zu, zum Beispiel alle Fächer erhalten die Unterrichtsart GK.
**Fachstatus**|Tragen Sie hier nur etwas ein, wenn es eine definitive Zuordung zwischen Fach und Fachstatus gibt.
**Markieren**|Legen Sie hier das häufigste Belegungsmuster fest.
**Position**|Zeugnisberichte benötigen Informationen um Fächer an der korrekten Stelle zeigen zu können. Bitte schauen Sie im Modul MAGELLAN Berichte nach, ob für die von Ihnen eingesetzen Zeugnisberichte Vorgaben für Position pro Fach existieren und tragen Sie diese hier bitte bereits ein. 
**Q1Sprache-Q4Sprache**|Einige Zeugnisberichte geben Hinweise zu bilingualem Unterricht aus, bitte schauen vorab im Modul MAGELLAN Berichte nach, ob das für Ihre Zeugnisse zutrifft und geben ggfs. die Information bereits hier ein. 


![Beispiel für den Inhalt einer Fachwahltafel](/images/gym_oberstufe/fachwahltafel.png)

#### Eine Fachwahltafel zuweisen

So weisen Sie eine Fachwahltafel Schülern in der Ansicht „Abitur“ zu:

1. Wechseln Sie in der Ansicht „Abitur“ auf die Registerkarte Fachwahl.

2. Klicken Sie im oberen Bereich auf die Schaltfläche `Fachwahltafel zuweisen`.

![Hier können Sie Schülern Fachwahltafeln zuweisen.](/images/gym_oberstufe/gym_oberstufe07.png)

3. Markieren Sie die Schüler, denen Sie eine Fachwahltafel zuweisen wollen und klicken Sie dann auf `Weiter`.

4. Markieren Sie die gewünschte Fachwahltafel und ordnen Sie optional im unteren Bereich den Halbjahren die entsprechende Zeiträume zu. Sollen bei der Zuweisung der Fachwahltafeln die eventuell bereits bestehenden Fachwahlen der markierten Schüler nicht zuvor gelöscht werden, so müssen Sie das Kontrollkästchen Vorhandene Fachwahlen der Schüler nicht löschen markieren. Klicken Sie auf `Weiter`.

5. Geben Sie optional den zuzuordnenden `Abiturjahrgang `und die `Fachwahlverordnung `an und klicken Sie dann auf `Weiter`.

6. Klicken Sie auf `Fertigstellen`, um die Fachwahltafel den markierten Schülern zuzuordnen.

#### Fächer manuell zuordnen

Die Fächer der Fachwahl können auch ohne die Kopiervorlage der Fachwahltafeln dem Schüler zugeordnet werden. Dazu gehen Sie pro Fach wie folgt vor:

1. Wechseln Sie in der Ansicht „Abitur“ auf die Registerkarte Fachwahl.

2. Klicken Sie im oberen Bereich auf das rote Plus für eine neue Zeile.

3. Tragen Sie jetzt das Fach und optional die Unterrichtsart und den Fachstatus ein.

> #### warning::Wichtig!
>
> Wird ein Fach manuell zugeordnet, sind in der dadurch erzeugten neuen Zeile die Spalten „1. HJ“ bis „6. HJ“ automatisch markiert.

Wenn Sie die Fachwahl manuell pro Fach auf diese Weise zuordnen, müssen Sie im Unterschied zur Zuweisung per Fachwahltafel auch

* pro Fach die Pflichtkursanzahl optional eintragen,
* pro Fach die Unterrichtsart und optional den Fachstatus eintragen,
* pro Fach festlegen, in welchen Halbjahren das Fach belegt wird sowie
* die Fachwahlverordnung und Zuordnung der Halbjahre zu den die Zeiträume pro Schüler manuell vornehmen.

### Fachwahl prüfen

Sobald Sie dem Schüler eine Fachwahlverordnung zugeordnet haben, wird die Schaltfläche `Neu prüfen` zur Überprüfung der Fachwahl aktiv. Auf Basis der eingetragenen Fachwahl können Sie durch Wahl der Schaltfläche `Neu prüfen` diese prüfen. Das Ergebnis der Prüfung wird im oberen Bereich der Registerkarte Fachwahl angezeigt. Ist die Anzeige rot unterlegt, handelt es sich um eine (noch) nicht gültige Fachwahl.

 ![Diese Fachwahl ist noch fehlerhaft](/images/gym_oberstufe/gym_oberstufe09.png)

Bei einer gültigen Fachwahl ist der obere Hinweistext grün hinterlegt mit dem Hinweis „Fachwahl ist gültig“.

![Diese Fachwahl ist gültig](/images/gym_oberstufe/gym_oberstufe10.png)

Mit Wahl der Schaltfläche `Neu prüfen` wird oberhalb dieser Schaltfläche der Status `Fachwahl geprüft ` angezeigt. Verändert man die Fachwahl des Schülers, wechselt der Status automatisch auf Fachwahl nicht geprüft.


![Dies ist die Anzeige des Prüfstatus „Fachwahl nicht geprüft“ bzw. „Fachwahl geprüft“](/images/gym_oberstufe/gym_oberstufe11.png)
!](/images/gym_oberstufe/gym_oberstufe12.png)



> #### warning::Wichtig!
>
> Ist für ein eingetragenes Fach keine der Spalten „1. HJ“ bis „6. HJ“ markiert, wird dieses Fach bei der Fachwahlprüfung als nicht gewählt betrachtet.
> Die Zuordnung der Zeiträume zu den Halbjahren 1 bis 6 auf der rechten Seite haben keinen Einfluss auf die Fachwahlprüfung. Sie dienen nur der späteren Zuweisung der Fahlwahlen eines Halbjahres zu den Fächern des Schülers (siehe nachfolgender Abschnitt)

### Fachwahl zu den Fächern des Schülers übernehmen

Die unter Ansicht `Abitur > Fachwahl` erstellten Fachwahlen der Schüler können nun zu Fächern der Schüler auf der Registerkarte Ansicht `Schüler > Zeugnis > Fächer` übernommen werden. Diese Zuweisung erfolgt immer zum aktuell eingestellten Zeitraum.

Bei der Übernahme der Fachwahl eines Schülers werden nur die Fächer übernommen, die

* in einem der sechs Halbjahre auf der rechten Seite den aktuellen Zeitraum von MAGELLAN zugewiesen haben und
* die in diesem Halbjahr das Kontrollkästchen markiert haben.

Beispiel:

In MAGELLAN ist der aktuelle Zeitraum das „1. Halbjahr 2011/2012“. Der Schüler hat die nachfolgende Fachwahl:

 ![Beispiel für die Fachwahl eines Schülers](/images/gym_oberstufe/gym_oberstufe13.png)

Die Spalte 1. HJ entspricht dem Zeitraum „1. Halbjahr 2011/2012“. Übernimmt man nun die Fachwahl im aktuellen Zeitraum, so werden alle Fächer der Fachwahl übernommen bis auf das Fach „Fr“, da dieses in der Spalte 1. HJ nicht markiert ist.

Auf Basis dieser Zuordnung kann nun die Zuweisung der Fachwahlen zu den Fächern der Schüler wie folgt durchgeführt werden:

1. Wechseln Sie in der Ansicht `„Abitur“` auf die Registerkarte `Fachwahl`.

2. Klicken Sie im oberen Bereich auf die Schaltfläche `Fachwahl übernehmen`.

3. Markieren Sie die Schüler, deren Fachwahl Sie übernehmen wollen. 

4. Klicken Sie auf `Fertigstellen`, um die Fachwahlübernahme zu starten.

Die übernommen Fächer finden Sie nun auf der Registerkarte Ansicht `Schüler > Zeugnis > Fächer`.


|Option im Assistenten|Bedeutung|
|--|--|
|![](/images/gym_oberstufe/fw.06.png) |Es wird geprüft, ob bereits für den Schüler Fächer unter `Schüler > Zeugnis > Fächer` existieren, wenn ja wird die Fachwahl nicht übernommen. Hat der Schüler keine Fächer, werden die Fächer übergeben.|
|![](/images/gym_oberstufe/fw.07.png) |Es werden unter `Schüler > Zeugnis > Fächer` existierende Fächer gelöscht (damit auch ev. bereits erfasste Noten) und die Fächer aus der Fachwahl eingetragen.|
|![](/images/gym_oberstufe/fw.08.png) |Bestehende Fächer auf der Zeugniskarte bleiben erhalten, die Fächer der Fachwahl werden ergänzt. |
|![](/images/gym_oberstufe/fw.09.png) |Bestehende Fächer auf der Zeugniskarte bleiben erhalten, die Fächer der Fachwahl werden ergänzt, der Fachstatus bleibt erhalten.|



### Nutzung der Fachwahlen in Stundenplanprogrammen

Nachdem die Fachwahlen den Fächern der Schüler zugewiesen worden sind, können diese Daten im Stundenplanprogramm DAVINCI oder anderen Stundenplanprogrammen zur weiteren Stundenplanung verwendet werden. Nähre Informationen zum Datenabgleich finden Sie im Kapitel „Stundenplandaten“.

## Die Abiturzulassungsüberprüfung

Die Überprüfung der Abiturzulassung gliedert sich in zwei aufeinander folgende Schritte:

1. Die Überprüfung der Leistungsfachqualifikation. Dieser Punkt entfällt ggf. je nach Bundesland.
2. Die Überprüfung der Abiturzulassung

Diese Schritte werden in den nachfolgenden Abschnitten erläutert.

![Registerkarte „Qualifikation“ in der Ansicht „Abitur“](/images/gym_oberstufe/gym_oberstufe14.png)

> #### warning::Wichtig!
>
>  Überprüfen Sie, ob für den Schüler unter „Prüfungsordnung“ die korrekte Prüfungsordnung eingestellt ist bzw. wählen Sie die entsprechende aus.

Sie können auf der Registerkarte „Qualifikation“ einzelne Spalten ausblenden bzw. die Spaltenüberschrift jeder einzelnen Spalte modifizieren. Klicken Sie dazu auf die Schaltfläche `Layout anpassen…`.

### Was soll berechnet werden?

Stellen Sie den „Status“ auf Leistungsfachqualifikation berechnen oder Gesamtqualifikation berechnen. Beide Berechnungen unterscheiden sich nur darin, dass bei der Berechnung der Leistungsfachqualifikation der GK-Bereich nicht beachtet wird. Markieren Sie anschließend die eingebrachten Kurse. Eingebrachte Kurse werden gelb markiert angezeigt. Sie können die eingebrachten Kurse manuell oder per Automatik markieren.

### Eingebrachte Kurse manuell markieren

Klicken Sie auf `Initialisieren`. Entsprechend des Skripts geschieht beim Initialisieren Folgendes:

Es werden für jeden Kurs automatisch die Halbjahre grau markiert, die für die Abiturzulassung nicht relevant sind. Diese Funktion ist abhängig vom jeweiligen Skript.
Alle anderen Halbjahre des jeweiligen Kurses werden zur Eingabeerleichterung gelb, d.h. „eingebracht“ markiert. Sie brauchen dann nur noch auf `Manuelles Markieren` zu klicken und diejenigen Kurse zu demarkieren, die nicht eingebracht werden sollen.

Markieren Sie die eingebrachten Kurse des Schülers, d.h. markieren Sie `Manuelles Markieren`, wählen Sie die Option `Kurse einbringen` und klicken Sie die entsprechenden Kurse an. Die eingebrachten Kurse werden gelb markiert.

> #### primary::Hinweis
>
> Das letzte Halbjahr im Leistungskursbereich darf bei Skripten mit Leistungs- und Grundkursunterscheidung nicht als „eingebracht“ markiert werden. Es wird automatisch in den Prüfungsbereich übernommen und geht somit in die Berechnung ein.

### Die Vorschlagsautomatik

Wenn Sie auf `Vorschlag `klicken, dann werden von der Vorschlagsautomatik entsprechend der Abiturverordnung die Kurse automatisch gelb markiert, die die maximale Qualifikationspunktzahl in den ersten beiden Qualifikationsbereichen erbringen.

> #### warning::Wichtig!
>
>  Voraussetzung für die Vorschlagsautomatik ist, dass Sie über die Angaben in der Spalte „Fachstatus“ die vier - bzw. in einigen Bundesländern fünf - Prüfungsfächer bestimmt haben.

Die Vorschlagsautomatik des jeweiligen Skriptes generiert einen Vorschlag für die maximale Qualifikationssumme des Schülers. STÜBER SYSTEMS hat die Vorschlagsautomatik sorgfältig an die offiziellen Bestimmungen angepasst und arbeitet ggf. Novellierungen der Bestimmungen in die Skripte ein. STÜBER SYSTEMS übernimmt allerdings keine Garantie für die Richtigkeit des Vorschlags.

### Zulassung berechnen

Klicken Sie auf `Neu berechnen`, um die Zulassung automatisch durch das entsprechende Skript berechnen zu lassen. Im Meldungsfenster werden die Qualifikationspunktzahl für den LK- und den GK-Bereich (letzteres nur bei `Gesamtqualifikation berechnen`) sowie evtl. Fehler angezeigt. Wenn Sie auf `Vorschlag `geklickt haben, ist das Meldungsfenster bereits geöffnet und die Qualifikation berechnet worden. Liegt die Summe beider Bereiche über der Mindestpunktzahl und sind keine weiteren Fehler ausgewiesen, dann ist die Abiturzulassung erreicht.

![Meldungsfenster mit Fehlermeldungen zur Abiturzulassung](/images/gym_oberstufe/gym_oberstufe15.png)

Die Hinweise bzw. Fehlermeldungen im Meldungsfenster sind abhängig vom verwendeten Skript. Fehler führen dazu, dass die Zulassung nicht erreicht ist.

> #### success::Tipp
>
> Klicken Sie auf die Schaltfläche `Meldungen anzeigen`, wenn Sie das Meldungsfenster anzeigen wollen, ohne auf `Vorschlag` oder auf `Neu berechnen` klicken zu müssen.

Außerdem werden automatisch folgende Berechnungen bzw. Eingaben auf der Registerkarte „Prüfung“ durchgeführt:

* Der „Status“ wird auf „Leistungsfachqualifikation erreicht“ oder „Leistungsfachqualifikation nicht erreicht“ bzw. „Gesamtqualifikation erreicht“ oder „Gesamtqualifikation nicht erreicht“ umgesetzt.

* Die Summen der Punkte der einzelnen Halbjahre auf der Registerkarte „Qualifikation“ werden berechnet und in der Spalte „Summe“ angezeigt.

* Die Prüfungsfächer 1 bis 4 (bzw. 5) werden auf der Registerkarte „Prüfung“ eingetragen.

* Die Noten aus 13 werden auf der Registerkarte „Prüfung“ eingetragen.

### Zulassungsdaten manuell eingeben

Wenn Sie die Zulassungsdaten nicht skriptgesteuert eingeben möchten, können Sie die durch das Skript gemachten Eingaben auch selbst vornehmen:

1. Setzen Sie den „Status“ auf „Qualifikation erreicht“ oder „Qualifikation nicht erreicht“.

2. Tragen Sie die Summen je Fach in der Spalte „Summe“ auf der Registerkarte „Qualifikation“ ein.

3. Tragen sie die Prüfungsfächer 1 bis 4 (bzw. 5) auf der Registerkarte „Prüfung“ ein.

4. Tragen Sie die Noten aus 13 auf der Registerkarte „Prüfung“ ein.

### Kurse nicht auf dem Zeugnisausdruck drucken

Kurse des Schülers, die nicht auf dem Abiturzeugnis erscheinen sollen, müssen Sie entsprechend markieren. Markieren Sie dazu Manuelles Markieren, wählen Sie die Option `Nicht auf Zeugnis drucken` und klicken Sie die entsprechenden Kurse an. Die ausgenommenen Kurse werden standardmäßig grau markiert.

> #### primary::Hinweis
>
> Die Farben in der Oberstufe im Menü „Abitur“ sind individuell einstellbar. Unter `Extras > Farben…` legen Sie fest, welche Hintergrundfarben in der Ansicht verwendet werden sollen.

## Der Simulationsmodus

Wenn Sie z.B. für einen Schüler die eingebrachten Kurse verändern möchten, um eine neue Einbringungsvariante durchzuspielen, können Sie dazu den Simulationsmodus in MAGELLAN verwenden. Klicken Sie auf `Bearbeiten > Simulation` oder die entsprechende Schaltfläche oben in der Symbolleiste, um das Simulationsfenster zu öffnen. Das Simulationsfenster umfasst die Registerkarten „Qualifikation“ und „Prüfung“. Wenn Sie die Simulation beenden möchten, klicken Sie auf die Schaltfläche `Simulation beenden`. Sie werden dabei in einem Dialogfenster gefragt, ob Sie die Änderungen dauerhaft übernehmen möchten.

## Die Gesamtqualifikation

Die Berechnung der Gesamtqualifikation bzw. der Abiturnote wird auf der Registerkarte „Prüfung“ durchgeführt.

![Registerkarte „Prüfung“ in der Ansicht „Abitur“](/images/gym_oberstufe/gym_oberstufe16.png)

Die Gesamtqualifikation ergibt sich, indem zusätzlich zu der schon feststehenden Qualifikation im Leistungs- und Grundfachbereich die Qualifikation im Prüfungsbereich durch die Noten im schriftlichen und mündlichen Abitur festgestellt wird. Sie erfolgt in zwei Schritten:

1. Eingabe der schriftlichen Abiturnoten und Qualifikationsüberprüfung für das schriftliche Abitur
2. Eingabe der mündlichen Abiturnoten und Abiturnotenberechnung

> #### primary::Hinweis
>
> Einige Bundesländer haben fünf Prüfungsfächer. Standardmäßig werden 4 Prüfungsfächer angezeigt. Sie können die Anzeige auf fünf Prüfungsfächer erweitern, indem Sie auf die Schaltfläche Layout anpassen klicken.

### Layout anpassen

Sie können die Anzahl der angezeigten Prüfungsfächer auf fünf und die Anzahl der angezeigten Teilnoten für die besondere Lernleistung auf vier erweitern, indem Sie das Fenster `Abiturprüfung anpassen`  über die Schaltfläche `Layout anpassen` aufrufen und im entsprechenden Dialogfenster die Einstellungen machen.

### Schriftliche Prüfungsdaten pro Schüler oder pro Fach und Lehrer eingeben

Für die Eingabe der schriftlichen Prüfungsnoten stehen Ihnen zwei Varianten zur Auswahl: Sie tragen die Noten pro Schüler unter `Abitur > Prüfungen` ein oder Sie nutzen den Assistenten `Schriftliche Prüfungsnoten...`.

Für die Eingabe pro Schüler machen Sie auf der Registerkarte „Prüfung“ folgende Angaben:

1. Geben Sie ggf. die Noten aus 13 ein. Wenn Sie auf der Registerkarte „Qualifikation“ auf Neu berechnen klicken, werden automatisch die angegebenen Prüfungsfächer und die Noten aus 13 auf diese Registerkarte übertragen.
2. Geben Sie die schriftlichen Noten ein.
3. Geben Sie ggf. das Thema und die Punktzahl der besonderen Lernleistung ein.
4. Geben Sie ggf. das Fach der Fachpraxisprüfung und die entsprechende Note ein.
5. Markieren Sie die Sprachkenntnisse.
6. Kontrollieren Sie, ob der „Status“ auf „Gesamtqualifikation erreicht“ steht. Stellen Sie ihn andernfalls manuell ein. Dieser Status wird in der Regel durch Neu berechnen durch das Skript eingestellt.

Für die Eingabe mit Hilfe des Assistenten `Schriftliche Prüfungsnoten...` gehen Sie bitte wie folgt vor:

1. Lösen Sie bitte unter `Abitur > Qualifikation` den Punkt `Neu Berechnen` aus, damit die Prüfungsfächer vorbelegt sind
2. Starten Sie den Assistenten unter `Abitur > Prüfung > Schriftliche Prüfungsnoten`
3. Wählen Sie ein Prüfungsfach aus, die Fächer werden nach den unterrichtenden Lehrern getrennt aufgelistet.

![Auswahl des Faches](/images/gym_oberstufe/gym_oberstufe17.png)

Ihnen werden alle Schüler gezeigt, die dieses Fach als Prüfungsfach beim gleichen Lehrer haben. Für die Eingabe kann nach der Unterrichtsart und dem Fachstatus gefiltert werden.

![Eingabeliste für die schriftlichen Prüfungsnoten](/images/gym_oberstufe/gym_oberstufe18.png)


| Spalte                      | Bedeutung                                |
|-----------------------------|------------------------------------------|
| Spalte Note                 | Wenn für Schüler bereits schriftliche Prüfungsnoten für dieses Fach erfasst wurden, werden diese in der Spalte Note gezeigt. Ändern Sie diese Note, wird sie nach dem Beenden des Assistenten auf der Karte Prüfung als schriftliche Note gezeigt. |
| Spalten Prüfer1 und Prüfer2 | Nutzen Sie diese beiden Spalten um eine höhere Genauigkeit für die Notenerfassung zu erzielen. Lassen Sie dazu Ihre Prüfer die Noten jeweils in die Spalten Prüfer1 und Prüfer2 eintragen – die Spalte Note wird nur gefüllt, wenn beide Noten identisch sind. Beide Spalten lassen sich jeweils Layout anpassen ein- oder ausblenden. |



### Die besondere Lernleistung

Geben Sie auf der Registerkarte „Prüfung“ das Fach (nur bestimmte Bundesländer), Thema und Punktzahl der besonderen Lernleistung ein, falls eine vorliegt. Die Anzahl der Bewertungen können Sie ggf. (je nach Bundesland) auf maximal vier Punktzahlen erweitern (siehe „Layout anpassen“). Markieren Sie „Lernleistung einbringen“, falls die Lernleistung eingebracht werden soll. Wenn Sie auf „Neu berechnen“ klicken, um die Prüfungsqualifikation zu berechnen, prüft das Skript automatisch, ob eine besondere Lernleistung vorliegt und ob es besser wäre, die Lernleistung einzubringen oder nicht. Ggf. wird ein Hinweis im Meldungsfenster ausgegeben, der Sie darauf hinweist, die Lernleistung besser einzubringen bzw. nicht einzubringen.

### Fachpraxisprüfung

Geben Sie auf der Registerkarte „Prüfung“ das Fach und die Note der Fachpraxisprüfung ein, falls eine vorliegt (z.B. in Rheinland-Pfalz).

### Prüfungsqualifikation für das schriftliche Abitur automatisch berechnen

Klicken Sie auf `Neu berechnen`, um die Qualifikation im Prüfungsbereich automatisch durch das entsprechende Skript berechnen zu lassen. Im Meldungsfenster unten werden die Qualifikationspunktzahl in den drei Bereichen, die Gesamtpunktzahl und die Durchschnittsnote angezeigt. Solange keine Note für das mündliche Prüfungsfach eingetragen wurde, wird angezeigt, welche Mindestpunktzahl in der mündlichen Prüfung erreicht werden muss, damit das Abitur bestanden ist. Wenn als Mindestpunktzahl Null angezeigt wird, ist das Abitur bereits unabhängig von der mündlichen Note bestanden. Außerdem werden automatisch folgende Berechnungen bzw. Zuordnungen durchgeführt:

* Der „Status“ wird auf der Registerkarte auf „Abitur bestanden“ oder „Abitur nicht bestanden“ umgesetzt.
* Die Summen für die Prüfungsfächer 1 bis 4 werden berechnet und auf der Registerkarte eingetragen.
* Die Gesamtpunktzahl wird auf der Registerkarte eingetragen.
* Die Durchschnittsnote wird auf der Registerkarte eingetragen.

### Abiturnote berechnen

Nach dem mündlichen Abitur tragen Sie die mündlichen Prüfungsnoten auf der Registerkarte „Prüfung“ ein. Klicken Sie danach wieder auf `Neu berechnen`, um die Abiturnote zu berechnen.

> #### primary::Hinweis
>
> Über die Schaltfläche „Sammelzuweisung“ können Sie mehreren Abiturienten das gleiche Konferenz- bzw. Zeugnisdatum zuweisen.

### Prüfungsqualifikationsdaten manuell eingeben

Wenn Sie die Gesamtqualifikation nicht skriptgesteuert eingeben möchten, können Sie die durch das Skript gemachten Eingaben auch selbst vornehmen:

1. Setzen Sie den „Status“ auf Abitur bestanden oder Abitur nicht bestanden um.
2. Geben Sie die Summen für die Prüfungsfächer 1 bis 4 ein.
3. Geben Sie die Gesamtpunktzahl ein.
4. Geben Sie die Durchschnittsnote ein.

### Zeugnisbemerkungen eingeben

Geben Sie auf der Registerkarte „Zeugnis“ evtl. Zeugnisbemerkungen ein, die auf dem Abiturzeugnis gedruckt werden sollen. Sie können die Zeugnisbemerkung eintippen, auf das Verzeichnis Zeugnisbemerkungen zugreifen und die Rechtschreibprüfung nutzen. Bitte lesen Sie dazu auch den Abschnitt [Zeugnisbemerkungen](https://doc.magellan6.stueber.de/howto/zeugnisdaten.html#zeugnisbemerkungen).

## Oberstufenzeugnisse

Bei der Ausgabe der Zeugnisse in der Oberstufe muss man zwischen zwei Arten von Zeugnissen unterscheiden:
Zeugnisse des aktuellen Zeitraums: Hierbei handelt es sich um Halbjahres- oder Jahreszeugnisse wie z.B. das Zeugnis der Jahrgangsstufe 12/1 oder der Jahrgangsstufe 12/2. Sie beziehen sich immer auf den aktuell eingestellten Zeitraum in MAGELLAN.

Zeugnisse über mehrere Zeiträume: Diese Zeugnisse beziehen sich auf Daten aus mehreren Zeiträumen. Im Fall der Oberstufe werden diese Daten im Bereich „Abitur“ in MAGELLAN eingetragen. Beispiele für zeitraumübergreifende Zeugnisse sind das Fachhochschul-, das Abiturzeugnis oder die Punktekreditkarte.

### Zeugnisse des aktuellen Zeitraums

Die Ausgabe der Zeugnisse des aktuellen Zeitraums erfolgt analog zum Drucken von Standardzeugnissen in MAGELLAN. Die Eingabe der für den Zeugnisausdruck relevanten Daten des Schülers entspricht dem Vorgehen aus Kapitel [Zeugnisdaten erfassen](https://doc.magellan6.stueber.de/howto/zeugnisdaten.html#zeugnisdaten-erfassen).

### Zeugnisse über mehrere Zeiträume

Klicken Sie bei den Abiturdaten des Schülers auf die Registerkarte „Abiturzeugnis“, um die Zeugnisbemerkungen anzugeben. Zusammen mit den Angaben auf den Registerkarten Abiturzulassung und Abiturprüfung verfügen Sie dann über alle Daten, um zeitraumübergreifende Zeugnisse wie das Abiturzeugnis auszudrucken. So drucken Sie Abitur-, Fachhochschulzeugnisse, Punktekreditkarten:

1. Markieren Sie in der Liste der Schüler der Oberstufe per Mausklick oder mit Umschalt+Mausklick oder Strg+Mausklick die entsprechenden Schüler.

2. Klicken Sie auf `Bearbeiten` und `Drucken `und wählen Sie das Zeugnisformular und klicken Sie auf `Drucken`.

