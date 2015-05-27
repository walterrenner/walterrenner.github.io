---
layout: default
---

## PEP-8 in einem Ordner ausführen und Ergebnisse in eine Datei schreiben

~~~ bash
    $ pip install pep8
    $ cd workspace/ptweb/
    $ pep8  --max-line-length=119 .|grep ": E" > ~/Desktop/ptweb.issues.txt
~~~

http://legacy.python.org/dev/peps/pep-0008/
