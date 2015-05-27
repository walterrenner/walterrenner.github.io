---
layout: default
---

## Alle git repos pullen

~~~ bash
    for i in */.git ; do ( cd "${i/\/.*/}" ; git pull ) ; done
    # updates from all git repos below your CWD
~~~
