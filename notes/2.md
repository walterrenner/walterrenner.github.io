---
layout: default
---

## Delete all sessions within a Django management shell

~~~bash
$ ./manage.py shell
~~~

~~~python
from django.contrib.sessions.models import Session
Session.objects.all().delete()
~~~
