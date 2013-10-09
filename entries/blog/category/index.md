---
[metadata]
title = Mini nlp projects
[options]
layout=layouts/posts.php

; Blog provider
providers[Collection] = 'post&sort=asc'

; break on category
generators[] = TagArray
array_on = Collection
tagname = project

; paginate results
generators[] = Pagination
paginate_on = Collection
ipp = 1

---
