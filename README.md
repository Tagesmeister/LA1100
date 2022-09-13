# Projekt-Dokumentation


Pascal Oestrich

| Datum | Version | Zusammenfassung                                                                          |
| ----- | ------- | ---------------------------------------------------------------------------------------- |
|  23.08.2022     | 0.0.1   | Heute habe ich die User-Stories geschrieben und ein Pap vom Programm erstellt. |        
|  30.08.2022     | 0.0.2   |   Heute habe ich die wichtigsten Funktionen vom Spiel programmiert, nämlich die if und else schleifen. Dazu programmierte ich zum Spiel eine Wiederholfrage, wenn ich das Spiel fertig gespielt habe. |
|  06.09.2022     | 0.0.3   |   Das Spiel läuft Einwand frei. Ich habe dazu noch programmiert, dass das Programm bei einer falschen Eingabe nicht abstürzt. Am Ende des Spiels wird man ja noch gefragt, ob man weiter spielen oder aufhören möchte. Beim Beenden des Spiels wird eine kleine Ausgabe getätigt. Ich programmierte das Spiel so, dass jetzt das Design übersichtlich und gut aussieht. |

## 1 Informieren

### 1.1 Ihr Projekt

In meinem Projekt, werde ich ein kleines Spiel mit C# programmieren, in dem man eine Zahl zwischen 1 und 100 erraten soll.
### 1.2 User Stories

| US-№ | Verbindlichkeit | Typ  | Beschreibung                       |
| ---- | --------------- | ---- | ---------------------------------- |
| 1  |   Muss  | Funktional| Ich als Spieler möchte, dass meine erratete Zahl zwischen 1 und 100 liegt. Um das Spiel zu definieren.                                         |
| 2  |   Muss  | Funktional|    Der Spieler kann die Zahl erratene. Um das Spiel spielen zu können.                                                                         |
| 3  |   Muss  | Funktional|   Das Programm gibt für jede geraten zahl einen Hinweis aus. ("Die geratete Zahl ist niedriger als die Geheimzahl.") ("Die geratene Zahl ist grösser als die Geheimzahl.") ("Die Geheimzahl wurde erraten.") Dies ist wichtig, um das Spiel angenehmer zu gestalten.                                                                            |
| 4  |   Muss  | Funktional|   Wenn die Geheimzahl erraten wurde, soll die Anzahl der Rat versuche dargestellt werden. Diese Funktion dient dazu, zum zu sehen, wie viele versuche ich gebraucht habe.                            |
| 5  |   Muss  | Funktional|   Der Benutzer erwartet, dass das Programm mit Fehlereingaben umgehen kann. Das ist natürlich wichtig, um das Spiel angenehm spielen zu können.                                         |
| 6  |   Kann  | Qualität  |   Am Ende des Programms, erwartet der Spieler gefragt zu werden, ob er das Spiel weiter spielen oder beenden will. Dies dient dazu, um das Spiel schnell zu wiederholen. |
| 7  |   Kann  | Rand      |   Die Ausgaben vom Programm, sollen gut, schön und übersichtlich dargestellt werden. Diese Funktin schliesst die mögliche Verwirrung des Spielers aus.                               |



### 1.3 Testfälle

