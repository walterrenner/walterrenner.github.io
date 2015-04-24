---
layout:     post
title:      Widerrufene Zertifikate in Chrome sperren
categories:
---

**[Update 25. April 2015]** Die beschriebene Einstellung wurde aus Chrome mittlerweile entfernt.


Nach der letztlich bekannt gewordenen Sicherheitslücke in der OpenSSL-Bibliothek, die unter dem Namen [Heartbleed](http://heartbleed.com/ "Heartbleed Website") bekannt wurde, empfehle ich jedem seine Sicherheitseinstellungen in Chrome anzupassen.

In den erweiterten Einstellungen, erreichbar unter `chrome://settings/#advanced-settings-expander`, setzt man das Häkchen für "Check for server certificate revecation". Hiermit werden wirderrufene Zertifikate für HTTPS-Verbindungen nicht mehr akzeptiert.

![](/images/chrome_cert_settings.png "Screenshot Chrome Einstellungen")

Um die vorgenommenen Einstellungen zu überprüfen könnt ihr diese [Testseite](https://revoked.grc.com/ "Testseite für widerrufe Zertifikate") besuchen und Chrome sollte euch die untere Fehlermeldung zeigen.

![Chrome Fehlermeldung beim Aufruf einer Website mit widerrufenem Zertifikat](/images/revoked_cert_error.png)

Weitere nütztliche Einstellungen für den Browser von Google hat [@mkalina](https://twitter.com/mkalina/) in seinem [Blog-Artikel](https://mkln.org/2014/05/maximaler-datenschutz-mit-google-chrome/) zusammengefasst.
