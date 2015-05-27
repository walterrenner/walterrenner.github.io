---
layout: default
---

## Querverbindungen zu meinen Werkzeugen

Ich benutze im Alltag und auf der arbeit oft drei Werkzeuge: SublimeText, das Terminal und den Finder.

Ich arbeite oft im Kontext eines .git Repository. Das beudeutet ich schiebe im Finder Dateien hin und her. Aktiviere im Terminal virtuelle umgebungen oder starte Scripte. Und in SUblime editiere ich diverse Dateien. Oft muss ich in diesem "ordner"-Kontext zwischen diesen drei Applikationen wechseln.

Ziel ist es mit Tastatubbefehlen denselben ordner in den anderen Programmen zu öffnen

#####vom Terminal:
eine Finderfenster aud dem Teminal zu öffnen ist easy `open .`.
*   Sublime bitet eine * auf guithub gefunden `sublime .` es kann auch ein pfad angegeben werden.

#####vom Finder:
Dienste für Sublime
Shortcurt für Terminal in Systemeinstallungen -> Tastatur

#####von Sublime:
http://wbond.net/sublime_packages/terminal#Installation

~~~ python
[
{
    "keys": ["super+shift+o"],
    "command": "open_dir",
    "args":
        {"dir": "$file_path", "file": "$file_name"}
},
{
    "keys": ["super+shift+t"],
    "command": "open_terminal",
    "args": {
        "parameters": ["-T", "Working in directory %CWD%"]
    }
}
]
~~~