| TC-№ | Ausgangslage | Eingabe | Erwartete Ausgabe |
| ---- | ------------ | ------- | ----------------- |
| 1.1  |      Programm gestartet Eingabefeld ist bereit für Eingabe.       |    Zahl über 100     |      Die gesuchte Zahl liegt zwischen 1 und 100.             |
| 2.1 |        Programm gestartet Eingabefeld ist bereit für Eingabe.    |     Die gesuchte Zahl   |         "Die eingegebene Zahl ist korrekt!"         |
| 2.2 |        Programm gestartet Eingabefeld ist bereit für Eingabe.     |     Die falsche Zahl   |         Die gesuchte Zahl ist grösser/kleiner als die gesuchte Zahl (Das Eingabefeld erscheint.)       |
| 3.1 |        Programm gestartet Eingabefeld ist bereit für Eingabe.     |     Gebe eine höhere als die Gesuchte Zahl ein   |         "Die gesuchte Zahl ist kleiner" (eingegebene Zahl)       |
| 3.2 |        Programm gestartet Eingabefeld ist bereit für Eingabe.     |     Gebe eine kleinere als die Gesuchte Zahl ein   |        "Die gesuchte Zahl ist kleiner" (eingegebene ZahL)       |
| 3.3 |        Programm gestartet Eingabefeld ist bereit für eingabe.    |     Die gesuchte Zahl   |         "Supper deine gesuchte Zahl ist:" (Gesuchte Zahl)        |
| 4.1 |        Programm gestartet Geheim zahl wurde erratet und eingetippt  |    Enter   |         "Deine versuche:" (Anzahl versuche)        |
| 5.1 |        Programm gestartet Eingabefeld ist bereit für eingabe.    |     Gebe "Hallo Welt" ein   |         "Falsche Eingabe: Geben Sie eine Zahl ein!!" (Das Eingabefeld erscheint.)      |
| 5.2 |        Programm gestartet Eingabefeld ist bereit für eingabe.    |     Gebe "3.32" ein   |         "Falsche Eingabe: Geben Sie eine Zahl ein." (Das Eingabefeld erscheint.)        |
| 6.1 |        Programm gestartet, die Zahl wurde korrekt eingetippt.   |  Enter      |        "Willst du noch Einmal spielen? [ja|nein]" (Ein Feld erscheint, indem man ja eingeben kann."      |
| 6.2 |        Programm gestartet Ich werde gefragt, ob ich das Spiel wiederholen möchte.   |    ja   |         "Das Spiel wird wiederholt." (Eine neue Randomzahl wird generiert.    |
| 7.1 |        Die Zahl wurde richtig eigegeben |    Enter    |         (Alles ist schön untereinander aufgelistet.)        |


### 1.4 Diagramme

![image](https://user-images.githubusercontent.com/110892258/188563705-a478d185-8b44-4033-b98f-4c2925b4e7c8.png)

## 2 Planen

| AP-№ | Frist | Zuständig | Beschreibung | geplante Zeit |
| ---- | ----- | --------- | ------------ | ------------- |
| 1.A  |    23.08.2022   |      Ich    |     Die Projektbeschreibung geschrieben. Und Pap erstellen.        |       4        |
| 2.A  |    30.08.2022   |     Ich     |      Das Grundprinzip des Programms wird realisiert.       |       4        |
| 2.B  |    30.08.2022   |     Ich     |      Informieren: Von den Zusatzfähigkeiten des Programms (Wiederholfragen) (übersichtlichkeit) (Fehlerbehebung).    |       2        |
| 3.A  |    06.09.2022   |     Ich     |     Die Zusatzfähigkeiten des Programms werden realisiert (Wiederholfragen) (übersichtlichkeit) (Fehlerbehebung).       |       4        |
| 3.B  |    06.09.2022   |     Ich     |      Das Programm wird getestet und alle Probleme behoben.       |       4        |

Geplante zeit (Zahl) = 45 min.


Total: 18 * 45min = 810 min


## 3 Entscheiden


## 4 Realisieren

| AP-№ | Datum | Zuständig | geplante Zeit | tatsächliche Zeit |
| ---- | ----- | --------- | ------------- | ----------------- |
| 1.A  |  23.08.2022     |    Ich      |        4       |          3         |
| 2.A  |  30.08.2022     |    Ich      |        4       |          3         |
| 2.B  |  30.08.2022     |    Ich      |        2       |          1         |
| 3.A  |  06.09.2022  |    ich    |      4      |        4      |


## 5 Kontrollieren

### 5.1 Testprotokoll

| TC-№ | Datum | Resultat | Tester |
| ---- | ----- | -------- | ------ |
| 1.1  |    13.09.2022   |     Funktioniert nicht    |   Oestrich     |
| 2.1  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 3.1  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 3.2  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 3.3  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 4.1  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 5.1  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 5.2  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 6.1  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 6.2  |    13.09.2022   |     Funktioniert     |  Oestrich      |
| 7.1  |    13.09.2022   |     Funktioniert     |  Oestrich      |

#####Fazit:
Mein Programm funktionuert ganz gut, ausser wenn ich eine grössere Zahl als 100 eingebe, kommt eine falsche Ausgabe.


### 5.2 Exploratives Testen

| BR-№ | Ausgangslage | Eingabe | Erwartete Ausgabe | Tatsächliche Ausgabe |
| ---- | ------------ | ------- | ----------------- | -------------------- |
| I    |      Programm gestartet, Zahl wurde erraten. Ich werde gefragt, ob ich nich einmal spielen möchte.       |    alles ausser (ja)  und (nein)   |         Ungültige Eingabe          |          Programm schliesst sich.            |
| II |      Programm gestartet, Eingabefeld offen.       |     Eine Zahl die grösser als 100 ist    |       "Die gesuchte Zahl liegt zwischen 1 und 100."           |                      |

1. Alles funktioniert gut, man sollte doch noch implementieren, dass wenn man eine höhere Zahl als 100 und eine kleinere Zahl als 0 eingibt, ein Fehler auftaucht.
2. Am Ende wenn man nicht *nein* schreibt, sondern irgendetwas anders als *ja*, dann stürtzt den Programm trotzdem ab, obwohl man *nein* nicht eingegeben hat.

Mein Programm wurde von Lorenzo Lai überprüft.


## 6 Auswerten

✍️ Fügen Sie hier eine Verknüpfung zu Ihrem Lern-Bericht ein.
