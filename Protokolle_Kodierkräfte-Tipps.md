# Protokoll vom Interview der Kodierkräfte (Hr. Abraham, Hr. Franke) am 29.11.2019

* KJP: Liebigstraße ... 
* Psychiatrie: Semmelweisstraße ...

## Zum Patientenverlauf:

* Aufnahme: Ambulanz oder Aufnahme
    * Aufnahmegespräch mit dem Arzt
    * Diagnosestellung
    * Entscheidung stationär / Tagesklinik (Scorer-Formulare, PsychPV)
    * Patientenakte wird angelegt
    * Therapieplanung

* Wiederkehrender Prozess aus:
    * Neuen Diagnosen
    * Neuen Therapien
* Entlassung:
    * Arztbrief
    * Abrechnung


## Systeme:
* Papierakte:
    * Medikation
    * Laborbefunde
    * Fieberkurven usw.

* SAP:
    * Belegungsplan
    * Patientenorganizer (elektr. Patientenakte)
    * Ärztlicher und Pflegerischer Verlauf (Fließtext) <- Wer macht das?

* RKT (SAP-Produkt):
    * Wird erst durch die Anfrage der KRankenkasse / MDK interessant
    * Verwaltungsseite des SAP
    * Unterlagenversand usw.
    * **Für unsere Analyse nicht relevant**
    
* ID-Scorer-Psych:
    * Aufruf über SAP-Komfortkodierung
    * beeinhaltet die Einstufungen Regelpatient / Akutpatient (Psych-PV)
    * Verläufe:
        * Ärzte
        * Pflege
        * Spezialtherapeuten
        * Psychologen
    * Grouper IDDiaCos erstellt aus all diesen Daten die OPS-Schlüssel
    * Fehlende Einträge werden rot markiert (Hier entstehen Verluste)
    * Inhaltliche Dokumentation: Freitext, schlecht für Grouper geeignet
    * Aufnahme von Diagnosen und Therapieplänen ist hier möglich, verlangsamt das System aber immens
    * Klick auf "Verschlüsseln und Kodieren" führt zum IDDiacos

* IDDiacos:
    * Grouper für PEPP-Codes (Erstellt aus den Diagnose- und Therapieschlüsseln Abrechnungscodes)
    * Eintragung der Diagnoseschlüssel und OPS-Codes erfolgt hier (laufender Prozess)
    * Ein Code -> Eine Hauptdiagnose

* HYDMedia:
    * Archivprogramm (retrospektive Fallauswertung)
    * hält eingescannte Patientenakten
    * grobe Gliederung:
        * Anamnese / Verlauf
        * Befunde
        * Arztbriefe (syn. Epikrise, Entlassungsbrief)
        * Concealings ... ?
        * Klinik/Pflege/Sonstiges


## Zur PPP-Richtlinie:
* Patienten müssen eigentlich täglich eingestuft werden (bsp intensiv / nicht-intensiv)
* Rechnungen sind nach Entlassung der Patienten nicht mehr änderbar (Nachtragungen nicht möglich)
* Personalaufwandserfassung muss 14-tägig übertragen werden


## Probleme:
* Visiten werden schriftlich dokumentiert, aber nicht im System niedergeschrieben / in OPS-Codes umgwandelt. 
* Einheitliche Dokumentation zwischen den Stationen fehlt.
* Immernoch viele Händische Dokumente, bsp. Dienstpläne und Therapiepläne
* Wenn der Aufwand nicht vollständig dokumentiert ist, kann es zum Streichen von Stellen kommen

### Besonderheit:
* Förderung durch den Staat sorgt dafür, dass Änderung meist kritisch gegenüber gestanden wird, da die Finanzierung geregelt gesichert ist
