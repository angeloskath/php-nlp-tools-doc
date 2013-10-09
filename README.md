NlpTools Documentation
======================

This repository holds the documentation site of [NlpTools](http://php-nlp-tools.com/).

Format
------

The format used is markdown. At the beginning of the file
there is a section that starts with `----` and closed
with another `----` that is parsed as an ini configuration
string. The configuration looks like this:

```
----
[metadata]
title=Here goes a title
[options]
layout=layouts/page.php
----

Normal markdown here
```

Most commonly if you want to add a page you should simply
copy a similar page (if you want to add a blog post, copy
a blog post if you want to add documentation etc) and
edit the configuration section as little as possible.

### Code blocks ###

The documentation is parsed with [Markdown Extra][1] which
allows for fenced code blocks. You can create a fenced
codeblock with `~~~`. The parser passes the codeblock to
[Geshi][2] to provide syntax highlighting. This means that
you can use `~~~ php` to highlight php code `~~~ bash`
etc.

### File extension ###

The file extension should be **.gmd** otherwise there
will be no syntax highlighting.

External Files
--------------

To link to external files, add them to the files directory and
use an absolute path that contains the files directory. For
example:

```
This is an image of the clustering of the classic concentric
circular dataset with dbscan.
<img src="/files/clustering/dbscan_circles.png" class="border"/>
```


[1]: http://michelf.ca/projects/php-markdown/extra/
[2]: http://qbnz.com/highlighter/
