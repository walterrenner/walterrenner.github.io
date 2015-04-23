---
layout: default
---

## Hide email addresses from page source with Django

Inspired by Sarven Capadislis [Blog Post](http://csarven.ca/hiding-email-addresses#httpredirect).

~~~python
def email_me(request):
    response = HttpResponse("", status=302)
    response['Location'] = "mailto:me@email.com"
    return response
~~~
