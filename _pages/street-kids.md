---
layout: default
permalink: /street-kids
author: eclub
image: default-bg.jpg
logo:
  url: logo/rotaract-alpha.png
  position: center

pretitle: Help them smile again!
title: Street Kids
description: Meals, Shelter and Education for Kenyan Kids

show-home: true
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
      url: https://fb.com/Rotaract-Club-of-Eco-Warriors-106271138555346
      newtab: true
      title: RID 9212
      description: Kenya 🇰🇪
      image: flags/ke.png
    right:
      url: https://rotary1990.ch
      newtab: true
      title: RID 1990
      description: Switzerland 🇨🇭
      image: flags/ch.png
  - left:
      url: https://www.rotary1960.org
      newtab: true
      title: RID 1960
      description: Portugal 🇵🇹
      image: flags/pt.png
    right:
      url: https://e-rotaract.com
      newtab: false
      title: RID 1780
      description: France 🇫🇷
      image: flags/fr.png

links-footer:
  - icon: fas fa-hand-holding-heart
    name: Make a Donation
    url: "#donation"
    newtab: false

---

{% include img src="actions/street-kids/cover.png" %}

The Street Kids is a **continuous project for 11+ kids** from Nairobi, Kenya. We help them by providing **2 meals** a day, **shelter** & **education**.

We know each kid, and we keep regular contact with them all through weekly calls, sharing photos, messages, and more.

It is an international partnership among different clubs and Rotary International Districts, including clubs from [9212 (Kenya)](https://fb.com/Rotaract-Club-of-Eco-Warriors-106271138555346), [1990 (Switzerland)](https://rotary1990.ch), [1960 (Portugal)](https://www.rotary1960.org), and [1780 (France)](https://e-rotaract.com).

# Join Us every Sunday {#videocall}

We have weekly videocalls of 30 minutes, every Sunday:

- 12:00 - Kenya 🇰🇪 (UTC+3)
- 11:00 - Central Europe: CH🇨🇭, FR🇫🇷, NO🇳🇴...
- 10:00 - Western Europe: PT🇵🇹, UK🇬🇧...

{% include btn
  url="/street-kids/call"
  newtab=true
  class="button-primary"
  icon="fa fa-video fa-lg"
  text="Street Kids Videocall"
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

- Account holder: District Rotary 1990, Comission Rotaract
- IBAN:

<input id="iban" value="CH30 8080 8003 8478 5531 6" type="text" style="position: fixed; bottom: 0; right: 0; opacity: 0; transform: scale(0);" />
<a onclick="copyEvent('iban')" class="button">
  <i class="fa fa-copy fa-lg"></i> Copy IBAN
</a>
<script>
  document.write(document.getElementById('iban').value)
</script>

<script>
function copyEvent(id) {
  $("#"+id).select();
  document.execCommand("copy");
}
</script>

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

- Rotary Jorat [<a-out/>](https://jorat.rotary1990.ch/fr)
- Rotary de Romans [<a-out/>](https://rotaryromans.com)
- Rotary Neuchâtel Lac [<a-out/>](https://neuchatel-lac.rotary1990.ch/fr)
- Rotary Nyon-La Côte [<a-out/>](https://nyon-la-cote.rotary1990.ch/fr)
- Rotary Sion [<a-out/>](https://sion.rotary1990.ch/fr)
- Rotary Bern Christoffel [<a-out/>](https://bern-christoffel.rotary1990.ch/fr)
- Rotary Gstaad-Saanenland [<a-out/>](https://gstaad-saanenland.rotary1990.ch/fr)
- Rotary Les Rangiers [<a-out/>](https://les-rangiers.rotary1990.ch/fr)
- The 15+ Rotaract Clubs of RID 1960 [<a-out/>](https://www.rotaract1960.org/clubes-rtc)
- Patrick Léon Favre
- Jean-François Richter
- Oliver Rosenbauer
- Marie-Renée Borburgh

# The Districts of Our Rotaractors & Rotarians
