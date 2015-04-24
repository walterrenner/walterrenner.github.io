---
layout:     post
title:      Alle git repos pullen
categories: quicktip
---

~~~ bash
    for i in */.git ; do ( cd "${i/\/.*/}" ; git pull ) ; done
    # updates from all git repos below your CWD
~~~
