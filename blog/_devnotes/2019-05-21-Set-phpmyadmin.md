---
layout: post
title: "Set PhpMyAdmin"
description: "Way to set phpmyadmin to listen only on localhost"
tags: [ Linux , command , shell ]
---


>$ sudo nano /etc/phpmyadmin/apache.conf

{% include codeHeader.html %}
```
Alias /phpmyadmin /usr/share/phpmyadmin
<Directory /usr/share/phpmyadmin>
    Options Indexes FollowSymLinks
    DirectoryIndex index.php

    Order deny,allow
    Deny from all
    Allow from 127.0.0.1
</Directory>
```
---