# Voraussichtliche Änderungen

Sie erhalten hier einen Überblick über die voraussichtlichen Änderungen und Korrekturen für das nächste Serviceupdate. Die nachfolgend gelisteten Änderungen wurden noch nicht veröffentlicht.

## Wichtiger Hinweis

> #### danger::Achtung!
>
> Bitte beachten Sie, dass unser Support für die jeweils aktuelle Ausgabe von MAGELLAN gilt, dass ist aktuell MAGELLAN 7.  **Die Unterstützung für MAGELLAN 6 wird Ende dieses Jahres eingestellt.** Eine Anleitung zum Umstieg von 6 auf 7 finden Sie [hier](https://doc.magellan7.stueber.de/schulverwaltung/update/umstieg-von-6-auf-7/).

## LEGENDE

| Abkürzung | Bedeutung |
| --- | --- |
| FIX | Korrektur bestehender Funktionalität |
| NEW | Neue Funktionalität |
| CHANGE | Änderung des Ablaufs, der Verarbeitung oder Bedienung |

---

## 6.5.41 - 673

### MAGELLAN

* FIX:

### Berichte

Eine Anleitung unserer Berichte finden Sie im Modul MAGELLAN BERICHTE, das Bestandteil der Installation ist und unter `Start > Programme > Stüber Systems > MAGELLAN BERICHTE` aufgerufen werden kann.

#### Berichte für Berlin

* FIX: BER-Schul Z 300 (11.19).rpt (Leerzeichen vor Datumsangabe eingefügt)
* CHANGE: BER-Schul Z 250 (11.19).rpt (es werden nur Wahlpflichtfächer ausgegeben, die eine Note im Feld "Endnote" eingetragen haben, Wahlpflichtfächer ohne Benotung werden nun auch in der Fachbezeichnung entwertet auf dem Zeugnis ausgegeben)
* FIX: BER-Schul Z 306 (11.19)(FG).rpt (Bereich der Zeugnisbemerkungen nun mit variabler Größe)
* FIX: BER-Schul Z 306 (11.19).rpt (Bereich der Zeugnisbemerkungen nun mit variabler Größe)

#### Berichte für Saarland

Unter ...Magellan\Berichte\Zeugnisse\Saarland\Ministerium finden Sie folgende Zeugnisformulare neu abgelegt. Eine Handout zu den Formularen finden auf dem BSCW-Server http://bscw.saarland.de.

* NEW: SAR-GY-AZ (Klassenstufen 5-10)+GEMS-AZ (Einführungsphase).rpt
* NEW: SAR-GY-AZ (modifiziert Klassenstufen 9 und 10).rpt
* NEW: SAR-GY-HJZ-JZ (Klassenstufen 5-10)+GEMS-HJZ-JZ (Einführungsphase).rpt
* NEW: SAR-GY-Verhaltenszeugnis.rpt
  
### Skripte

* FIX: DE-DIAP-2015.dws > Vorschlagsautomatik korrigiert (Einbringunsgverpflichtung mind. 2 HJ in Naturwissenschaften, optimale Punktzahl)
* FIX: DE-DIAP-2015.dws > Vorschlagsautomatik für FHR-Berechnung korrigiert, es werden nun die zulässigen 14 Kurse aus 7 Fächern im Vorschlag markiert
* CHANGE: Importiere SDTF.dws (Unterrichtsart-Schlüssel "L" ist hinzugekommen)
