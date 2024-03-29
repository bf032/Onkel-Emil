---
title: "Codebuch Onkel Emil"
author: "Hanna Bekele, Berenice Fengler, Nina Walter, Anika Geiger"
date: "21/05/2022"
output: html_document
editor_options: 
  markdown: 
    wrap: 72
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

Das Netzwerk ist ein *gerichtetes* two-mode Netzwerk.

# EDGE-Attribute

**id**

eindeutige Identifikation jedes einzelnen Knotens (vertex), der erfasst
wird, selbst ernannte Abkürzungen

**from**

definiert den Sender in gerichteten Netzwerken. Entspricht ID in der
Nodelist.

**to**

definiert den Empfänger in gerichteten Netzwerken. Entspricht ID in der
Nodelist.

**relationship**

definiert Beziehungsart zwischen zwei Akteuren

1 = *Liebesbeziehung* Liebesbeziehung zwischen zwei Akteuren\
2 = *Verwandtschaft* Diese Akteure sind miteinander verwandt\
3 = *Rekrutierung* Wer hat wen in den Freundeskreis gebracht?

**start_relationship**

Beginn der Beziehung

**end_relationship**

Ende der Beziehung

**role**

Rolle eines Akteurs bei einer Aktion, codiert nach

1 = Lebensmittel besorgen\
2 = Unterkunft stellen\
3 = Papiere besorgen\
4 = Krankschreibungen/ Arbeitsunfähigkeitsbescheinigungen\
5 = Informationen beschaffen\
6 = Hilfe bei Flucht\
7 = Geldbeschaffung\
10 = Hilfeleistungen empfangen\
11 = ärztliche Versorgung\
12 = Rechtsauskunft\

# NODE-Attribute

**id**

eindeutige Identifikation jedes einzelnen Knotens (vertex), der erfasst
wird, selbst ernannte Abkürzungen

**name**

Name der Person bzw. Aktion

**name_short**

Personen: Vorname oder Nachname, wenn voller Name nicht bekannt\
Aktionen: selbstgewählte Abkürzungen

**type**

0 = Person\
1 = Aktion

**sex**

1 = weiblich\
2 = männlich\

**year_birth**

Jahr der Geburt

**year_death**

Jahr des Todes

**profession**

Welcher Berufsgruppe hat er/sie angehört?

1 = Recht (Jurist)\
2 = Medien/Druck (Journalist, Drucker, Grafiker)\
3 = Kunsthandwerk (Dirigent, Musiker, Schauspieler)\
4 = Bildung (Studienrat, Gesandtschaftsrat)\
5 = Gesundheitswesen (Arzt)\
6 = Soziales & Religion (Pfarrer)\
7 = Ernährung/Handel (Konditor)\
8 = Militär\
9 = Anderes

**membership**

Ist der-/diejenige Mitglied oder nur Unterstützer der Gruppe?

1 = Mitglied\
2 = Stammgruppe\
3 = Unterstützer\
4 = Geholfene Personen\
5 = Geholfen und Mitglied\
6 = Geholfen und Stammgruppe\
7 = Geholfen und Unterstützer

**joining**

Jahr des Beitritts zur Gruppe Onkel Emil

**leaving**

Wann hat er/sie die Gruppe verlassen?

**type_action**

Um welche Art von Aktion handelt es sich?

1 = Hilfsaktionen\
2 = aktiver Protest gegen das NS-System

**year_action**

In welchem Jahr war die Aktion?
