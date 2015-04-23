---
layout: default
---

## Get Django admin url for model instance

Source: [http://stackoverflow.com/questions/10420271/django-how-to-get-admin-url-from-model-instance](http://stackoverflow.com/questions/10420271/django-how-to-get-admin-url-from-model-instance)

~~~python
from django.core import urlresolvers
from django.contrib.contenttypes.models import ContentType
from django.db import models

class AdminURLModel(models.Model):
    class Meta:
        abstract = true

    def get_admin_url(self):
        content_type = ContentType.objects.get_for_model(self.__class__)
        return urlresolvers.reverse("admin:%s_%s_change" % (content_type.app_label, content_type.model), args=(self.id,))
~~~
