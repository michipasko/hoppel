# Hoppel!

## Elevator Pitch
Ein Kleinkind drückt eine beliebige Taste — und ein kleiner Hase springt
quietschfidel an einer zufälligen Stelle aus dem Gras hervor. Keine Regeln,
kein Scheitern, nur reines Staunen und Freude bei jedem Tastendruck.

## Genre & Plattform
- **Genre:** Reaktionsspiel / Sensorisches Spielzeug (kein klassisches Spiel
  mit Gewinn-/Verlustbedingung)
- **Plattform:** Desktop-Browser oder lokale Anwendung (Vollbild)
- **Perspektive:** 2D, Frontalansicht

## Hauptcharakter
- **Name:** Hoppel
- **Aussehen:** Ein rundlicher, weicher Hase in warmem Hellgrau oder Cremeweiß,
  mit großen Augen und langen Ohren — bewusst einfach und klar gezeichnet,
  damit er auch für sehr junge Kinder sofort erkennbar ist
- **Persönlichkeit:** Verspielt, überraschungsfreudig, immer gut gelaunt
- **Animation:** Hoppel springt aus dem Gras hervor (kurze Auf-Animation),
  bleibt einen Moment sichtbar mit einer kleinen Idle-Animation (Ohren
  wackeln, Nase zuckt), und verschwindet dann langsam wieder im Gras — bereit
  für den nächsten Auftritt

## Spielziel
Es gibt kein klassisches Spielziel. Das Erlebnis ist das Ziel: Taste drücken,
Hase erscheint, Kind staunt und lacht. Der Kreislauf wiederholt sich
unendlich ohne Zeitlimit oder Punktestand.

## Kernmechaniken

1. **Universelle Tastatureingabe**
   Jede beliebige Taste auf der Tastatur loest denselben Effekt aus. Es gibt
   keine "falsche" Taste. Auch die Leertaste, Pfeiltasten und Zifferntasten
   funktionieren.

2. **Zufaelliges Erscheinen**
   Bei jedem Tastendruck erscheint Hoppel an einer zufaelligen horizontalen
   Position am unteren Bildschirmrand — immer aus dem Gras hervorspringend.
   Die Position wird so gewaehlt, dass Hoppel immer vollstaendig sichtbar ist
   (kein Abschneiden am Rand).

3. **Sofortiges visuelles & akustisches Feedback**
   Der Tastendruck loest unmittelbar aus: Animation startet sofort (keine
   Verzoegerung), begleitet von einem kurzen, froehlichen Geraeusch (z. B.
   ein weiches "Boing" oder ein froehliches Quietschen). Kinder in diesem
   Alter brauchen unmittelbare Rueckkopplung.

4. **Sanfter Disappear-Effekt**
   Nach ca. 1,5–2 Sekunden verschwindet Hoppel wieder langsam im Gras
   (kurze Runter-Animation). Wird eine neue Taste gedrueckt waehrend Hoppel
   noch sichtbar ist, erscheint er sofort an einer neuen Stelle — der alte
   Auftritt bricht sauber ab.

5. **Ruhiger Hintergrund**
   Eine einfache, freundliche Wiese mit Grasgruppen am unteren Rand. Kein
   ablenkender Hintergrund, keine bewegten Elemente ausser Hoppel selbst.
   Optional: sanfte Hintergrundmusik (Kindergarten-Stil, leise).

## Welt & Level
Es gibt genau eine Szene: eine sonnige Wiese. Keine Level, keine
Leveluebgaenge, keine Fortschrittsanzeige. Die Wiese ist immer gleich —
Verlasslichkeit und Wiederholung sind fuer Kleinkinder wichtig und beruhigend.

Optional fuer eine spaetere Ausbaustufe (Version 2, kein Scope-Creep jetzt):
- Jahreszeiten-Themes (Schnee im Winter, Herbstblaetter) als rein optische
  Variante ohne Auswirkung auf das Spielprinzip

## Visueller Stil & Stimmung
- **Stil:** Weich, rund, bunt — inspiriert von Bilderbuch-Illustrationen.
  Keine scharfen Kanten, keine dunklen Farben.
- **Farbpalette:** Warmes Gruen fuer die Wiese, helles Blau fuer den Himmel,
  Cremeweiß/Hellgrau fuer Hoppel. Pastelltoene insgesamt.
- **Stimmung:** Geborgen, verspielt, ueberraschungsfreudig. Das Spiel soll
  sich anfuehlen wie ein Guckkastenspiel oder ein "Wo ist Hoppel?"-Bilderbuch.
- **Schriften:** Keine Texte im Spiel notwendig. Kinder in diesem Alter lesen
  nicht. Hoechstens ein einfaches Logo auf dem Startbildschirm.

## Zielgruppe
- **Primaer:** Kleinkinder im Alter von 1–2 Jahren
- **Sekundaer:** Eltern und Betreuungspersonen, die gemeinsam mit dem Kind
  spielen und die Tastatur fuehren
- **Wichtig:** Das Spiel muss kindsicher sein — kein Zugriff auf
  Systemfunktionen, Vollbildmodus empfohlen, keine Links oder externe Inhalte

## Empfohlene Technologie

**Empfehlung: Python mit pygame**

- **Begruendung:** pygame eignet sich hervorragend fuer dieses Projekt, weil
  das Spiel als lokale Desktop-Anwendung laeuft (kein Browser notwenig), die
  Tastatureingabe direkt und ohne Verzoegerung abgefangen werden kann, und
  der Einstieg auch fuer weniger erfahrene Entwickler machbar ist.
- **Vollbild:** pygame unterstuetzt nativen Vollbildmodus, der verhindert,
  dass das Kind versehentlich das Fenster schliesst.
- **Alternativ:** Phaser.js (JavaScript, laeuft im Browser) — etwas mehr
  Aufwand beim Einrichten, dafuer ohne Installation auf jedem Geraet nutzbar.
- **Nicht empfohlen fuer dieses Projekt:** Godot oder Unity — zu viel Overhead
  fuer ein so fokussiertes Mini-Spiel.

## Naechste Schritte

1. **Grafiken erstellen** — Hoppel als Sprite mit 3 Animationsphasen:
   Hervorspringen, Idle (Ohren wackeln), Verschwinden. Wiese als
   Hintergrundbild.
2. **Soundeffekte besorgen** — 1 Sprung-Sound, optional 1 Hintergrundmelodie.
   Lizenzfreie Quellen: freesound.org, OpenGameArt.org.
3. **Prototyp bauen** — Nur Tastatureingabe, zufaellige Position, Sprite
   anzeigen. Kein Sound, keine Animation — erst mal funktional.
4. **Animation & Sound integrieren** — Sobald der Prototyp laeuft.
5. **Testen mit echten Kleinkindern** — Beobachten, ob das Feedback schnell
   genug ist und ob Hoppel sichtbar genug reagiert.
6. **Vollbildmodus & Kindsicherung aktivieren** — Vor dem echten Einsatz.
