# Datenpflege in MAGELLAN 7

Den Großteil der Datenpflege nehmen Sie bitte in MAGELLAN 6 vor, einige Dinge sind aber in MAGELLAN 6 nicht eintragbar, sondern erst durch die erweiterte Datenstruktur in MAGELLAN 7 erfassbar.

## Ausbildung in MAGELLAN 6 und MAGELLAN 7

SaxSVS erfordert im Bereich der Ausbildung folgende Werte:

* al_kennziffer -> Bildungsgang
* al_schulart   -> Schulform
* al_zeitform   -> Organisation

Da diese in unterschiedlichen Kombinationen auftreten können, müssen die Daten bei der Schüler-Ausbildung pro Schüler angegeben werden.
Die Felder Schulform und Organisation gibt es erst ab MAGELLAN 7 in der Schüler-Ausbildung. Sie haben die Möglichkeit die Felder direkt in der Schüler-Ausbildung
einzutragen, oder die Sammelzuweisung unter `Schüler > Schüler > Sammelzuweisung` zu nutzen. 

### Sammelzuweisung für Bildungsgang, Schulform und Organisation

So geht's:
1. Die Sammelzuweisung rufen Sie unter `Menüpunkt Schüler > Registerkarte Schüler > Sammelzuweisung` auf. 
2. Markieren Sie die Gruppe von Schülern, für die die gleichen Eigenschaften vergeben werden sollen.
3. Klicken Sie `Weiter` bis zur dritten Karte, hier können Ausbildungsinformationen neu oder ergänzend (Neue Ausbildung anlegen / ggfs. aktuelle Ausbildung bearbeiten) für eine bestehende Ausbildung zugewiesen werden. 

![MAGELLAN 7 > Menü Schüler > Tab Schüler> Sammelzuweisung](/images/sachsen/sammelzuweisung01.png)



## Förderbedarf in MAGELLAN 6 und MAGELLAN 7

In MAGELLAN 6 kann für die Felder `Förderbedarf`, `Schwerpunkt1`,`Schwerpunkt2` und `Behinderung` jeweils nur ein Wert pro Schüler erfasst werden. Diese Einzelwerte werden bei der Übernahme der Daten aus Ihrer MAGELLAN 6-Datenbank in eine MAGELLAN 7-Datenbank als eine Zeile (mit den einzelnen Angaben) einer Liste dargestellt. Sie haben damit die Möglichkeit ab MAGELLAN 7 mehrere Bedarfe (mehrere Zeilen in einer Liste) im Programm zu erfassen.

> #### warning::Wichtig!
>
> Bitte prüfen Sie, ob in Ihrem Verzeichnis `Extras > Schlüsselverzeichnisse > Förderbedarf` die nachfolgenden abgebildeten Schlüsselzeilen vorhanden sind. Wenn nicht, dann können Sie die Zeilen von Hand eingeben oder im MAGELLAN ADMINISTRATOR unter `Datenaustausch > Kataloge (Schlüsselverzeichnisse)importieren > Bundesland Sachsen und Schlüssel für berufsbildende Schulen` das Verzeichnis `SopaedFoerderungen` einlesen.

![MAGELLAN 7 > Extras > Schlüsselverzeichnisse > Förderbedarf](/images/sachsen/schluessel01.png)


Nachstehend sehen Sie auf der linken Seite die alte Ansicht aus MAGELLAN 6 unter Daten 4, hier gibt es nur die Möglichkeit jeweils einen Wert zu erfassen. Auf der rechten Seite die neue Möglichkeit mehrere Einträge in einer Liste anzulegen.

![Linke Seite MAGELLAN 6 und rechte Seite MAGELLAN 7](/images/sachsen/foerderungen.png)


