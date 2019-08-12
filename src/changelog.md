# Was ist neu

Dieses Kapitel gibt ihnen einen Überblick über aktuelle Änderungen in MAGELLAN 6.

Den Änderungsverlauf aus den vergangenen Jahren finden Sie hier: [2018](changelog-2018.md),[2017](changelog-2017.md), [2016](changelog-2016.md), [2015](changelog-2015.md), [2014 und früher](changelog-archive.md).

* Was wir für die nächste Ausgabe planen, sehen Sie im Kapitel ["Voraussichtliche Änderungen"](changelog-next.md).

* [Anleitung zum Einspielen eines Serviceupdate.](installation/update.md)

* [Probleme beim Einspielen des Updates?](installation/probleme-beim-update.md)

## LEGENDE

Abkürzung | Bedeutung
----------|----------
FIX       | Korrektur bestehender Funktionalität
NEW       | Neue Funktionalität
CHANGE    | Änderung des Ablaufs, Verarbeitung oder Bedienung

## Wichtiger Hinweis

> #### danger::Achtung!
>
>
> Bitte beachten Sie, dass unser Support einen Supportvertrag voraussetzt und für die jeweils aktuelle Ausgabe von MAGELLAN gilt, dass ist aktuell MAGELLAN 7.  **Die Unterstützung für MAGELLAN 6 wird Ende dieses Jahres eingestellt.**

## 6.5.37 - 673 (12.08.2019)

### MAGELLAN

* FIX: Anpassung im Skript "Schüler korrigieren.dws"

### Statistik

* NEW: Rheinland-Pfalz Statistikmodul 2019. Beachten Sie bitte die aktualisierten Schlüsselverzeichnisse. Bitte beachten Sie die aktualisierte [Statistikdokumentation](https://doc.ls.stueber.de/rheinland-pfalz/abs-bbs/) für RLP.

## 6.5.36 - 673 (19.07.2019)

### Skripte

* FIX: "Zuweisen von Kategorietafeln" korrigiert
* FIX: "Benutzerrechte zuweisen" korrigiert

## 6.5.35 - 673 (01.07.2019)

> #### warning::Wichtig!
>
> Die Datenstruktur von MAGELLAN ist erweitert worden! 
> Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von MAGELLAN erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](https://doc.magellan6.stueber.de/installation/update.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](https://doc.magellan6.stueber.de/installation/probleme-beim-update.html).
> Bitte denken Sie daran im Anschluss an die Strukturanpassung der Datenbank noch die Zugriffsrechte der Benutzer unter `MAGELLAN ADMINISTRATOR > Datenbankpflege > Datenbank überprüfen > Zugriffsrechte synchronisieren` zu aktualisieren!

### MAGELLAN

* FIX: Beim Update wird die audit.conf nicht mehr ersetzt
* FIX: Die Rechte für den Assistenten `Extras > Schüler korrigieren` wurden angepasst (Bitte Zugriffsrechte synchronisieren!)
* FIX: Ergebnisfenster des Assistenten `Extras > Schüler korrigieren` bleibt geöffnet
* FIX: Die Rechte für die Nutzung der ENBREA-Leistungen wurden analog der Kollegiumsrechte für `Schüler > Zeugnis > Fächer/Leistungen` eingefügt
* CHANGE: Beim Assistenten `Klassen > Bearbeiten > Schuljahreswechsel` werden auch die Einträge für ENBREA-Leistungen für die neuen Klassen übernommen.
* NEW: Neue Nachrichtenfunktion: Die MAGELLAN-Willkommensseite wurde neu gestaltet und enthält jetzt zu den wichtigsten Aufrufen (Dokumentation, Newsletter, Ticketsystem usw.) einen Nachrichtenbereich, über den wir Sie auf dem Laufenden halten werden. Sie erhalten diesen Überblick beim Aufruf von MAGELLAN, des MAGELLAN ADMINISTRATORs und der MAGELLAN BIBLIOTHEK.

### Skripte

* CHANGE: `Benutzerrechte zuweisen.dws` Rechte für ENBREA-Leistungen ergänzt
* CHANGE: `Synchronisiere Zugriffsrechte.dws` Rechte für ENBREA-Leistungen ergänzt

### Berichte (neu oder geändert)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE: RLP-GY-AZ (2016).rpt (hinter den Fremdsprachen wird das Sprachniveau in Klammern ausgegeben)

![](/images/liesmich/6.5.34_01.png)

* CHANGE: RLP-GY-AZ (7-10).rpt _(hinter den Fremdsprachen wird das Sprachniveau in Klammern ausgegeben)_
* CHANGE:  Skript BER-APO-2017.dws,  Prüfung auf mehr als 3 Seminarkurse
* CHANGE: DAS-Prüfungsbogen (Anlage 7 zu DIA-PO)(2018).rpt (Unterrichtssprachen)

#### Berlin

* CHANGE: BER-Schul Z 306 (11.18).rpt _(Fußnote 1) bei den Fremdsprachen gemäß Vorlage geändert, Text "Freibleibende Felder sind zu entwerten" ergänzt, Ausgabe "Punkte in einfacher Summe" für die 5 Prüfungskomponente korrigiert)_
* CHANGE: BER-GY (Abi-18a - Mitteilungen zu den schriftlichen und mündlichen Prüfungen)(03.12).rpt _(Ausgabe "Punkte in einfacher Summe" und "Note" für die 5 Prüfungskomponente korrigiert, Ausgabe der Punkte in einfacher Summe für die 5 Prüfungskomponente auf Seite 2/Rückseite korrigiert)_
* NEW: BER-Schul Z 255 (10.18).rpt _(Schul Z 255 – Zeugnis des Gymnasiums über die erweiterte Berufsbildungsreife (10.18))_

