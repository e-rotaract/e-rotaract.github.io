---
layout: default
permalink: /templates

author: eclub
logo:
  url: logo/rotaract-alpha.png
  position: center

pretitle: Pre-title
title: Title
description: Description

links-side: false

links-home:
    - name: Make a Donation
      icon: fa fa-hand-holding-heart
      url: "#donation"
      newtab: false
      show-home: true
      show-side: false
    - name: Street Kids Videocall
      icon: fa fa-video
      url: "#videocall"
      newtab: false
      show-home: true
      show-side: false

links-gallery:
  - left:
      name: RID 9212<br>Kenya 🇰🇪
      image: flags/ke.png
      url: https://fb.com/Rotaract-Club-of-Eco-Warriors-106271138555346
      newtab: true
    right:
      name: RID 1990<br>Switzerland 🇨🇭
      image: flags/ch.png
      url: https://rotary1990.ch
      newtab: true
  - left:
      name: RID 1960<br>Portugal 🇵🇹
      image: flags/pt.png
      url: https://www.rotary1960.org
      newtab: true
    right:
      name: RID 1780<br>France 🇫🇷
      image: flags/fr.png
      url: https://e-rotaract.com
      newtab: false

links-footer:
  - name: Make a Donation
    icon: fas fa-hand-holding-heart
    url: "#donation"
    newtab: false

show-notif: false

---

# Title 1

## Title 2

### Title 3

text *text* **text** ***text*** ~text~ ~~text~~

[internal link](/) [external link <a-out/>](https://iaco.io)

<code id="text">code</code>

{% include btn
  url="javascript:navigator.clipboard.writeText($('#text').text())"
  icon="fas fa-copy fa-lg"
  text="Copy Text"
%}

{% include img src="default-bg.jpg" %}

- list item
- list item

{% include btn
  url="/"
  newtab=true
  class="button-primary"
  icon="fa fa-video fa-lg"
  text="Button"
%}

{% include gallery-btn
  large=false
  items='[
    { name: "Copy Account Holder", icon: "fas fa-copy fa-lg", url: "javascript:navigator.clipboard.writeText($(\'#holder\').text())" },
    { name: "Copy IBAN Code", icon: "fas fa-copy fa-lg", url: "javascript:navigator.clipboard.writeText($(\'#iban\').text())" }
  ]'
%}
