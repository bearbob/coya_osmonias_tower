# Osmonias Turms

Osmonias Turm ist ein Abenteuer im Stil eines Choose-Your-Own-Adventure.
Mit Hilfe (mehr oder weniger) einfacher Definitionen in LaTeX und dem großartigen Template [rpgtex/DND-5e-LaTeX-Template](https://github.com/rpgtex/DND-5e-LaTeX-Template) wird ein kurzes Abenteuer beschrieben.

## Hilfsdefinitionen

### \block{<Name des Markers>}{<Überschift>}

Beginnt einen neuen Textblock und generiert eine Referenznummer, die im Text aufgerufen werden kann.
Beispiel: ```\block{theIntersectionRoomFromDungeon}{Ich habe die Wahl}```

### \goto{<Name des Markers>}

Erzeugt eine neue Referenz auf einen Textblock, der mit `\block{..}{..}` erzeugt wurde.
Im Text wird die Nummer des referenzierten Blocks ausgegeben.

### \getItem{<Name des Markers>}

Erzeugt eine neue Referenz auf eine Gegenstandsbeschreibung, die mit `\inventory{..}` erzeugt wurde.
Im Text wird der Buchstabe 'G' und die Nummer des referenzierten Gegenstands ausgegeben, z.B. `G16`.

### \inventory{<Name des Markers>}

Erzeugt eine neuen Zielreferenz für eine Gegenstandsbeschreibung.

### \setEvent{<Name des Markers>}

Erzeugt eine neuen Zielreferenz für eine Ereignisbeschreibung.

### \getEvent{<Name des Markers>}

Erzeugt eine neue Referenz auf eine Ereignisbeschreibung, die mit `\setEvent{..}` erzeugt wurde.
Im Text wird der Buchstabe 'E' und die Nummer des referenzierten Gegenstands ausgegeben, z.B. `E4`.
