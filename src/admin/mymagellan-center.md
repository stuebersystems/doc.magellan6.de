# Das MYMAGELLAN CENTER

Das MYMAGELLAN CENTER ist das zentrale Administrationswerkzeug zur dezentralen Noteneingabe über MYMAGELLAN. Es dient der Verteilung der Daten pro MYMAGELLAN-Teilnehmer in jeweils eine MYMAGELLAN-Datei (Export aus Magellan) und dem späteren Einsammeln der vom MYMAGELLAN-Teilnehmer modifizierten MYMAGELLAN-Dateien (Import nach Magellan).

Im Rahmen der Installation von Magellan erfolgt auch die Installation des MYMAGELLAN CENTERs. Um das MYMAGELLAN CENTER zu starten, gehen Sie wie folgt vor:

1. Klicken Sie auf Start, dann auf Programme und dann auf STÜBER SYSTEMS.

2. Klicken Sie auf MYMAGELLAN CENTER 6.

3. Tippen Sie Ihre Kennung und Ihr Kennwort ein und bestätigen Sie mit OK (Wenn Sie Magellan neu installiert haben, dann tippen Sie unter Kennung „sysdba“ und das Kennwort „masterkey“ ein).

![Das MYMAGELLAN CENTER](/images/mym_01.start.png)


MYMAGELLAN ist ein Programm zur dezentralen Notenerfassung für die Benutzer von Magellan. Es besteht aus zwei Programmenteilen:

* **MYMAGELLAN CENTER:** Dient dem Administrator zum Erzeugen und späteren Einsammeln von jeweils einer MYMAGELLAN-Datei pro MYMAGELLAN-Teilnehmer. Diese MYMAGELLAN-Datei enthält nur die für den Teilnehmer aufgrund seiner Benutzerrechte relevanten Daten auf Basis der Magellan-Datenbank.

* **MYMAGELLAN:** Dient dem MYMAGELLAN-Teilnehmer zur Eingabe seiner Noten. Er verwendet dazu die vom Administrator zuvor erzeugte MYMAGELLAN-Datei.

Im Unterschied zur zentralen Noteneingabe an der Schule über die Magellan-Clients kann so jeder Teilnehmer von MYMAGELLAN seine Noten auf einem beliebigen PC eingeben. Er benötigt dazu lediglich die vom MYMAGELLAN CENTER erzeugte MYMAGELLAN-Datei und muss MYMAGELLAN auf seinem PC installieren. Die MYMAGELLAN-Datei dient somit dem Datenaustausch zwischen MYMAGELLAN und der Magellan-Datenbank.

![Übersichtsschema zu MYMAGELLAN](/images/mym_00.1ablauf.png)


