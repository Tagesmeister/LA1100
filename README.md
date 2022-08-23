# Projekt-Dokumentation


Pascal Oestrich

| Datum | Version | Zusammenfassung                                                                          |
| ----- | ------- | ---------------------------------------------------------------------------------------- |
|  23.08.2022     | 0.0.1   | Heute habe ich die User-Stories geschrieben und ein Pap vom programm erstellt.   |        
|                 | ...     |                                                                                |
|                 | 1.0.0   |                                                                                |

## 1 Informieren

### 1.1 Ihr Projekt

In meinem Projekt, werde ich ein kleines Spiel mit C# Programmieren, in dem man eine Zahl zwischen 1 und 100 eraten soll.
### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1  |   Muss  | Funktional| Ich als Spieler möchte, dass meine erratete Zahl zwischen 1 und 100 liegt. Um das Spiel du deffinieren.                                         |
| 2  |   Muss  | Funktional|    Der Spieler kann die Zahl erraten. Um das Spiel spielen zu können.                                                                         |
| 3  |   Muss  | Funktional|   Das Programm gibt für jede geratete zahl einen Hinweis aus. ("Die geratete Zahl ist niedriger als die Geheimzahl.") ("Die geratene Zahl ist grösser als die Geheimzahl.") ("Die Geheimzahl wurde erraten.") Dies ist wichtig, um das Spiel angenehmer zu gestalten.                                                                            |
| 4  |   Muss  | Funktional|   Wenn die Geheimzahl erraten wurde, soll die Anzahl der Ratversuche dargestellt werden. Dieses Funktion dient dazu, zum zu sehen, wie viele versuche ich gebraucht habe.                            |
| 5  |   Muss  | Funktional|   Der Benutzer erwartet, dass das Programm mit Fehlereingaben umgehen kann. Das ist natürlich wichtig, um das spiel angenehm spielen zu können.                                         |
| 6  |   Kann  | Qualität  |   Am Ende des Programms, erwartet der Spieler gefragt zu werden, ob er das Spiel weiter spielen oder beenden will. Dies dient dazu um das Spiel schnell zu wiederholen. |
| 7  |   Kann  | Rand      |   Die Ausgaben vom Programm, sollen gut, schön und übersichtlich dargestellt werden. Diese Funktin schliesst die mögliche Verwirung des Spielers aus.                               |


### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |      Programm gestartet Eingabefeld ist bereit für eingabe.       |    Zahl über 100     |      Die gewünschte Zahl liegt zwischen 1 und 100.             |
| 2.1 |        Programm gestartet Eingabefeld ist bereit für eingabe.    |     Die gesuchte Zahl   |         "Die eingegebene Zahl ist Korrekt!"         |
| 2.2 |        Programm gestartet Eingabefeld ist bereit für eingabe.     |     Die falsche Zahl   |         "Die eingegebene Zahl ist flasch!" (Das Eingabefeld erscheint.)       |
| 3.1 |        Programm gestartet Eingabefeld ist bereit für eingabe.     |     Gebe eine höhere als die Gesuchte Zahl ein   |         "Die eingegebene Zahl ist zu hoch!"       |
| 3.2 |        Programm gestartet Eingabefeld ist bereit für eingabe.     |     Gebe eine kleinere als die Gesuchte Zahl ein   |         "Die eingegebene Zahl ist zu klein!"       |
| 3.3 |        Programm gestartet Eingabefeld ist bereit für eingabe.    |     Die gesuchte Zahl   |         "Die Glückszahl ist Korrekt!"         |
| 4.1 |        Programm gestartet Geheim zahl wurde erratet   |       |         "Die eingegebene Zahl ist korrekt! Hier sind Ihre versuche: (Anzahl versuche)        |
| 5.1 |        Programm gestartet Eingabefeld ist bereit für eingabe.    |     Gebe "Hallo Welt" ein   |         "Es ist eine Zahl gesucht! versuche es nochmal."  (Das Eingabefeld erscheint.)      |
| 5.2 |        Programm gestartet Eingabefeld ist bereit für eingabe.    |     Gebe "3.32" ein   |         "Es sind ganze Zahlen gesucht! versuche es nochmal." (Das Eingabefeld erscheint.)        |
| 6.1 |        Programm gestartet Die Zahl wurde korrekt eingegeben.   |        |         "Möchten Sie das Spiel wiederholen? Dann schreiben Sie wiederholen." (Ein Feld erscheint, indem man wiederholen eingeben kann."      |
| 6.2 |        Programm gestartet Ich werde gefragt, ob ich das Spiel wiederholen möchte.   |    Wiederholen   |         "Das Spiel wird wiederholt." (Das Spielt beginnt von Vorne.    |
| 7.1 |        Das Programm ist am Ende|        |         (Alles ist schön untereinander aufgelistet.)        |


### 1.4 Diagramme

✍️ Hier können Sie PAPs, Use Case- und Gantt-Diagramme oder Ähnliches einfügen.

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |    23.08.2022   |      Ich    |     Die Projektbeschreibung geschrieben. Und Pap erstellen.        |       4        |
| 2.A  |    30.08.2022   |     Ich     |      Das Grundprinzip des Programms wird realisiert.       |       4        |
| 2.B  |    30.08.2022   |     Ich     |      Informieren: Von den Zusatzfähigkeiten des Programms (Wiederholfrage) (übersichtlichkeit)     |       2        |
| 3.A  |    06.09.2022   |     Ich     |     Die Zusatzfähigkeiten des Programms werden realisiert.       |       4        |
| 2.A  |    13.09.2022   |     Ich     |      Das Programm wird getestet und alle Probleme behoben.       |       4        |

Geplante zeit (Zahl) = 45 min.


Total: 18 * 45min = 810 min


## 3 Entscheiden

✍️ Dokumentieren Sie hier Ihre Entscheidungen und Annahmen, die Sie im Bezug auf Ihre User Stories und die Implementierung getroffen haben.

## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |       |           |               |                   |
| ...  |       |           |               |                   |

✍️ Tragen Sie jedes Mal, wenn Sie ein Arbeitspaket abschließen, hier ein, wie lang Sie effektiv dafür hatten.

## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |       |          |        |
| ...  |       |          |        |

✍️ Vergessen Sie nicht, ein Fazit hinzuzufügen, welches das Test-Ergebnis einordnet.

### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |              |         |                   |                      |
| ...  |              |         |                   |                      |

✍️ Verwenden Sie römische Ziffern für Ihre Bug Reports, also I, II, III, IV etc.

## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
