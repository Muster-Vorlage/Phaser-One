# Kästchen-Jets

Ein Würfel-Duell auf Kästchenpapier für **2 Spieler an einem Gerät** oder **1 Spieler gegen den Computer** (Leicht / Mittel / Schwer).
Inspiriert von einem Papier-und-Stift-Spiel mit Jets, Würfel und Laser-Linien.

**Spielen:** `index.html` im Browser öffnen. Keine Installation, kein Build.

## Regeln

1. Jeder Spieler hat drei Jets: Blau oben, Rot unten. Jeder Jet hat einen Laser, der an seiner Nase beginnt.
2. Würfeln, dann einen eigenen Jet wählen und seinen Laser **genau so viele Kästchen** weiterziehen, wie der Würfel zeigt. Der Laser geht dort weiter, wo er zuletzt aufgehört hat.
3. Gezogen wird Kästchen für Kästchen: geradeaus oder um die Ecke, nie schräg.
4. Laser dürfen keine anderen Laser kreuzen, nicht durch eigene Jets und nicht über den Rand.
5. Erreicht ein Laser ein Kästchen eines gegnerischen Jets (gestrichelter Rahmen), ist der Jet abgeschossen. Der Zug endet sofort.
6. Bei einer Sechs wird nach dem Zug noch einmal gewürfelt.
7. Kommt der Laser nicht mehr weiter, endet der Zug früher. Kann ein Spieler gar nicht ziehen, verfällt sein Zug.
8. Wer zuerst alle drei gegnerischen Jets abschießt, gewinnt. Können beide nicht mehr ziehen, gewinnt, wer mehr Jets übrig hat.

## Bedienung

- Maus / Finger: auf die markierten Punkte tippen oder darüber wischen.
- Tastatur: Leertaste = würfeln, 1–3 = Jet wählen, Pfeiltasten = Laser zeichnen, Rücktaste = Schritt zurück.

## Computer-Gegner

Der Computer probiert alle möglichen Laserwege für den aktuellen Wurf durch und bewertet jede Stellung
über die kürzesten freien Wege (Breitensuche) zu den gegnerischen Jets: eigene Treffchancen hoch, gegnerische
Treffchancen niedrig. Dadurch greift er an und blockiert zugleich. „Mittel“ und „Leicht“ spielen absichtlich mit Zufall.
