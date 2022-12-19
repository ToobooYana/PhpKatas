
# Bowling

Ein Bowling-Spiel besteht aus Würfen (engl. roll), um 10 Pins am Ende der Bowling-Bahn abzuräumen. Mit jedem Wurf können also 0 bis 10 Pins umgeworfen werden. Pro Runde hat ein Spieler max. 2 Würfe, um die 10 Pins abzuräumen.

Würfe werden zu Rahmen (engl. frame) zusammengefasst, die jeweils eine Punktzahl zugeordnet bekommen. Ein Spiel besteht aus 10 Runden oder Rahmen.

Wieviele Würfe pro Runde von einem Spieler gemacht werden dürfen, hängt davon ab, wieviele Pins mit ihnen geworfen werden:

-   Wenn der erste Wurf eines Spielers alle 10 Pins abräumt (engl. strike), ist er der einzige Wurf in der Runde.
-   Ansonsten enthalten die Rahmen immer zwei Würfe, jeder mit 0 bis 10 Pins.
    -   Ausnahme: Wenn der 10. Rahmen als ersten Wurf einen strike enthält oder beide Würfe zusammen einen spare (s.u.) ergeben, dann kann ein drittes Mal geworfen werden.

Für die Berechnung der Punktzahl eines Rahmens gibt es einige Regeln:

-   Ein Rahmen, dessen beide Würfe zusammen maximal 9 Pins gerissen haben, erhält die Summe der Pins als Punktzahl.
-   Ein Rahmen dessen beide Würfe zusammen 10 Pins gerissen haben (engl. spare), erhält als Punktzahl 10 + die Zahl der Pins des nächsten Wurfes.
-   Ein Rahmen mit einem strike erhält als Punktzahl 10 + die Summe der Pins der nächsten beiden Würfe.

Bei Robert C. Martin findet sich diese Darstellung für ein Bowling-Spiel:

![enter image description here](https://github.com/ToobooYana/PhpKatas/blob/main/Bowling/bowlinframe.png)

Jeder Rahmen zeigt den ersten und zweiten und beim letzten sogar den dritten Wurf mit ihren Pins sowie die kummulierte Punktzahl. Ist das Kästchen für den zweiten Wurf halb ausgefüllt, liegt ein spare vor, ist es ganz ausgefüllt, war der erste Wurf ein strike.


# User Story 1

Erstelle ein Programm, das beim Benutzer abfragt, wieviele Pins bei den einzelnen Rahmen geworfen wurden. Am Ende der Eingabe der letzten Würfe für Rahmen Nummer 10 soll dann das Gesamtergebnis angezeigt werden.
Das kann als Webanwendung erstellt werden oder als Konsolenanwendung.

# User Story 2 

Nun wird das Programm erweitert. Das Spiel soll nun für zwei Personen gedacht sein. Am Anfang sollen die beiden Personen ihre Namen schreiben. Danach wird im Wechsel abgefragt, wieviele Pins pro Frame geworfen wurden. Zum Schluss wird dann der Name und das Gesamtergebnis von Spieler 1 und Spieler 2 ausgegeben. 


# Hinweis

Fange mit kleinen Schritten an. Erstelle für jeden kleinen Schritt schon mal einen Unit-Test und lasse immer alle Unit-Test laufen, um zu prüfen, ob die Software noch weiter korrekt läuft. Im ersten Schritt kannst du z.B. die 1. Regel umsetzen. Danach setzt du im 2. Schritt die 2. Regel um ("Ein Rahmen dessen beide Würfe zusammen 10 Pins gerissen haben (engl. spare), erhält als Punktzahl 10 + die Zahl der Pins des nächsten Wurfes.") und dann folgt Regel Nr. 3.

Viel Erfolg! :-)
