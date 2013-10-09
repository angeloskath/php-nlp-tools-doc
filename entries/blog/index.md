---
[metadata]
title = Blog
[options]
layout=layouts/posts.php

; Blog provider
providers[Collection] = 'post'

; paginate results
generators[] = Pagination
paginate_on = Collection

---
