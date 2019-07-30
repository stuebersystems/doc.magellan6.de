# Formulare, Listen und Zeugnisse

Dieses Kapitel beschreibt das Drucken von Formularen, Listen und Zeugnissen mit MAGELLAN. Grundlage für die Druckmöglichkeiten bilden Berichte, die im Berichtsgenerator Crystal Reports erstellt worden sind. Zum Ausdruck können Sie entweder auf von uns erstellte Berichte zurückgreifen oder Sie erstellen Berichte nach Ihren eigenen Bedürfnissen. Die alternative Ausdruckmöglichkeit über Microsoft Access wird ebenfalls erläutert. 

callDer Seriendruck über Word und die Exportmöglichkeiten nach Excel bzw. HTML werden im Kapitel [„Seriendruck, Serienemail, Dokumentenverwaltung und Exportieren“](https://doc.magellan6.stueber.de/howto/seriendruck.html) vorgestellt.

## Magellan Crystal-Reports

### Allgemeines

Berichte definieren in MAGELLAN das Layout und den Inhalt von Ausdrucken in Form von Zeugnissen, Übersichten, Formularen, Listen usw. Diese Berichte sind in MAGELLAN standardmäßig in dem Berichtsgenerator Crystal Reports erstellt worden. 

Mit MAGELLAN wird eine große Anzahl von Crystal Reports-Berichten kostenlos mitgeliefert. Eine Übersicht über die vorhandenen Berichte finden Sie über den MAGELLAN-Berichts-Explorer. Alle darin erwähnten Crystal Reports-Berichte für Listen und Zeugnisse können mit dem kostenlos mitgelieferten Runtime-Modul von MAGELLAN ausgedruckt werden. Wenn Sie lediglich die mitgelieferten Zeugnisformulare verwenden, ohne Änderungen am Layout vorzunehmen, benötigen Sie keinen Druckreportgenerator, da bereits eine Runtime-Version des in MAGELLAN verwendeten Crystal Reports-Berichtsgenerators mitinstalliert wird. 

Wenn Sie Berichte selbst verändern oder erstellen möchten, benötigen Sie Crystal Reports. Um bestehende Berichte zu verändern oder eigene Berichte mit Crystal Reports zu erstellen, müssen Sie eine Lizenz von Crystal Reports erwerben. STÜBER SYSTEMS liefert in Kombination mit einer MAGELLAN-Lizenz exklusiv eine spezielle Schulversion von Crystal Reports Professional. Diese Sonderversion kann dann auf fünf Rechnern installiert werden, auf denen auch MAGELLAN installiert ist.

### Unterstützte Crystal Reports Versionen

Magellan 6 verfügt über eine Drucktechnologie, die Crystal Reports 9, 10 und XI(...) unterstützt. Die Berichte werden in Crystal Reports XI zur Verfügung gestellt, die abwärtskompatibel bis zur Version 9 von Crystal Reports sind. 

### Was ist mit meinen selbst erstellten Berichten aus MAGELLAN 4?

Wenn Sie selbst erstellte Crystal Reports Berichte aus der Version 4 von MAGELLAN auch unter MAGELLAN 6 nutzen wollen, müssen Sie diese in Crystal Reports ab der Version 9 überprüfen. Gehen Sie dazu wie folgt vor:

1. Öffnen Sie dazu Ihren Bericht in Crystal Reports 9 oder höher.

2. Klicken Sie auf `Datenbank > Datenbank überprüfen`.

3. Führen Sie die Aktualisierung aus.

Zusätzlich muss im Bericht (sowohl im Hauptbericht als auch in allen Unterberichten) jeweils im Dialogfenster Berichtsoptionen das Markierungsfeld `Beim ersten Aktualisieren überprüfen` NICHT angekreuzt sein. Gegebenenfalls müssen Sie Ihren Bericht aufgrund der Beschreibung der MAGELLAN-Datenstruktur im Dokument MAGELLAN-Datenstruktur.pdf anpassen. Die betrifft nur Berichte, die das Feld „Tutor“ bzw. die Tabelle „Adressen“ verwenden.

## Berichte organisieren

Alle Berichte in MAGELLAN sind den entsprechenden Bereichen für Schüler, Bewerber, Klassen, Lehrer, Sorgeberechtigte, Betriebe, Personen, Adressen, Schulen, Mandanten zugeordnet. Zusätzlich gibt es noch die gesonderten Bereiche Zeugnisse und Kurslisten für Schüler. Alle Berichte können auf Basis der Auswahllisten der jeweiligen Bereiche gedruckt werden. Wie Sie die Berichte ausdrucken, erfahren Sie im nachfolgenden Abschnitt „Berichte drucken“. Die Verwaltung der Berichte öffnen Sie über `Extras > Berichte organisieren`.
 

![Das Fenster Berichte organisieren besteht aus einer Schnellstartleiste auf der linken Seite, die den Bereichen in MAGELLAN entsprechen.](/images/formulare/formulare1.png)

Klicken Sie beispielsweise auf den Ordner `Klassen`, so erscheinen auf der rechten Seite alle Berichte, die für Klassen existieren. Über die Funktion `Kopieren > Einfügen` können Sie die einzelnen Berichte in den gewünschten Ordner verschieben. Alle Berichte, die sich in dem Ordner „Kurslisten“ befinden, werden ebenfalls dem Bereich der Klassen zugeordnet. Berichte im Ordner `Zeugnisse` werden dem Bereich der Schüler zugeordnet. Über die Schaltfläche `Dokumente importieren` können Sie Ihre Berichtsverwaltung um eventuell selbst erstellte Berichte erweitern.

## Berichte drucken

### Formulare und Listen

Sie drucken Listen bzw. Formulare, indem Sie in die entsprechende Auswahlliste wechseln und dort die gewünschten Einträge markieren, für die ein Bericht gedruckt werden soll. Wollen Sie z.B. einen Bericht für Schüler ausdrucken, dann müssen Sie einen oder mehrere Schüler in der Auswahlliste der Schüler markieren und dann mit der rechten Maustaste den Befehl `Bericht drucken` aufrufen. Es öffnet sich das Fenster Bericht drucken, in dem Sie den gewünschten Bericht auswählen können.
 
![Klicken Sie auf „Vorschau“, um den Bericht nur in der Vorschau zu öffnen.](/images/formulare/formulare2.png)

Wenn Sie auf `Drucken und Export nach PDF` klicken, wird zunächst der Berichte für alle markierten Schüler pro Schüler ins PDF-Format exportiert und dann erfolgt der eigentliche Druck. Diese Schaltfläche ist anstatt der Schaltfläche Drucken nur dann sichtbar, wenn Sie in den Optionen den Export ins PDF-Format eingestellt haben (siehe „Berichte und Zeugnisse exportieren“). Andernfalls lautet die Schaltfläche nur `Drucken`. Berichte im Bereich „Mandanten“ beziehen sich auf alle Daten des aktuellen Zeitraums des markierten Mandanten. Hier finden Sie z.B. Übersichtslisten über alle Schüler des Mandanten, Bewerberranglisten über alle Bewerber des Mandanten usw.

> #### primary::Hinweis
>
> Sie können alle Berichte optional nach Excel, Word oder ins PDF-Format exportieren. Rufen Sie dazu die Seitenvorschau des Berichtes auf und klicken auf das Symbol ![ ](/images/formulare/formulare3.png). Wählen Sie anschließend das gewünschte Export-Format (z.B. Excel-Format) und legen Sie einen Speicherort fest. Sie können die Berichte dann z.B. im Excel-Format weiterverarbeiten.

### Kurslisten

Um Kurslisten zu drucken, müssen Sie die entsprechende(n) Klasse(n) in der Auswahlliste Klassen markieren und dann mit der rechten Maustaste den Befehl `Kurslisten drucken` wählen. Es öffnet sich das Fenster Kursliste drucken.
 
![Stellen Sie hier die gewünschten Filter ein. Klicken Sie dann auf OK und wählen Sie den gewünschten Bericht zum Druck aus.](/images/formulare/formulare4.png)

### Prüfungslisten

Prüfungslisten basieren auf den Daten in der Ansicht „Abitur“. Um Prüfungslistenlisten zu drucken, müssen Sie die entsprechende(n) Schüler(n) in der Auswahlliste Abitur markieren und dann mit der rechten Maustaste den Befehl `Prüfungslistenlisten drucken` wählen. Es öffnet sich das Fenster `Prüfungsliste drucken`.
 
![Stellen Sie hier die gewünschten Filter für die Prüfungsliste ein. Klicken Sie dann auf OK und wählen Sie den gewünschten Bericht zum Druck aus.](/images/formulare/formulare5.png)

### Zeugnisse

So drucken Sie Zeugnisse:

1. Um Zeugnisse zu drucken, müssen Sie den bzw. die entsprechenden Schüler in der Auswahlliste Schüler markieren und dann mit der rechten Maustaste den Befehl `Zeugnisse drucken` wählen.
 
![Dialog „Zeugnisse drucken“](/images/formulare/formulare6.png)

2. Wählen Sie den gewünschten Report aus und klicken Sie auf `Vorschau`.
 
![Zeugnis in der Seitenvorschau](/images/formulare/formulare7.png)

Klicken Sie dann auf `Drucken` und der gewünschte Report wird gedruckt. Wenn Sie auf `Drucken und Export nach PDF` klicken, wird zunächst das Zeugnis für alle markierten Schüler pro Schüler ins PDF-Format exportiert und dann erfolgt der eigentliche Druck. Diese Schaltfläche ist anstatt der Schaltfläche `Drucken `nur dann sichtbar, wenn Sie in den Optionen den Export ins PDF-Format eingestellt haben (siehe „Einstellung für Crystal Reports Berichte“). Andernfalls lautet die Schaltfläche nur `Drucken`.

> #### primary::Hinweis
>
>  Sie können alle Zeugnisse optional nach Excel, Word oder ins PDF-Format exportieren. Rufen Sie dazu die Seitenvorschau des Berichtes auf und klicken auf das Symbol  . Wählen Sie anschließend das gewünschte Export-Format (z.B. Acrobat-Format) und legen Sie einen Speicherort fest. Sie können die Zeugnisse dann z.B. im Word-Format weiterverarbeiten.

So drucken Sie beim Schüler hinterlegte Zeugnisse: 

Um die beim Schüler hinterlegten Zeugnisse automatisiert zu drucken, müssen Sie den bzw. die entsprechenden Schüler in der Auswahlliste Schüler markieren und dann mit der rechten Maustaste den Befehl `Zeugnisformulare drucken` wählen. Weitere Informationen finden Sie dazu im Abschnitt ["Zeugnisformulare"](https://doc.magellan6.stueber.de/howto/zeugnisdaten.html#zeugnisformulare).
 
![Es kann ggf. nach einem Typ gefiltert werden, wenn Sie diesen im Schlüsselverzeichnis „Zeugnisformulare“ bei den Formularen hinterlegt haben.](/images/formulare/formulare8.png)

## Eigene Berichte erstellen

Wenn Sie neue Berichte erstellen bzw. vorhandene verändern möchten,  benötigen Sie einen Berichtsgenerator, d.h. ein Programm, mit dem Sie Berichte erstellen und verändern können. MAGELLAN verwendet ausschließlich den Berichtsgenerator Crystal Reports. In MAGELLAN werden daher nur Crystal Reports Berichte mitgeliefert. Sie können eine spezielle Schulversion von Crystal Reports von STÜBER SYSTEMS beziehen. 

Sie können Berichte alternativ auch in Access erstellen. Wie Sie Access an die MAGELLAN-Datenbank anbinden, erfahren Sie im Abschnitt [„Access-Anbindung in Magellan“](https://doc.magellan6.stueber.de/admin/import-export.html#access-anbindung-in-magellan). Das Drucken von Access-Berichten wird im nachfolgenden Abschnitt beschrieben. Bitte beachten Sie, dass gerade schwierige Berichte wie Zeugnisberichte in Crystal Reports wesentlich effizienter erstellt werden können. Falls Sie selbst in Crystal Reports Berichte erstellen möchten, finden Sie die dazu notwendigen Informationen in folgenden Dokumenten:

* „Crystal Reports Benutzerhandbuch“
* „Magellan 6 Datenstruktur“ (bitte unter support@stueber.de anfordern) 


Zudem gibt es eine große Auswahl von Sekundärliteratur zu Crystal Reports im Buchhandel. STÜBER SYSTEMS bietet zudem Schulungen zur Berichtserstellung in MAGELLAN an, die Ihnen eine Einführung geben bzw. Ihr Wissen vertiefen. 

Außerdem bietet STÜBER SYSTEMS speziellen Support zur Berichtserstellung mit MAGELLAN und Crystal Reports. Um Berichte selbst erstellen zu können, benötigen Sie sehr gutes Wissen in der Berichtserstellung in Crystal Reports und der MAGELLAN Datenstruktur. 
In der Regel ist es bei der Erstellung eigener Berichte am einfachsten, einen der mitgelieferten Berichte zu nehmen und diesen entsprechend abzuändern. Das Erlernen dieses Wissens ist nicht sehr schwer, aber auch nicht ganz einfach. Wenn Sie sich die Zeit und den Einarbeitungsaufwand sparen möchten, können Sie STÜBER SYSTEMS beauftragen, Ihre Zeugnisse und andere Berichte zu erstellen. Sie erhalten dann von STÜBER SYSTEMS die entsprechenden Crystal Reports Berichtsdateien, die Sie lediglich in das entsprechende Berichtsverzeichnis kopieren müssen. Schicken Sie dazu Ihre Papiervorlagen an STÜBER SYSTEMS. Sie erhalten dann ein Angebot über die Kosten für die Erstellung der Berichte.

## Access-Anbindung

Neben der standardmäßigen Ausdruckmöglichkeit von Crystal Reports Berichten können Sie auch über Access auf die Magellan-Daten zugreifen und somit Berichte unter Access erstellen. Wie Sie eine solche Anbindung von Access an MAGELLAN realisieren können, erfahren Sie im Abschnitt [„Access-Anbindung in Magellan“](https://doc.magellan6.stueber.de/admin/import-export.html#access-anbindung-in-magellan). Um die in Access erstellten Berichte nutzen zu können, müssen Sie:

* die Verknüpfung zur Access-Datenbank in den Optionen definieren und
* eine andere Vorgehensweise beim Druck der Berichte wählen.

So definieren Sie die Access-Verknüpfung zu einer erzeugten Access-Datenbank:

1. Klicken Sie auf `Extras` und dann auf `Optionen`.

2. Wählen Sie die Registerkarte `Access-Anbindung`. Tragen Sie hier den Pfad auf die neu erzeugte Access-Datenbank ein.

![Geben Sie hier die Verknüpfung zu der zuvor erstellten  Access-Datenbank an.](/images/formulare/formulare8.png)

Das Drucken von Access-Berichten unterscheidet sich geringfügig vom Ausdruck von Crystal Reports Berichten. Um einen Access-Bericht zu drucken, gehen Sie zunächst wie beim Ausdruck von Crystal Reports gemäß dem Magellan-Benutzerhandbuch vor. Dazu müssen Sie zunächst im jeweiligen Bereich (z.B. Schüler) all diejenigen Einträge in der Auswahlliste markieren, die Sie für den Ausdruck berücksichtigen wollen. Bei der Auswahl des zu druckenden Berichts unterscheidet sich jedoch die Vorgehensweise für einen Access-Bericht:

1. Klicken Sie nach dem Markieren auf `Bearbeiten` und dann `Access starten`.

2. Bestätigen Sie die Sicherheitsabfrage mit `Ja`.

Wenn Sie bei der Verknüpfung der MAGELLAN-Tabellen nicht festgelegt haben, dass das Kennwort mit gespeichert werden soll (siehe Abschnitt [„Access-Anbindung in Magellan“](https://doc.magellan6.stueber.de/admin/import-export.html#access-anbindung-in-magellan)), müssen Sie zunächst noch das Kennwort der ODBC-Verbindung eintragen. Andernfalls wird direkt Access gestartet und Sie können einen zuvor definierten Bericht auswählen und in Access ausdrucken.
