---
layout: post
title: "Pulsing with CSS"
description: "Pulsing elements via CSS"
tags: [ Web, Development, CSS]
---

HTML:

{% include codeHeader.html %}
```
<div class="pulse"></div>
```

CSS:

{% include codeHeader.html %}
```
.pulse {
  box-shadow: 0 0 0 0 rgba(232, 76, 61, 0.7);
  cursor: pointer;
  -webkit-animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
  -moz-animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
  -ms-animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
  animation: pulse 1.25s infinite cubic-bezier(0.66, 0, 0, 1);
}
  @-webkit-keyframes pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}
  @-moz-keyframes pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}
  @-ms-keyframes pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}
  @keyframes pulse {to {box-shadow: 0 0 0 45px rgba(232, 76, 61, 0);}}
```
