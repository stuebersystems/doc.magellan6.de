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


## 6.5.43 - 674

### MAGELLAN

* NEW: 

### Berichte

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

#### Berlin (Berufsbildende Schulen)

> #### wichtig::Hinweis!
>
> Die aktuellesten Zeugnisse und Anleitungen zu den Eingaben in MAGELLAN für jedes Zeugnis finden Sie  [hier](https://my.hidrive.com/share/qptlwhk642). Sollten sich nach Einspielen des Updates Korrekturen oder Änderungen ergeben, werden diese dort vorab bereit gestellt.

Ordner | Inhalt
--|--
BS Zeugnisse | Schul Z 500, Schul Z 501, Schul Z 502, Schul Z 503 
BFS Zeugnisse | Schul Z 520, Schul 521, Schul Z 522, Schul Z 523, Schul Z 526
IBA Zeugnisse | Schul Z 590
Berechnungsskripte | BER-BBS-Matrix-2016.dws, BER-BFS-Matrix-2016.dws, BER-IBA-HJ-2020.dws


CHANGE | BS Zeugnisformulare
--|--
BER-Schul Z 500 (09.19).rpt | Rechtschreibfehler BERUFSÜBERGREIFENDER UNTERRICHT
BER-Schul Z 501 (09.19).rpt | Rechtschreibfehler BERUFSÜBERGREIFENDER UNTERRICHT, Ausgabe Wahlb/WahlPF rechte Spalte korrigiert
BER-Schul Z 502 (09.19).rpt | Datum des Gesamtnotendurchschnittes entspricht dem Zeugnisdatum
BER-Schul Z 503 (09.19).rpt | Siegel blau eingefügt, Rechtschreibfehler BERUFSÜBERGREIFENDER UNTERRICHT, im Kopf "Die Leistungen in alle(n) Schulhalbjahren..... hier wurde "n" ergänzt


CHANGE | BFS Zeugnisformulare
--|--
BER-Schul Z 520 (09.19).rpt | Rechtschreibfehler BERUFSÜBERGREIFENDER UNTERRICHT
BER-Schul Z 521 (09.19).rpt |
BER-Schul Z 522 (09.19).rpt |
BER-Schul Z 523 (09.19).rpt | Rechtschreibfehler BERUFSÜBERGREIFENDER UNTERRICHT, Kopf "Abschlusszeugnisses der Berufsfachschule"
BER-Schul Z 526 (09.19).rpt | Rechtschreibfehler BERUFSÜBERGREIFENDER UNTERRICHT

CHANGE | IBA Zeugnisformulare
--|--
BER-Schul Z 590 (12.19).rpt | Rechtschreibfehler BERUFSÜBERGREIFENDER UNTERRICHT

* FIX: BER-Schul Z 300 (11.19).rpt (Versetzungsvermerk korrigiert, wird ein Schüler nicht versetzt, gibt des Zeugni "Nicht versetzt...." aus)

#### Saarland

> #### wichtig::Hinweis!
>
> Die Zeugnisse für Allgemeinbildende Schulen werden Ihnen auch über den [BSCW Server](https://bscw.saarland.de/) bereit gestellt.


* CHANGE: SAR-FHReife (Nachweis)(GOS2.0) Zweitschrift.rpt
* CHANGE: SAR-FHReife (Nachweis)(GOS2.0).rpt
  
### Skripte

* NEW: BER-IBA-HJ-2020.dws (Doku unter https://doc.la.stueber.de/03.ber/ber-iba-hj-2020dws/)