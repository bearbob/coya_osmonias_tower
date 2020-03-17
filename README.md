# Osmonias Turms

Osmonias Turm ist ein Abenteuer im Stil eines Choose-Your-Own-Adventure.
Mit Hilfe (mehr oder weniger) einfacher Definitionen in LaTeX und dem großartigen Template [rpgtex/DND-5e-LaTeX-Template](https://github.com/rpgtex/DND-5e-LaTeX-Template) wird ein kurzes Abenteuer beschrieben.

## Hilfsdefinitionen

### \block{<Name_des_Markers>}{<Überschift>}

Beginnt einen neuen Textblock und generiert eine Referenznummer, die im Text aufgerufen werden kann.
Beispiel: ```\block{theIntersectionRoomFromDungeon}{Ich habe die Wahl}```

### \goto{<Name_des_Markers>}

Erzeugt eine neue Referenz auf einen Textblock, der mit `\block{..}{..}` erzeugt wurde.
Im Text wird die Nummer des referenzierten Blocks ausgegeben.

### \getItem{<Name_des_Markers>}

Erzeugt eine neue Referenz auf eine Gegenstandsbeschreibung, die mit `\inventory{..}` erzeugt wurde.
Im Text wird der Buchstabe 'G' und die Nummer des referenzierten Gegenstands ausgegeben, z.B. `G16`.

### \inventory{<Name_des_Markers>}

Erzeugt eine neuen Zielreferenz für eine Gegenstandsbeschreibung.

### \setEvent{<Name_des_Markers>}

Erzeugt eine neuen Zielreferenz für eine Ereignisbeschreibung.

### \getEvent{<Name_des_Markers>}

Erzeugt eine neue Referenz auf eine Ereignisbeschreibung, die mit `\setEvent{..}` erzeugt wurde.
Im Text wird der Buchstabe 'E' und die Nummer des referenzierten Gegenstands ausgegeben, z.B. `E4`.