## 6.5.34 - 672 (28.05.2019)

> #### warning::Wichtig!
>
> Die Datenstruktur von MAGELLAN ist erweitert worden!   
> Bitte aktualisieren Sie als erstes Ihren Serverrechner, anschließend alle Arbeitsplatzrechner! Beim ersten Start von MAGELLAN erfolgt eine automatische Anpassung an die neue Datenstruktur durch einen Assistenten. Eine genaue Anleitung zum Serviceupdate finden Sie [**hier**](http://doc.magellan6.stueber.de/installation/serviceupdates.html). Sollten Probleme auftreten, schauen Sie bitte [**hier**](http://doc.magellan6.stueber.de/installation/troubleshootingupdate.html).

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* CHANGE: 
* FIX: Synchronisiere Mittelstufe.dws
* FIX: BER-APO-2017.dws
* FIX: NRW-APO-BK-2012.dws
* CHANGE: SHL-APO-2018.dws (GER-Niveau wird nun NEU vom Skript berechnet, lesen Sie dazu folgenden [Abschnitt](https://doc.la.stueber.de/Skripte/SAR-APO-2018.html))

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* CHANGE: DAS-GY-ABI \(DIA\)\(2019\).rpt (_Layoutänderungen, KMK Logo auf Deckblatt eingebaut_)
* CHANGE: BAW-BG-ABI \(DIN A4 doppelseitig 2018\).rpt
* CHANGE: SAC-BG-ABI \(E.01.06\).rpt  \(_Layoutänderungen\)_
* NEW: NRW-BK-ABI \(Anlage D41\)\(2018\)\(GeR\).rpt \(_Anlage D 41, Zeugnis der Allgemeinen Hochschulreife - Niveau gemäß GER eingebaut, zum Erfassen der Niveaustufen lesen Sie bitte folgenden Artikel in der MAGELLAN 6 Knowledge Base: _[https://doc.magellan6-kb.stueber.de/sprachreferenzen.html](https://doc.magellan6-kb.stueber.de/sprachreferenzen.html) \)
* FIX: NIE-GY (Studienbuch - Einführungsphase) G9.rpt _(vor einstellige Punktzahlen wird nun eine Null vorangestellt)_
* FIX: SHL-GY-ABI (2018).rpt _(vor einstellige Punktzahlen wird nun eine Null vorangestellt)__


#### Berlin

* CHANGE: BER-Schul Z 306 \(11.18\).rpt \(_Positionierung der Fächer angepasst, Für die Sortierung der Fächer auf den Zeugnissen muss im Menü "Schüler" bei jedem Schüler auf der Registerkarte "Zeugnis\|Fächer" bzw. im Menü "Abitur"  bei jedem Schüler auf der Registerkarte "Qualifikation" pro Fach eine Position in der Spalte "Position" angegeben werden. Die Ausgabe der Fächer auf dem Zeugnis entspricht dieser Sortierung. _\)
* CHANGE: BER-GY \(abi\_4\_berechnungsbogen\)\(10.16\).rpt \(_Layoutänderungen_\)
* NEW: BER-Schul 5 256 (10.18).rpt (_Schul Z 256 – Zeugnis des Gymnasiums über den mittleren Schulabschluss (10.18)_)


> #### danger::Achtung!
>
> * SERIENDRUCK: Wir übergeben für den Seriendruck fest an Word die Zeichencodierung als UTF8. 
> Wenn Sie in der Registry einen Schlüssel gesetzt hatten, der Umlauteproblem von Word lösen sollte, muss dieser Schlüssel (der den Zeichensatz 1252 vorgibt) wieder entfernt werden! 
> Artikel: ["Word stellt Umlaute nicht korrekt dar"](https://doc.magellan6-kb.stueber.de/seriendruck/umlaute.html)
>
> * RUNTIME-ERROR: Einige Benutzer, die von älteren Versionen umsteigen, können MAGELLAN im Anschluss nicht starten. Meist ist die Ursache, dass eine der Dateien, die beim Programmstart geladen werden, beschädigt ist. 
>   Sie finden hier eine [Anleitung](https://doc.magellan6.stueber.de/installation/probleme-beim-update.html#meldung-runtime-error-) um dieses Problem zu beheben.

---
## 6.5.33 - 671 (16.04.2019)


### MAGELLAN ADMINISTRATOR

* CHANGE: `Datenbank überprüfen > Anrede setzen` \(Aktion wird ausgeführt, wenn die Anrede leer, F oder H ist\)


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* CHANGE: NRW-APO-2012.dws \(Problem in der Vorschlagsautomatik korrigiert\)
* FIX: RLP-APO-2014.dws: Vorschlag für Musik als freiwilliges Fach korrigiert.
* CHANGE: NRW-APO-BK-2012.dws: Mit der Ausgabe dieses Skriptes werden beim Initialisieren nur noch Kurse berücksichtigt, die mit einer der nachstehenden Unterrichtsart markiert sind. Durch diese Änderung werden gezielt Kurse von der Berücksichtigung im Abitur ausgeschlossen. In den Fachdaten erfasste Zeilen, die beispielsweise das Arbeits- und Sozialverhalten beinhalten, bleiben so außen vor.

| Kürzel | Schlüssel | Bedeutung |
| --- | --- | --- |
| LK | LK | Leistungskurs  \(LK wird für das Abitur und die Fachhochschulreife, nicht durch Unterrichtsart sondern durch Fachstatus "1PF/2PF" identifiziert.\) |
| GK | GK | Grundkurs \(GK wird für das Abitur und die Fachhochschulreife, nicht durch Unterrichtsart sondern durch nicht erfolgten Eintrag der Fachstatus "1PF/2PF" identifiziert.\) |
| DB | DB | Die Unterrichtsart kann verwendet werden, damit die Kursergebnisse beim Initialisieren mit einbezogen werden. |
| BU | BU | Die Unterrichtsart kann verwendet werden, damit die Kursergebnisse beim Initialisieren mit einbezogen werden. |
| BÜ | BÜ | Die Unterrichtsart kann verwendet werden, damit die Kursergebnisse beim Initialisieren mit einbezogen werden. |

#### BER-APO-2017.dws

* FIX: wenn Biologie als einziges naturwissenschaftiches Fach durchgängig belegt wurde, wird nun richtig geprüft, dass auch in Physik oder Chemie zwei Kurse belegt und eingebracht werden müssen \(VO-GO §25\)
* FIX: wenn Sport als 4. oder 5. PF gewählt ist, wird nun richtig der letzte Kurs Sporttheorie eingebracht sowie 3 Praxiskurse Sport \(ein weiterer Sportkurs \(Praxis oder Theorie\) kann zusätzlich eingebracht werden
* FIX: Vorschlag berücksichtigt nun auch Folgendes: für das 5. PF gilt \(außer Sport\) - nur der letzte Kurs muss eingebracht werden, wenn die Belegverpflichtunganderweitig im gleichen Aufgabenfeld erfüllt wurde

#### DE-DIAP-2015.dws

* CHANGE: Vorschlagsautomatik optimiert
* NEW: Ermittlung einer Schnittverbesserung durch mögliche Einbringung einer mdl. Note 
![``Abitur > Prüfung``](images/liesmich/6.5.33_01.png)
* NEW: Ermittlung der Abiturzulassung am Ende der Q3 wenn unter dem Menü ``Abitur > Qualifikation`` in den Feldern ``Q4`` keine Punktwerte eingetragen sind
![``Abitur > Qualifikation``](images/liesmich/6.5.33_02.png)

#### DE-MSA-2019.dws

* NEW: Neues Berechnungsskript für die Durchschnittsberechnung MSA für Auslandsschulen gemäß Ordnung für den Abschluss der Sekundarstufe I an Deutschen Schulen im Ausland vom 16.03.2017 im Menü `Schüler > Zeugnis > Leistungen`. 
Bitte bitte lesen Sie dazu den Abschnitt der Landesanpassung [DE-MSA-2019](https://doc.la.stueber.de/durchschnitt_abschluss/de-msa-2019dws.html)

![`Schüler > Zeugnis > Leistungen`](images/liesmich/6.5.33_03.png)

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* FIX: RLP-GY-AZ (2016).rpt (Bericht optimiert, damit allen Angaben auf einer Seite ausgegeben werden)
* FIX: BER \(Kurswahl\).rpt \(Anzahl der auszugegebenen Fächer unter Aufgabenfeld 2 um zwei Fächer erweitert\)
* NEW: Klassenliste mit Schülersummendaten Ausländer.rpt
* FIX: BER-Schul Z 302 (10.18).rpt (Ausgabe der Fächer im Bereich "weitere Fächer" korrigiert)

#### DAS-Zeugnisse

* CHANGE: DAS-Versetzungszeugnis-GY-MSA (ZKA)(Anlage 11)(§23).rpt |personalisierte Zeugnisbemerkungen |
* FIX: DAS-HS-MSA-AS (Anlage 8 und 9)(§23).rpt |Ausgabe der mdl. Noten, es werden alle eingetragenen Fächer mit einer mdl. Note ausgegeben, Ausgabe Notendurchschnitt korrigiert|
* FIX: DAS-ZZ (Q-Phase)(Anlage 1)(RiLi 1.6).rpt | personalisierte Zeugnisbemerkungen|
* NEW: DAS-GY-ABI (DIA)(2019).rpt | +++Abiturzeugnis+++ bitte verwenden Sie dieses Zeugnis für den Druck des Abiturzeugnisses 2019 gemäß Anlage 7 anstatt des Berichtes _DAS-GY-ABI (Anlage 7).rpt_|
* FIX:  DAS-Zeugnis Gymnasium - Mittlerer Schulabschluss (Anlage 10)(§23).rpt | Ausgabe der mdl. Noten, es werden alle eingetragenen Fächer mit einer mdl. Note ausgegeben, Ausgabe Notendurchschnitt korrigiert|


> #### primary::Hinweis
>
> Bitte tragen Sie im Verzeichnis ``Fächer`` in der Spalte "Merkmal" für die Fächer Deutsch, Englisch, Mathematik und die Landessprache die nachstehend Kürzel ein. Aus diesen Kürzeln ergeben sich die Fächer auf erhöhtem Anforderungsniveau. Zudem wird in einigen Berichten durch dieses Fachmerkmal geklammert ein (E) hinter der Fachbezeichnung ausgegeben.


| Fach (Bezeichnung/Kürzel) | Merkmal |
|---------------------------|---------|
| -                         | -       |
| Deutsch                   | D       |
| Mathematik                | M       |
| Englisch                  | E       |
| Landessprache             | LS      |



## 6.5.32 - 671 (01.02.2019)


### MAGELLAN

* FIX: Problem beim Versetzen von Schülern in einen anderen Mandanten behoben, für jeden Schüler wird seine Herkunftsschule in den anderen Mandanten übernommen.
* FIX: Problem beim Kopieren von Schülern in parallelen Mandanten mit Merkmalen (umbenannte Merkmale mit Leerzeichen in der Umbenennung)behoben
* FIX: Neu eingestellte aktuelle Ausbildung wird gespeichert vor Kartenwechsel (Problem trat bei Wechsel auf Merkmale auf)
* NEW: Beim Import von Schülern/Bewerbern aus SchülerOnline (NRW) wird aus dem Geschlecht (m/w) automatisch die Anrede(Herr/Frau) vorbefüllt.


### MAGELLAN ADMINISTRATOR

* FIX: Text unter `Datenpflege > Datenbank überprüfen > Abiturdetails korrigieren` korrigiert
* NEW: Unter `Datenpflege > Datenbank überprüfen > Anrede setzen` gibt es die Möglichkeit für Schüler/Bewerber/Lehrer/Personen, die bislang keine Anrede hatten, die Anrede (Herr/Frau) anhand der Auswahl des Geschlechts (m/w) zuzuweisen. [Dokumentation hier](https://doc.magellan6.stueber.de/admin/db-connection.html#datenbank-%C3%BCberpr%C3%BCfen)
* NEW: Unter `Datenpflege > Datenbank überprüfen > Schüler-Passfoto löschen` können Sie alle Passbilder der inaktiven Schüler aus der Datenbank (aller Schüler, aller Zeiträume, aller Mandanten) entfernen. Die Größe der Datenbank reduziert sich nach dem Sichern und Wiederherstellen Ihrer Datenbank. [Dokumentation hier](https://doc.magellan6.stueber.de/admin/db-connection.html#datenbank-%C3%BCberpr%C3%BCfen)

![Neue Funktionen `Anrede setzen` und `Schüler-Passfoto löschen`](/images/liesmich/6.5.32.01.png)


### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* CHANGE: NRW-APO-BK-2012.dws: Beim Initialisieren und beim Vorschlag werden nur Zeilen berücksichtigt, die die Unterrichtsarten `GK`, `LK` oder `DB` haben. Sollten Sie weitere Fächer in der Abiturqualifikationskarte haben (beispielsweise Ergebnisse des Arbeits- und Sozialverhaltens), werden diese nicht für die Abiturqualifikation berücksichtigt.
* CHANGE: MVP-APO-2017.dws: kleine Korrekturen

### Berichte \(neu oder geändert\)

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

* NEW: NIE-GY (Studienbuch - Einführungsphase) G9.rpt _(zweite Seite des Studienbuches, Einführungsphase)_
* NEW: BER-Schul Z 250 (10.18).rpt _(Schul Z 250 – Zeugnis des Gymnasiums, Jahrgangsstufen 7 bis 10, optional Jahrgangsstufen 5 und 6 – (10.18))_
* NEW: SAC-BS-AS (Vorbereitungsklasse) (A.01.06)(2019).rpt _(Zeugnis der Berufsschule Vorbereitungsklasse)_
* NEW: SAC-BS-HJI (A.01.02)(2019).rpt _(Halbjahresinformation der Berufsschule Vorbereitungsklasse))_

#### Sachsen

In folgenden Berichten wurde das Wort „SchulG“ durch das Wort „SächsSchulG“ (gemäß VwV Zeugnisse berufsbildende Schulen vom 05.11.2018) ersetzt:
* CHANGE: SAC-BS-BVB Maßnahme (A.01.05).rpt 
* CHANGE: SAC-BVJ-AS mit HS (A.01.08).rpt
* CHANGE: SAC-BVJ-AS ohne HS (A.01.09).rpt
* CHANGE: SAC-BVJ-AS ohne HS (A.01.10).rpt
* CHANGE: SAC-BGJ-AS ohne HS (A.01.11).rpt
In folgenden Berichten wurde die Angabe „Personensorgeberechtigte/r“ durch das Wort „Eltern“ ersetzt.
* CHANGE: SAC-BF-HJI (B.01.01).rpt
* CHANGE:SAC-BS-JZ (A.02.01).rpt
* CHANGE: SAC-FOS-HJZ (D.01.01).rpt
* CHANGE: SAC-FOS-JZ (D.01.02).rpt
* CHANGE: SAC-BG-HJZ (E.01.01).rpt
* CHANGE: SAC-BG-JZ (E.01.02).rpt
* CHANGE: SAC-BG-HJZ (E.01.03).rpt
* CHANGE: SAC-BG-HJZ (E.01.04).rpt

#### Berlin
* NEW: BER-Schul Z 250 (10.18).rpt

## 6.5.31 - 671 (18.01.2019)

### MAGELLAN

* CHANGE: Änderung im Seriendruck, die Zeichencodierung wird fest als UTF8 von MAGELLAN übergeben, WORD hat in einigen Ausgaben ein Problem ab einer bestimmten Menge von Datensätzen die Zeichencodierung korrekt zu erkennen.

### Importe

* FIX: SAC-BS_Bildungsgaenge.keys: In der Spalte `Bezeichnungen` wurden die vorangestellten Schlüsselnummern entfernt.

### Skripte

Eine Anleitung für alle unsere Berechnungsskripte finden Sie in der Dokumentation [MAGELLAN Landesanpassungen](https://doc.la.stueber.de).  
Hinweis für angepasste Skriptdateien: Mit der MAGELLAN-Version 6.5 wurde der Skriptingmechanismus auf eine neue Version aktualisiert. Welche Änderungen für von Schulen angepasste Skripte notwendig sind, beschreiben wir hier: [https://doc.magellan-scripting.stueber.de/anderungen.html](https://doc.magellan-scripting.stueber.de/anderungen.html)

* FIX: DE-DIAP-2015.dws: Fehler bei Summierung im Bereich 4 behoben.
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

#### Rheinland-Pfalz

In folgenden Zeugnissen wurde die Ausgabe des erreichten Niveaus auf der Grundlage des "Gemeinsamen Europäischen Referenzrahmens für Sprachen" (GER) eingebaut bzw. das Deckblatt aktualisiert. Bitte tragen Sie unter `Daten 3 > Fremdsprachenfolge` im Feld `Referenz` das Referenzniveau der Fremdsprache ein. Grundlage bildet das `Verzeichnis > weitere Schlüsselverzeichnisse > Sprachreferenzen`. Vom Bericht wird das Kürzel abgefragt. Eine Klammer wird nur bei vorhandenem GER Niveau ausgegeben. D.h. wenn in Daten3 Referenzniveau eingetragen ist, wird die Fremdsprache ohne Klammer ausgegeben. Z.B. "Latein", "Englisch", "Englisch (B1)", ...



| Kürzel | Schlüssel | Bezeichnung      |
|--------|-----------|------------------|
| B1     | B1        | B1               |
| B1/B2  | B1/B2     | B1, in Teilen B2 |
| B2     | B2        | B2               |
| B2/C1  | B2/C1     | B2, in Teilen C1 |
| C1     | C1        | C1               |





![](images/liesmich/MAG.6.5.30_001.png)

* CHANGE: RLP-BG-ABI (2018)(inkl.GER).rpt
* CHANGE: RLP-GY-ABI (2018-G8-G9)(inkl.GER).rpt
* CHANGE: RLP-GY-ABI (2018-G8-G9)(A4 Seite 1).rpt
* CHANGE: RLP-GY-ABI (2018-G8-G9)(A4 Seite 2)(inkl.GER).rpt
* CHANGE: RLP-GY-ABI (2018-G8-G9)(A4 Seite 1)(ohne Wappen).rpt
* CHANGE: RLP-BG-ABI (2018)(inkl.GER)A4.rpt
* CHANGE: RLP-BG-ABI (inkl.GER).rpt
* CHANGE: RLP-BG-ABI (inkl.GER)A4.rpt

#### Berlin

_Die Zeugnisse sind für G8/G9 Schulen ausgelegt._


* NEW: BER-Schul Z 300 (10.18).rpt
* NEW: BER-Schul Z 301 (11.18).rpt
* NEW: BER-Schul Z 302 (10.18).rpt
* NEW: BER-Schul Z 303 (10.18).rpt
* NEW: BER-Schul Z 306 (11.18).rpt
* NEW: BER-Schul Z 351 (10.18)_Kolleg.rpt
* NEW: BER-Schul Z 351 (10.18)_Oberstufe.rpt 


