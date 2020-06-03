# Voraussichtliche Änderungen

Sie erhalten hier einen Überblick über die voraussichtlichen Änderungen und Korrekturen für das nächste Serviceupdate. Die nachfolgend gelisteten Änderungen wurden noch nicht veröffentlicht.

## Wichtiger Hinweis

!!! danger::Achtung!

    Bitte beachten Sie, dass unser Support für die jeweils aktuelle Ausgabe von MAGELLAN gilt, dass ist aktuell MAGELLAN 7.  **Die Unterstützung für MAGELLAN 6 wird Ende dieses Jahres eingestellt.** Eine Anleitung zum Umstieg von 6 auf 7 finden Sie [hier](https://doc.magellan7.stueber.de/schulverwaltung/update/umstieg-von-6-auf-7/).

## LEGENDE

| Abkürzung | Bedeutung |
| --- | --- |
| FIX | Korrektur bestehender Funktionalität |
| NEW | Neue Funktionalität |
| CHANGE | Änderung des Ablaufs, der Verarbeitung oder Bedienung |

---

## 6.5.42 - 673

### MAGELLAN

* FIX:
* NEW:
* CHANGE:

### Berichte

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

#### Berlin (Berufsbildende Schulen)

Die aktuellesten Zeugnisse und eine Anleitung zu den Eingaben in MAGELLAN für jedes Zeugnis finden Sie  [hier](https://my.hidrive.com/share/qptlwhk642). Sollten sich nach Einspielen des Updates Korrekturen oder Änderungen ergeben, werden diese dort vorab bereit gestellt.

Ordner | Zeugnisformulare
--|--
Berufsschule | Schul Z 500, Schul Z 501, Schul Z 502, Schul Z 503 
Berufsfachschule | Schul Z 520, Schul 521, Schul Z 522, Schul Z 523, Schul Z 526 

CHANGE | Zeugnisformular
--|--
BER-Schul Z 500 (09.19).rpt | Ausgabe X. Halbjahr der Berufsschule im Zeugniskopf korrigiert, wenn Ausbildungsbeginn im 2. HJ ist, wird nun das Halbjahr korrekt berechnet, Logo neu eingefügt, lange Fachbezeichnungen im Berufsübergreifenden Bereich sowie Wahlpflicht/Wahlunterricht werden zweizeilig ausgegeben
BER-Schul Z 501 (09.19).rpt | Fußnote 4 wird korrekt ausgegeben, das BIS-Datum für den Besuch des Schülers an der Schule wird aus dem Feld "Zeugnisdatum" im Menü Berufsschule > Matrix gezogen, Füllwerte o. B., b.f.werden wieder korrekt ausgegeben
BER-Schul Z 502 (09.19).rpt | das BIS-Datum für den Besuch des Schülers an der Schule wird aus dem Feld "Zeugnisdatum" im Menü Berufsschule > Matrix gezogen
BER-Schul Z 503 (09.19).rpt | Logo neu eingefügt, lange Fachbezeichnungen im Berufsübergreifenden Bereich sowie Wahlpflicht/Wahlunterricht werden zweizeilig ausgegeben

![Umbruch Fachbezeichnung des Berufsübergreifenden Bereiches (Schul Z 500, Schul Z 503)](/images/liesmich/6.5.42_01.png)

* NEW: BER-Schul Z 520 (09.19).rpt
* NEW: BER-Schul Z 521 (09.19).rpt
* NEW: BER-Schul Z 522 (09.19).rpt
* NEW: BER-Schul Z 523 (09.19).rpt
* NEW: BER-Schul Z 526 (09.19).rpt

#### Berlin (Allgemeinbildende Schulen)

* NEW: BER-Schul Z 255 (2019.2020).rpt
* NEW: BER-Schul Z 256 (2019.2020).rpt
* NEW: BER-Schul Z 324 (11.19).rpt
  
#### Saarland

* NEW: SAR-FHReife (Nachweis)(GOS2.0) Zweitschrift.rpt
* NEW: SAR-FHReife (Nachweis)(GOS2.0).rpt

> #### wichtig::Hinweis!
>
> Die Zeugnisse *SAR-FHReife (Nachweis)(GOS2.0) Zweitschrift.rpt* und *SAR-FHReife (Nachweis)(GOS2.0).rpt* werden Ihnen auf dem BSCW Server unter https://bscw.saarland.de/ bereit gestellt.

### Skripte

* NEW: BER-BFS-Matrix-2016.dws (Endnotenberechnung in der Berufsschulmatrix gemäß Berufsfachschulverordnung vom 14.07.2008, in der letzten Fassung vom 28.08.2016 Berlin) Eine Anleitung dazu finden Sie unter https://doc.la.stueber.de/berufsschule/ und https://doc.la.stueber.de/03.ber/ber-bfs-matrix-2016dws/
* CHANGE: NRW-APO-BK-2012 und NRW-APO-2012 Abschaffung der so genannten „Abweichungsprüfungen“, (d.h. verpflichtende mündliche Prüfungen im ersten bis dritten Abiturfach bei einer Abweichung der Prüfungsnote von der Vornote von vier oder mehr Punkten)