> #### primary::Hinweis
>
> In diesem Abschnitt werden ausschließlich die Aufgaben für das MYMAGELLAN CENTER aus Sicht des Administrators vorgestellt. Weitere Information zu MYMAGELLAN finden Sie im Dokument [MYMAGELLAN](https://doc.MYMAGELLAN6.stueber.de/) .

Die Nutzung von MYMAGELLAN kann in drei Hauptschritte unterteilt werden:

**Erster Schritt:** Verteilen der MYMAGELLAN-Dateien für alle MYMAGELLAN-Teilnehmer durch das MYMAGELLAN CENTER (Aufgabe des Administrators)

![Verteilen der MYMAGELLAN-Dateien durch das MYMAGELLAN CENTER](/images/mym_00.2ablauf.png)


**Zweiter Schritt:** Nutzung der MYMAGELLAN-Dateien in MYMAGELLAN zur Eingabe der Noten (Aufgabe des MYMAGELLAN-Teilnehmers)

![Noteneingabe in MYMAGELLAN auf Basis der MYMAGELLAN-Datei](/images/mym_00.3ablauf.png)


**Dritter Schritt:** Einsammeln der von MYMAGELLAN nach der Noteneingabe aktualisierten MYMAGELLAN-Dateien der MYMAGELLAN-Teilnehmer (Aufgabe des Administrators)

![Einsammeln der MYMAGELLAN-Dateien durch das MYMAGELLAN CENTER nach Magellan](/images/mym_00.4ablauf.png)


Die nachfolgenden Beschreibungen beziehen sich auf das MYMAGELLAN CENTER in der Version „Professional“. Diese Version besitzt gegenüber dem MYMAGELLAN CENTER „Standard“ einige Zusatzfunktionen. Auf die Unterschiede zur Professional Version wird an den entsprechenden Stellen im Text mit [bei „Standard“ nicht enthalten] hingewiesen.

## Voraussetzungen

Voraussetzungen für die Nutzung des MYMAGELLAN CENTERs sind:
* die Definition der MYMAGELLAN-Teilnehmer in der Benutzerverwaltung des Magellan-Administrators
* die Eingabe der Stammdaten der Schüler
* die Zuordnung der MYMAGELLAN-Teilnehmer zu den Schülern in Magellan


### Benutzerverwaltung

Jeder MYMAGELLAN-Teilnehmer muss als Benutzer in der Benutzerverwaltung angelegt sein. Dabei muss er folgende Bedingungen erfüllen:
* Der Benutzer muss unter „Schulverwaltung“ der Benutzergruppe „Schulleitung 1“, „Schulleitung 2“, „Sekretariat 1“, „Kollegium 1“, „Kollegium 2“, „Kollegium 3“ oder „Kollegium 4“ zugeordnet sein.

* Der Benutzer muss unter „MYMAGELLAN“ den Status „Teilnehmer von MYMAGELLAN“ besitzen.

* Dem Benutzer muss unter „MYMAGELLAN“ eine „MYMAGELLAN-Datei“ (Datei mit der Endung .mym) zugeordnet werden. Die Datei muss lediglich benannt werden, jedoch nicht notwendigerweise schon existieren. Die Zuordnung der MYMAGELLAN-Datei kann auch alternativ im MYMAGELLAN CENTER erfolgen. Bitte achten Sie darauf, dass Sie mit dem Lupensymbol den kompletten Pfad aussuchen. Wenn Sie lediglich eine Dateibezeichnung eintragen, führt dies später zu einer Fehlermeldung, da der Speicherort nicht gefunden wird. Nur Benutzer mit diesen Rechten werden im MYMAGELLAN CENTER angezeigt.

* Dem Benutzer kann unter „MYMAGELLAN“ ein MYMAGELLAN-Kennwort zugeordnet werden. Mit dieem Kennwort wird dann die erstellte der MYMAGELLAN-Datei geschützt.

### Stammdaten der Schüler

Alle Schüler, deren Noten über MYMAGELLAN erfasst werden sollen, müssen in Magellan erfasst sein. Hierzu zählt neben der eigentlichen Definition des Schülers auch dessen Zuordnung zu einer Klasse. Zusätzlich müssen den Schülern Fächer zugeordnet werden, deren Noten mit MYMAGELLAN erfasst werden sollen, da eine Eingabe der Fächer in MYMAGELLAN nicht möglich ist.

### Zuordnung der MYMAGELLAN-Teilnehmer zu den Schülern

Die Zuordnung der MYMAGELLAN-Teilnehmer zu den Schülern erfolgt über die Aufgaben der Teilnehmer in der Schule:

* Klassenleiter 1: Der Lehrer ist in mindestens einer Klasse Klassenleiter 1 im aktuellen Zeitraum. In diesem Fall werden alle Schüler in die MYMAGELLAN-Datei exportiert, deren Klassenleiter 1 der Teilnehmer ist.

![Zuordnung des Klassenleiters 1 bei einer Klasse auf der Registerkarte „Zeiträume“. Die Zuordnung erfolgt pro Zeitraum.](/images/mym_02.klassenzeitraeume.png)


* Fachlehrer: Der Lehrer ist bei mindestens einem Schüler Fachlehrer. Dazu muss er bei den Zeugnisdaten des Schülers auf der Registerkarte Fächer in der Spalte Lehrer als Fachlehrer für das jeweilige Fach eingetragen sein.

![Zuordnung der Fachlehrer bei einem Schüler in der Spalte „Lehrer“ bei den Fächern.](/images/mym_03.schueler.faecher.png)

* Tutor: Der Lehrer ist bei mindestens einem Schüler als Tutor zugeordnet. Dies ist beispielsweise in der gymnasialen Oberstufe der Fall, wenn der Tutor den Stammkursleiter darstellt.


![Zuordnung des Tutors auf der Registerkarte „Zeugnis|Details“ des Schülers.](/images/mym_04.details.png)

Ist ein MYMAGELLAN-Teilnehmer im aktuellen Zeitraum weder Klassenleiter 1, noch Fachlehrer, noch Tutor, wird für ihn keine MYMAGELLAN-Datei durch das MYMAGELLAN CENTER erzeugt.

## MYMAGELLAN-Dateien verteilen

Sind alle Voraussetzungen für die Erstellung der MYMAGELLAN-Dateien erfüllt, werden nach dem Start des MYMAGELLAN CENTERs alle MYMAGELLAN-Teilnehmer aufgelistet.

> #### primary::Hinweis
>
> Vor dem eigentlichen Verteilen der MYMAGELLAN-Dateien, sollten Sie nochmals überprüfen, ob für jeden Teilnehmer der Speicherort und der Dateiname für seine MYMAGELLAN-Datei vordefiniert wurde. Wenn dies noch nicht über die Benutzerverwaltung des MAGELLAN ADMINISTRATORs erfolgt ist, können Sie diese Vorgaben auch im MYMAGELLAN CENTER definieren.

![Geben Sie für jeden Nutzer einen Speicherort und einen Dateinamen für seine Datei vor](/images/mym_12.mympfad.png)


So starten Sie die Verteilung der MYMAGELLAN-Dateien:

1. Markieren Sie die Teilnehmer, deren MYMAGELLAN-Dateien Sie verteilen wollen.

2. Klicken Sie auf `Umgebung` und dann auf `Daten verteilen`.

![Assistent zum Verteilen der MYMAGELLAN-Dateien.](/images/mym_05.daten.verteilen.png)

3. Klicken Sie im Assistenten auf `Weiter`.


![Hier wählen Sie den Zeitraum zum Verteilen der MYMAGELLAN-Dateien fest.](/images/mym_06.zeitraum.auswaehlen.png)

5. Legen Sie den Exportfilter fest. Haken Sie hierzu die entsprechende Option an.

![Hier legen Sie den Exportfilter fest.](/images/mym_07.exportfilter.waehlen.png)

6. Markieren Sie optional die zu filternden Klassen, d.h. legen Sie fest, ob nur Schüler bestimmter Klassen in die MYMAGELLAN-Dateien exportiert werden sollen. Klicken Sie dann auf `Weiter`.

7. [bei „Standard“ nicht enthalten] Legen Sie das Layout der Noteneingabe in MYMAGELLAN fest. Markieren Sie dazu, welche Spalten für den Nutzer der MYMAGELLAN-Datei in MYMAGELLAN sichtbar sein sollen. Klicken Sie dann auf `Weiter`.

![Hier legen Sie das Layout der MYMAGELLAN-Dateien fest.](/images/mym_08.layout.festlegen.png)

8. Legen Sie die anzuzeigen Zusatzdaten MYMAGELLAN fest. Markieren Sie dazu, welche Zusatzdaten für den Nutzer der MYMAGELLAN-Datei in MYMAGELLAN sichtbar und editierbar sein sollen. Klicken Sie dann auf `Weiter`.

![Hier legen Sie die Zusatzdaten für die MYMAGELLAN-Dateien fest.](/images/mym_09.zusatzdaten.png)

9. [bei „Standard“ nicht enthalten] Legen Sie die Editierbarkeit der Spalten „Position“, „Merkmal“, „Fachstatus“, „Unterrichtstart“, „Niveau“ und „Mahnung“ der MYMAGELLAN-Datei(en) fest. Zusätzlich können Sie angeben, ob bei Fachlehrern optional die Registerkarte „Weitere Daten“ in MYMAGELLAN ausgeblendet werden soll. Für die Verarbeitung der Fehlstunden, Fehlstunden unentschuldigt, Fehltage und Fehltage unentschuldigt beim späteren Einlesen der MYMAGELLAN-Dateien können Sie zusätzlich folgende Einstellungen auswählen:

* Fehlstunden/-tage in Magellan beim Einsammeln überschrieben: Die Werte der Felder „Fehlstunden“, „Fehlstunden unentschuldigt“, „Fehltage“ und „Fehltage unentschuldigt“ des Schülers in Magellan werden durch Einlesen einer MYMAGELLAN-Datei, mit Daten zu diesem Schüler überschrieben. Ausnahme: Kein Eintrag oder ein Null in MYMAGELLAN überschreiben keinen Wert in MAGELLAN. Eine Korrektur des verkehrten Wertes aus MAGELLAN ist nur im Schulverwaltungsprogramm selbst möglich.

* Fehlstunden/-tage in Magellan beim Einsammeln addieren: Die Werte der Felder „Fehlstunden“, „Fehlstunden unentschuldigt“, „Fehltage“ und „Fehltage unentschuldigt“ des Schülers in Magellan werden durch Einlesen einer MYMAGELLAN-Datei, mit Daten zu diesem Schüler addiert. Bitte beachten Sie, dass bei dieser Option im Fall eines erneuten Importes der Datei auch die Fehlzeiten erneut addiert werden.

* Fehlstunden/-tage in Magellan beim Einsammeln nicht aktualisieren: Die Werte der Felder „Fehlstunden“, „Fehlstunden unentschuldigt“, „Fehltage“ und „Fehltage unentschuldigt“ des Schülers in Magellan werden durch Einlesen einer MYMAGELLAN-Datei nicht verändert. Klicken Sie dann auf `Weiter`.


10. [bei „Standard“ nicht enthalten] Legen Sie optional das Kennwort der MYMAGELLAN-Datei(en) fest für die Benutzer fest, die noch keine MYMAGELLAN-Kennwort besitzen und klicken Sie dann auf `Weiter`.

![Hier legen Sie das pauschale Kennwort für Benutzer ohne MYMAGELLAN-Kennwort fest.](/images/mym_10.kennwort.png)

11. Geben Sie optional eine Bemerkung an, die beim Öffnen der MYMAGELLAN-Datei(en) sichtbar sein soll und klicken Sie dann auf `Weiter`.

12. Klicken Sie abschließend auf Starten, um das Verteilen der Dateien zu starten.

13. Mit jeder Erstellung einer MYMAGELLAN-Datei über den Assistenten werden nur die Daten pro Teilnehmer aus der MAGELLAN-Datenbank in die MYMAGELLAN-Datei exportiert, die für den Teilnehmer aufgrund seiner Aufgaben in der Schule (Klassenleiter 1, Fachlehrer oder Tutor) relevant sind. Sind die MYMAGELLAN-Dateien in den festlegten Ordnern erstellt, so wird in der Statusspalte das Symbol angezeigt. Zusätzlich wird das Datum in der Spalte „Letzter Export“ gesetzt.

> #### primary::Hinweis
>
> Bitte beachten Sie, dass für den Benutzer der MYMAGELLAN-Datei ausgeblendete Felder weiterhin mit Werten versehen sind. Diese Werte werden beim Zurückspielen der MYMAGELLAN-Dateien in die Quelldatenbank übernommen. Zwischenzeitliche Änderungen in der Quelldatenbank werden dabei überschrieben.
Und: Zeugnisbemerkungen werden nur von Klassenleitern und Tutoren nach Magellan übernommen.

## Noteneingabe über MYMAGELLAN

Die Noteneingabe in MYMAGELLAN ist der gesonderten Dokumentation [MYMAGELLAN](https://doc.MYMAGELLAN6.stueber.de/) zu entnehmen.

## Importlogik

Nachstehend wird beschrieben was genau beim Import passiert, falls Daten in MAGELLAN und/oder in in MYMAGELLAN vorhanden sind.

### Noten

Stand in MAGELLAN/MYMAGELLAN |Was passiert beim Import?
---|---
Note ist in MAGELLAN /keine Note in MYMAGELLAN| Note in MAGELLAN bleibt bestehen
Note ist nicht in MAGELLAN, Note ist in MYMAGELLAN| Note aus der MYMAGELLAN-Datei wird eingelesen
Noten sind in beiden Programmen|Note aus MYMAGELLAN wird eingelesen

> #### warning::Wichtig!
>
> Das bedeutet, wenn in MAGELLAN eine Note besteht, die Sie in der MYMAGELLAN-Datei entfernen, dann bleibt die Note weiterhin nach dem Einlesen in MAGELLAN bestehen.


### Beurteilungen

Gemeint sind die Beurteilungen unter `Schüler > Zeugnis > Leistungen` im Feld `Beurteilungen`. Hier können zusätzlich zur Benotung (per Punkt- oder Notenwert) schriftliche Beurteilungen pro Fach erfolgen.

Stand in MAGELLAN/MYMAGELLAN |Ergebnis
---|---
Beurteilung ist in MAGELLAN /keine Beurteilung in MYMAGELLAN| Beurteilung in MAGELLAN bleibt bestehen
Beurteilung ist nicht in MAGELLAN, Beurteilung ist in MYMAGELLAN| Beurteilung aus der MYMAGELLAN-Datei wird eingelesen
Beurteilung sind in beiden Programmen|Beurteilung aus MYMAGELLAN wird eingelesen

> #### primary::Hinweis
>
> Beispiel: Sie verteilen die Daten für Fachlehrer und Klassenleiter gleichzeitig, es ist beispielsweise die Fachzeile für Mathematik eines Schülers in der Fachlehrerdatei und in der Klassenleiterdatei. 
>**Die Eintragungen beider Rollen werden beim Import gleichwertig behandelt.** 
>Trägt nur einer der beiden in seine Datei eine Leistungsbeurteilung für Mathe ein, wird dessen Eintragung nach MAGELLAN importiert. 
>Tragen beide Kollegen (also der Fachlehrer und der Klassenlehrer tragen etwas für die Mathezeile ein) ein oder wurde bereits eine Eintragung in die MYMAGELLAN-Dateien exportiert, werden die Eingaben nacheinander importiert, die zuletzt importierte Information bleibt in MAGELLAN bestehen.   


### Zeugnisbemerkungen

Stand in MAGELLAN/MYMAGELLAN |Ergebnis
-|-
Bemerkung in MAGELLAN existiert, MYMAGELLAN-Datei wird erzeugt|Bemerkung wird mit in die MYMAGELLAN-Datei übergeben
Bemerkung wird in MYMAGELLAN aktualisiert<br/>Bemerkung wird in MAGELLAN neu angelegt|Bemerkungen werden beim Import in MAGELLAN gelöscht und durch aktualisierte oder neue Bemerkungen aus MYMAGELLAN ersetzt
Neue Bemerkung wird in MAGELLAN erfasst,<br/>während die MYMAGELLAN-Dateien ausgeteilt sind|Bemerkungen wird beim Import in MAGELLAN gelöscht und durch aktualisierte oder neue Bemerkungen ersetzt. Sind keine neuen Bemerkungen in MYMAGELLAN erfasst worden, können als Ergebnis auch KEINE Bemerkungen übrig bleiben.

> #### danger::Achtung!
>
>Beim Erstellen der MYMAGELLAN-Dateien werden bereits in MAGELLAN existierende Zeugnisbemerkungen in die Lehrer-/Tutorendateien mit ausgegeben. Um beim Import keine Dopplungen von Bemerkungen zu erzielen werden beim Einlesen der Klassenleiterdatei und der Tutorendatei jeweils zuvor die Schülerzeugnisbemerkungen gelöscht. Sollten einem Schüler ein Klassenleiter und ein Tutor zugeordnet worden sein, können damit je nach Einlesereihenfolge Zeugnisbemerkungen überschrieben werden.
>
>Beispiel: Schüler S1 wurden Lehrer L1 und Tutor T1 zugeordnet. Beim Erstellen der MYMAGELLAN-Dateien haken Sie versehentlich beide Rollen an, also Klassenleiter und Tutorendatei erstellen. Eventuell in MAGELLAN bereits existente Zeugnisbemerkungen werden für S1 ausgespielt. L1 vergibt eine neue Zeugnisbemerkung, T1 vergibt keine neue Zeugnisbemerkung. Die Dateien von L1 und T1 werden wieder importiert. Import der Datei von L1: Zeugnisbemerkungen werden für S1 gelöscht, neue und alte Zeugnisbemerkung werden aus der Datei von L1 importiert. Als nächstes wird die Datei für T1 importiert: die Zeugnisbemerkungen von S1 werden gelöscht (neue und alte reimportierte Zeugnisbemerkungen), nur die alten Zeugnisbemerkungen werden eingelesen. Im Ergebnis fehlen die neuen Zeugnisbemerkungen von L1. Sie können den Konflikt nur lösen, indem Sie entweder:
> * entweder Schülern nicht einen Klassenleiter UND einen Tutor zuweisen
> * oder falls beide Felder für Schüler vergeben sind, beim Erstellen der Dateien nicht Tutor- und Klassenleiterdateien gemeinsam erstellen, sondern erst die Dateien für die zweite Rolle nach dem Einsammeln der Daten der ersten Rolle verteilen.

### Fehlzeiten

![Bei Fehlzeiten richtet es sich danach, welche Option Sie beim Erzeugen der MYMAGELLAN-Datei gewählt haben.](/images/mym_13.fehlzeitoptionen.png)


Die Option "Fehlstunden/-tage in MAGELLAN beim Einsammeln addieren" ist ungeeignet fürs erneute Einlesen, da die Werte dann wieder aufsummiert werden, also die doppelte Anzahl von Fehlzeiten das Ergebnis wäre.

Gut geeignet ist die Option "Fehlstunden/-tage in MAGELLAN beim Einsammeln überschreiben".

Option|Ergebnis
-|-
Fehlstunden/-tage in MAGELLAN beim Einsammeln überschreiben|Der Eintrag aus der MYMAGELLAN überschreibt den Eintrag in MAGELLAN. <br/> **Ausnahme: Es wird nichts oder eine NULL in MYMAGELLAN erfasst, in diesem Fall bleibt der MAGELLAN-Eintrag erhalten.**
Fehlstunden/-tage in MAGELLAN beim Einsammeln addieren|Fehlstunden/-tage aus allen MYMAGELLAN-Dateien werden aufaddiert. <br/>Bitte beachten Sie, dass das erneute Einlesen einer Datei bei dieser Option auch erneut die Werte addiert.
Fehlstunden/-tage in MAGELLAN beim Einsammeln nicht aktualisieren|Es erfolgt keine Änderung in MAGELLAN.

> #### warning::Wichtig!
>
> [Ab Version 6.5.17] Wird die Option "Fehlstunden/-tage in MAGELLAN beim Einsammeln überschreiben" gewählt, kann ein Eintrag in MAGELLAN nicht auf NULL durch eine entsprechende Eingabe in MYMAGELLAN zurückgesetzt werden!

## MYMAGELLAN-Dateien einsammeln

Nachdem die Noteneingabe der MYMAGELLAN-Teilnehmer erfolgt ist, müssen diese ihre MYMAGELLAN-Dateien wieder in den gleichen MYMAGELLAN-Ordner unter dem gleichen Dateinamen kopieren. Hierbei wird die bestehende, zuvor exportierte MYMAGELLAN-Datei überspielt, wenn sie noch im Ordner vorliegt. Hat die MYMAGELLAN-Datei ein neueres Dateidatum als der letzte Export, so wird in der Statusspalte das Symbol angezeigt. Sie wissen dann direkt, ob der Teilnehmer seine mit MYMAGELLAN bearbeitete MYMAGELLAN-Datei zurückgebracht hat.

So starten Sie das Einsammeln der MYMAGELLAN-Dateien:

1. Markieren Sie die Teilnehmer, deren MYMAGELLAN-Dateien Sie einsammeln wollen.

2. Klicken Sie auf `Umgebung `und dann auf `Daten einsammeln`.

3. Klicken Sie im Assistenten auf `Weiter`.

4. Klicken Sie auf `Fertigstellen` um das Einsammeln zu starten.

**Durch das Einsammeln der MYMAGELLAN-Dateien werden alle entsprechenden Daten in Magellan mit den neuen Werten überschrieben!** Nach dem erfolgreichen Einsammeln wird die Importdatum in der Spalte „Letzter Import“ der jeweiligen MYMAGELLAN-Datei gesetzt und in der Statusspalte wird das Symbol angezeigt. Für die Statusspalte gibt es somit vier Modi.

Statusspalte |Bedeutung
--|--
kein Symbol |Keine MYMAGELLAN-Datei im angegebenen Ordner.
roter Pfeil|MYMAGELLAN-Datei erzeugt: MYMAGELLAN-Datei existiert im angegebenen Ordner.
blauer Pfeil|MYMAGELLAN-Datei bereit zum Import: MYMAGELLAN-Datei existiert im angegebenen Ordner und hat ein jüngeres Dateidatum als das letzte Exportdatum.
grüner Pfeil|MYMAGELLAN-Datei erfolgreich importiert: MYMAGELLAN-Datei existiert im angegebenen Ordner und hat ein älteres Dateidatum als das letzte Importdatum und ein jüngeres Dateidatum als das letzte Exportdatum.

> #### warning::Wichtig!
>
> Beim Einlesen der MYMAGELLAN-Dateien richtet sich das Verhalten beim Import der Felder „Fehlstunden“, „Fehlstunden unentschuldigt“, „Fehltage“ und „Fehltage unentschuldigt“ nach den Einstellungen beim Verteilen der MYMAGELLAN-Dateien.a

## Löschen der MYMAGELLAN-Dateien

Im MYMAGELLAN CENTER können Sie zu einem beliebigen Zeitpunkt die bereits erstellten MYMAGELLAN-Dateien direkt löschen. So löschen Sie MYMAGELLAN-Dateien:

1. Markieren Sie die Teilnehmer, deren MYMAGELLAN-Dateien Sie löschen wollen.

2. Klicken Sie auf `Umgebung `und dann auf `Dateien löschen`.

3. Klicken Sie im Assistenten auf `Weiter`.

4. Klicken Sie auf `Fertigstellen `um das Löschen zu starten.

> #### danger::Achtung!
>
> MYMAGELLAN-Dateien, die mit einer Ausgabe von MYMAGELLAN erstellt wurden, in der es eine Datenstrukturänderung gegeben hatte, lassen sich mit einer aktuelleren Version nicht bearbeiten. Wenn Sie das dennoch versuchen sollten, erhalten Sie den Hinweis, dass die Datei mit einer anderen Version erstellt wurde und dass Sie sich mit Ihrem Administrator in Verbindung setzen möchten. Dies bedeutet, dass die Dateien mit einer neuen Version neu erstellt werden müssen.


## MYMAGELLAN Dateien erneut importieren

Fällt nach dem Import auf, dass noch weitere Änderungen vorzunehmen sind, können MYMAGELLAN-Dateien auch erneut importiert werden.


### Bemerkungen

> #### warning::Wichtig!
>
> Wichtig bei den Bemerkungen, wie eigentlich auch bei allen anderen Zeugnisinformationen ist: Sind die MYMAGELLAN-Dateien beim Lehrer darf nichts in MAGELLAN verändert werden!

Bemerkungen, die später in der MYMAGELLAN-Datei noch ergänzt werden, können einfach ergänzt oder auch bereits eingelesene noch geändert werden.
Beim erneuten Einlesen werden die Bemerkungen in MAGELLAN gelöscht und durch die neu eingelesenen ergänzt. Es würden aber auch Bemerkungen gelöscht, die zwischenzeitlich in MAGELLAN mit eingefügt wurden!!!

### Fehlzeiten

![Bei Fehlzeiten richtet es sich danach, welche Option Sie beim Erzeugen der MYMAGELLAN-Datei gewählt haben.](/images/mym_13.fehlzeitoptionen.png)


Die Option "Fehlstunden/-tage in MAGELLAN beim Einsammeln addieren" ist ungeeignet fürs erneute Einlesen, da die Werte dann wieder aufsummiert werden, also die doppelte Anzahl von Fehlzeiten das Ergebnis wäre.

Gut geeignet ist die Option "Fehlstunden/-tage in MAGELLAN beim Einsammeln überschreiben".


> #### warning::Wichtig!
>
> Kein Eintrag oder eine Null aus den Fehlzeiten in MYMAGELLAN überschreibt keinen MAGELLAN-Eintrag!


## Organisation des zeitlichen Ablaufs

Vor dem Einsatz des MYMAGELLAN CENTERs bzw. von MYMAGELLAN sollten Sie sich ein entsprechendes Ablaufszenario erarbeiten. Dieses könnte beispielsweise wie folgt aussehen:

1. Bekanntgabe des Datums der Erzeugung der MYMAGELLAN-Dateien und der Frist zur Rückgabe der bearbeiteten MYMAGELLAN-Dateien pro Teilnehmer.

2. Bekanntgabe der Frist zur Kopie der MYMAGELLAN-Dateien auf die Datenträger.

3. Nach Ablauf der Rückgabefrist Überprüfung ob alle MYMAGELLAN-Dateien wieder eingespielt worden sind.

4. Einsammeln der MYMAGELLAN-Dateien.

## Mögliche Konflikte

### Konflikte bei Noten aufgrund Klassenlehrer/Tutor/Fachlehrer

Eine Verteilung der MYMAGELLAN-Dateien kann aufgrund der Benutzerrechte evtl. zu Konflikten führen.

Beim Erzeugen der Daten kann beispielsweise ein Schüler A sowohl in der MYMAGELLAN-Datei des Lehrers 1 existieren, weil dieser Klassenleiter 1 der aktuellen Klasse ist, als auch beim Fachlehrer der Klasse, weil dieser den Schüler A z.B. in Deutsch in der gleiche Klassen unterrichtet.

Es ist also organisatorisch festzulegen, wer überhaupt die Noten eingeben soll, um ein Überschreiben der Daten beim späteren Einsammeln zu vermeiden.

Beispielsweise könnten nur die Klassenleiter 1 der Klassen Teilnehmer von MYMAGELLAN sein, so dass nur die Klassenleiter die Noten mit MYMAGELLAN eingeben. Sie sollten daher beim Erzeugen der MYMAGELLAN-Dateien unter Filter genau festlegen, welche Daten in die MYMAGELLAN-Datei pro MYMAGELLAN-Teilnehmer übertragen werden sollen.

### Nicht eingegebene Noten in MYMAGELLAN

Nicht eingegebene Noten in MYMAGELLAN werden beim Einsammeln über das MYMAGELLAN CENTER besonders behandelt.

> #### danger::Achtung!
>
> Nicht eingegebene Noten in MYMAGELLAN werden beim Import nach MAGELLAN nicht berücksichtigt. Bestehende Noten in MAGELLAN werden so durch den Import einer MYMAGELLAN-Datei nicht gelöscht.

Hierbei gilt die Regel:
Ist einem Schüler in MYMAGELLAN für ein Fach keine Note eingetragen worden, so wird diese Note beim Import nach MAGELLAN nicht berücksichtigt. Wird z.B. in MYMAGELLAN für einen Schüler in einem Fach unter „Endnote 1“ keine Note eingetragen und in MAGELLAN ist für denselben Schüler unter „Endnote 1“ eine Note eingetragen, so wird diese durch dem Import nach MAGELLAN nicht überschrieben. 
Dieses Vorgehen ermöglicht die kombinierte Eingabe von Noten.
Unterrichtet beispielsweise der Lehrer L1 die Klasse 8a als Fachlehrer im Fach Deutsch und der Lehrer L2 ist Klassenleiter 1 der Klasse 8a , so ist folgende Konstellation möglich: Lehrer L2 gibt alle Noten bis auf das Fach Deutsch in MYMAGELLAN ein, Lehrer L1 gibt nur die Noten der 8a für das Fach Deutsch in MYMAGELLAN ein. Durch das Einspielen der MYMAGELLAN nach MAGELLAN werden beiden Dateien gemischt, so dass die Noten der Klasse 8a in MAGELLAN vollständig sind.

Dazu müssen Sie wie folgt vorgehen:

1. Lehrer L2 erhält über das Filter „Klassenleiter 1“ seine MYMAGELLAN-Datei. Er trägt in Absprache mit Lehrer L1 alle Noten der Klasse 8a mit Ausnahme des Fachs Deutsch über MYMAGELLAN ein und bringt die veränderte MYMAGELLAN-Datei wieder in die Schule.

2. Lehrer L1 erhält über das Filter „Fachlehrer“ seine MYMAGELLAN-Datei. Er trägt die Noten der Klasse 8a für das Fach Deutsch über MYMAGELLAN ein und bringt die veränderte MYMAGELLAN-Datei wieder in die Schule.

3. Die MYMAGELLAN-Dateien von L1 und L2 werden, unabhängig in welcher Reihenfolge, wieder nach MAGELLAN importiert. Alle Noten der 8a sind nun in MAGELLAN vollständig.

### Konflikt Klassenlehrer/Tutor/Fachlehrer bei „Weiteren Details“

Analog zu den Konflikten bei den Noten können auch Konflikte bei den weiteren Daten auftauchen:

* Unterrichtstage
* Versäumnisse
* Fehltage
* Davon unentschuldigt Fehltage
* Fehlstunden
* davon unentschuldigte Fehlstunden

Zur Konfliktlösung ist Folgendes zu berücksichtigen:

Kann der Lehrer eines Schülers die Registerkarte „Weiteren Daten“ in MYMAGELLAN editieren, so überschreiben in der Standardeinstellung seine Eingaben mit dem Einsammeln seiner MYMAGELLAN-Datei nach MAGELLAN unter grundsätzlich die bestehenden Eintragungen in MAGELLAN für diesen Schüler.

> ####### warning::Wichtig!
>
>Ausnahme: Wenn er keine Eintragungen in diesen Feldern in MYMAGELLAN vorgenommen hat, werden die Werte in MAGELLAN durch die >Eintragungen in MYMAGELLAN nicht überschrieben, wenn die Option beim Verteilen der MyMagelan-Dateien so gewählt wurde. Das >gilt für folgende Werte:
>* Unterrichtstage
>* Versäumnisse
>* Fehltage
>* Davon unentschuldigt Fehltage
>* Fehlstunden
>* davon unentschuldigte Fehlstunden

Beispiel:
Der Lehrer L1 hat beim Schüler S1 in seiner MYMAGELLAN-Datei die Eintragung 2 bei den Fehlstunden gemacht. Der Lehrer L2 hat beim gleichen Schüler S1 in seiner MYMAGELLAN-Datei keine Eintragung (Standardwert=0) gemacht. Wird nun zuerst die MYMAGELLAN-Datei von Lehrer L1 eingelesen, so erhält der Schüler S1 in MAGELLAN den Wert 2 bei Fehlstunden. Wird anschließend die MYMAGELLAN-Datei des Lehrers L2 eingelesen, so bleibt die 2 bestehenen, wird nicht durch die 0 überschrieben. Sollte L2 die Null erfasst haben um einen Eintrag in MAGELLAN zu korrigieren, bleibt der vorherige Wert (> 0) bestehen. Erfasst Lehrer L2 einen anderen Wert, zum Beispiel 3 Fehlstunden, überschreibt die 3 die 2 (entscheidend ist die Reihenfolge des Einlesens).

Zur Konfliktlösung stehen Ihnen vier Möglichkeiten zur Verfügung.

* **Gewünschte Einstellungen bei Fehlstunden/-tage wählen:** Bei der Erstellung der MYMAGELLAN-Dateien über das MYMAGELLAN CENTER geben Sie an, ob die Fehlstunden/-tage beim späteren importieren überschrieben (nicht durch Null oder keinen Eintrag), addiert oder unverändert in MAGELLAN belassen werden. Ein Addieren macht beispielsweise dann Sinn, wenn jeder Fachlehrer nur seine Fehlstunden/-tage des Schüler einträgt.

* **Zeugnisbemerkungen: **Zeugnisbemerkungen werden generell nur aus Klassenleiter- oder Tutorendateien nach MAGELLAN eingelesen, nicht aus Fachlehrerdateien.
Nur Klassenleiter nutzen MYMAGELLAN: Bei der Erstellung der MYMAGELLAN-Dateien über das MYMAGELLAN CENTER werden nur Klassenleiter berücksichtigt (Exportfilter „Teilnehmer ist Klassenleiter 1 des Schülers“ aktiviert). Da ein Schüler nur einen „Klassenleiter 1“ zu einem Zeitraum in MAGELLAN besitzen kann, können die „Weiteren Daten“ eines Schülers nicht von einem anderen Lehrer beim Einlesen der MYMAGELLAN-Dateien überschrieben werden.

* **„Weitere Details“ exklusiv für Klassenleiter:** Bei der Erstellung der MYMAGELLAN-Dateien über das MYMAGELLAN CENTER werden Klassenleiter und Fachlehrer berücksichtigt, wobei die „Weiteren Daten“ nur für den Klassenleiter sichtbar sind (Exportfilter „Teilnehmer ist Klassenleiter 1 des Schülers“ und „Teilnehmer ist Fachlehrer des Schülers“ aktiviert, Editierbarkeit „Register „Weitere Daten“ ist für Fachlehrer sichtbar“ deaktiviert). In diesem Fall kann nur der Klassenleiter das Register “Weitere Daten“ in MYMAGELLAN nur bei den Schülern sehen, bei denen er Klassenleiter ist. Ist er nur Fachlehrer des Schülers, sieht es das Register „Weitere Daten“ in MYMAGELLAN nicht.

* **Unterscheidung von Fall zu Fall: **Bei der Erstellung der MYMAGELLAN-Dateien über das MYMAGELLAN CENTER werden Klassenleiter und Fachlehrer berücksichtigt, wobei die „Weiteren Daten“ für alle Lehrer sichtbar sind (Exportfilter „Teilnehmer ist Klassenleiter 1 des Schülers“ und „Teilnehmer ist Fachlehrer des Schülers“ aktiviert, Editierbarkeit „Register „Weitere Daten“ ist für Fachlehrer sichtbar“ aktiviert). In diesem Fall besteht die potentielle Gefahr, dass die Daten der Lehrer sich in Abhängigkeit von der Reihenfolge des Einlesens in MAGELLAN gegenseitig überschreiben. Man kann jedoch in MYMAGELLAN auf dem Register „Weitere Daten über“ das Optionsfeld „Nur Verhalten und Mitarbeit“ erreichen, dass nur die Felder „Verhalten“ und „Mitarbeit“ von den „Weiteren Daten“ beim Einlesen nach MAGELLAN berücksichtigt werden. Die Berücksichtigung dieser Möglichkeit setzt jedoch eine genaue Absprache zwischen den beteiligten Lehrern und sollte daher nur in Sonderfällen genutzt werden.

## Konflikt zwischen Tutoren und Klassenleitern beim Import von Zeugnisbemerkungen

 Wichtig bei den Bemerkungen, wie eigentlich auch bei allen anderen Zeugnisinformationen ist: Sind die MYMAGELLAN-Dateien beim Lehrer darf nichts in MAGELLAN verändert werden!
 
Beim Erstellen der MYMAGELLAN-Dateien werden bereits in MAGELLAN existierende Zeugnisbemerkungen in die Lehrer-/Tutorendateien mit ausgegeben. Um beim Import keine Dopplungen von Bemerkungen zu erzielen werden beim Einlesen der Klassenleiterdatei und der Tutorendatei jeweils zuvor die Schülerzeugnisbemerkungen gelöscht. Sollten einem Schüler ein Klassenleiter und ein Tutor zugeordnet worden sein, können damit je nach Einlesereihenfolge Zeugnisbemerkungen überschrieben werden.

Beispiel: Schüler S1 wurden Lehrer L1 und Tutor T1 zugeordnet. Beim Erstellen der MYMAGELLAN-Dateien haken Sie versehentlich beide Rollen an, also Klassenleiter und Tutorendatei erstellen. Eventuell in MAGELLAN bereits existente Zeugnisbemerkungen werden für S1 ausgespielt. L1 vergibt eine neue Zeugnisbemerkung, T1 vergibt keine neue Zeugnisbemerkung. Die Dateien von L1 und T1 werden wieder importiert. Import der Datei von L1: Zeugnisbemerkungen werden für S1 gelöscht, neue und alte Zeugnisbemerkung werden aus der Datei von L1 importiert. Als nächstes wird die Datei für T1 importiert: die Zeugnisbemerkungen von S1 werden gelöscht (neue und alte reimportierte Zeugnisbemerkungen), nur die alten Zeugnisbemerkungen werden eingelesen. Im Ergebnis fehlen die neuen Zeugnisbemerkungen von L1. Sie können den Konflikt nur lösen, indem Sie entweder:
> * entweder Schülern nicht einen Klassenleiter UND einen Tutor zuweisen
> * oder falls beide Felder für Schüler vergeben sind, beim Erstellen der Dateien nicht Tutor- und Klassenleiterdateien gemeinsam erstellen, sondern erst die Dateien für die zweite Rolle nach dem Einsammeln der Daten der ersten Rolle verteilen.  



> #### success::Tipp
>
> Zum Schluss eine Vorgehenstipp für die Schulen in Rheinland-Pfalz, an denen es eine MSS gibt: In der Mainzer Studienstufe wird das Fach „Gemeinschaftskunde“ als Grundkurs von zwei Lehrkräften je zweistündig unterrichtet. Dadurch sind in beiden Lehrerdateien die Schüler beinhaltet. Es sollte zuvor vereinbart werden, wer die Noten erfassen soll. Vorschlag: Es trägt diejenige Lehrkraft die Noten ein, in deren Fach die Kursarbeit geschrieben wurde.