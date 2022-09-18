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

# Make a Donation {#donation}

With **150 euros/swiss francs per month**, we can feed a kid two meals a day and provide them with shelter and education: school, supplies, clothes!

<!--
<p style="text-align: center;">
  <a href="https://donorbox.org/street-kids-rotaract?default_interval=o" target="_blank" class="button button-primary">
    <i class="fas fa-hand-holding-heart fa-lg"></i> Donate to Street Kids
  </a>
</p>
-->

To donate through a bank transfer, here is our details:

- Account holder: <code id="holder">District Rotary 1990, Comission Rotaract</code>
- IBAN: <code id="iban">CH30 8080 8003 8478 5531 6</code>

{% include btn
  url="javascript:navigator.clipboard.writeText($('#holder').text())"
  icon="fas fa-copy fa-lg"
  text="Copy Account Holder"
%}

{% include btn
  url="javascript:navigator.clipboard.writeText($('#iban').text())"
  icon="fas fa-copy fa-lg"
  text="Copy IBAN"
%}

{% include gallery-btn
  large=false
  items='[
    { name: "Copy Account Holder", icon: "fas fa-copy fa-lg", url: "javascript:navigator.clipboard.writeText($('#holder').text())" },
    { name: "Copy IBAN", icon: "fas fa-copy fa-lg", url: "javascript:navigator.clipboard.writeText($('#iban').text())" }
  ]'
%}

{% include gallery
  shuffle=false
  grid=2
  items='[
    { img: "actions/street-kids/pack-1.png", url: "#donation" },
    { img: "actions/street-kids/pack-2.png", url: "#donation" },
    { img: "actions/street-kids/pack-3.png", url: "#donation" },
    { img: "actions/street-kids/pack-4.png", url: "#donation" }
  ]'
%}

# We are 100% Transparent

Here you can find all the financial receipts of our project. If you have questions, do not hesitate to contact us!

{% include btn
  url="https://www.dropbox.com/sh/iw2gokqs1dj3cig/AAAv_yq9HUx46d1n5YmXcKbha?dl=0"
  newtab=true
  class="button-success"
  icon="fab fa-dropbox fa-lg"
  text="Street Kids Finances"
%}

# A Huge Thanks to Our Donors

<section id="stats" class="animate-this">
  <div class="row">
    <div class="col-twelve">
      <div class="block-1-2 block-tab-1-2 block-mob-full stats-list">
        <div class="bgrid stat">
          <div class="icon-part">
            <i class="fas fa-hand-holding-heart fa-lg"></i>
          </div>
          <h3 class="stat-count">28240</h3>
          <br>
          <p>In Donations (CHF/EUR)</p>
        </div>
        <div class="bgrid stat">
          <div class="icon-part">
            <i class="fas fa-child fa-lg"></i>
          </div>
          <h3 class="stat-count">12</h3>
          <br>
          <p>Donors (Clubs & Individuals)</p>
        </div>
      </div>
    </div>
  </div>
</section>

<br>

- Diamond Circle Foundation
- Rotary de Romans (D1780) [<a-out/>](https://rotaryromans.com)
- Rotary Neuchâtel Lac [<a-out/>](https://neuchatel-lac.rotary1990.ch/fr)
- Rotary Nyon-La Côte [<a-out/>](https://nyon-la-cote.rotary1990.ch/fr)
- Rotary Sion [<a-out/>](https://sion.rotary1990.ch/fr)
- Rotary Bern Christoffel [<a-out/>](https://bern-christoffel.rotary1990.ch/fr)
- Rotary Gstaad-Saanenland [<a-out/>](https://gstaad-saanenland.rotary1990.ch/fr)
- Rotary Les Rangiers [<a-out/>](https://les-rangiers.rotary1990.ch/fr)
- The 15+ Rotaracts of RID 1960 [<a-out/>](https://www.rotaract1960.org/clubes-rtc)
- Rotary Jorat [<a-out/>](https://jorat.rotary1990.ch/fr)
- Patrick Léon Favre
- Jean-François Richter
- Oliver Rosenbauer
- Marie-Renée Borburgh

# The Districts of Our Rotaractors & Rotarians
