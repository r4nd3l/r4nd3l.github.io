---
layout: post
title: "PHP send mail() setup"
description: "Install postfix apt package to send mail via php"
tags: [ Linux , command , shell, PHP ]
---

#### PHP send mail() setup
---

{% include codeHeader.html %}
```
    $ sudo apt-get install postfix
    $ sudo apt install -y mailutils
   ($ sudo dpkg-reconfigure postfix)
```