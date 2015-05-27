---
layout: default
---

## Widerrufene Zertifikate in Chrome sperren

**[Update 27. Mai 2015]** Die beschriebene Einstellung wurde aus Chrome mittlerweile entfernt.


Nach der letztlich bekannt gewordenen Sicherheitslücke in der OpenSSL-Bibliothek, die unter dem Namen [Heartbleed](http://heartbleed.com/ "Heartbleed Website") bekannt wurde, empfehle ich jedem seine Sicherheitseinstellungen in Chrome anzupassen.

In den erweiterten Einstellungen, erreichbar unter `chrome://settings/#advanced-settings-expander`, setzt man das Häkchen für "Check for server certificate revecation". Hiermit werden wirderrufene Zertifikate für HTTPS-Verbindungen nicht mehr akzeptiert.

Um die vorgenommenen Einstellungen zu überprüfen könnt ihr diese [Testseite](https://revoked.grc.com/ "Testseite für widerrufe Zertifikate") besuchen und Chrome sollte euch eine Fehlermeldung zeigen.

Weitere nütztliche Einstellungen für den Browser von Google hat [@mkalina](https://twitter.com/mkalina/) in seinem [Blog-Artikel](https://mkln.org/2014/05/maximaler-datenschutz-mit-google-chrome/) zusammengefasst.
