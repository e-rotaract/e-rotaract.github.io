---
layout: default
permalink: "/ctrl"
author: eclub

logo: "assets/images/rotaract-logo-white.png"
logo-center: true
pretitle: Join us, together we can
title: Make our world a better&nbsp;place!
description: We are e-Rotaract Beyond Frontiers,<br>And we are here to hear your idea, let's&nbsp;do&nbsp;it!

site-links: true     # show the default site menu
links:
    - name: "Join us!"
      icon: "fa fa-hands-helping"
      url: "#join"
      newtab: false
      show-in-intro: true
      show-in-menu: true
    - name: "Let's be social"
      icon: "fa fa-user-friends"
      url: "#social"
      newtab: false
      show-in-intro: true
      show-in-menu: true
    - name: "Propose partnership"
      icon: "fa fa-hand-holding-heart"
      url: "#partnership"
      newtab: false
      show-in-intro: true
      show-in-menu: true

morelinks:
  - left:
      url: "https://e-rotaract.com/speakeat"
      newtab: false
      cta: "Come to our SpeakEat"
      title: "A moment to share knowledge and experiences!"
      image: "assets/images/speakeat-logo-only.jpg"
    right:
      url: "#social"
      newtab: false
      cta: "We are Rotaract"
      title: "Join us today!"
      image: "assets/images/rotaract-logo-pink.png"
---

We are an international group of friends, and we share one goal: do our best to help the world, because we believe together we can go further.

Our club is part of the global network of volunteering associations from Rotary International, and everyone is more than welcome to join.



# Let's connect! {#social}

![]({{site.baseurl}}/assets/images/friends-camping.jpg "Let's connect!")

Let's be social, find us online and connect with us!
And of course, we would love to hear you, so feel free to send us a message!

<ul class="ll">
  <li>
    💪 <span id="gym">_</span><br>
    🌱 <span id="vegan">_</span><br>
    😴 <span id="sleepmaster">_</span>
  </li>
  <li>
    🐢 <span id="iaco2030">_</span><small> 2030</small><br>
    🌲 <span id="vivaci2100">_</span><small> 2100</small><br>
    🔮 <span id="iacovivaci3000">_</span><small> 3000</small>
  </li>
</ul>


<script>
  window.onload = function() {
    //countUpFromTime(new Date().getFullYear()+"-01-01", 'yeardayspassed', "j", false);
    //countUpFromTime(new Date().getFullYear()+"-12-30", 'yeardaystogo', "j", false);

    //countUpFromTime("1994-02-01", 'borndayspassed', "j");
    //countUpFromTime("1994-02-01", 'bornweekspassed', "w");

    //countUpFromTime("2018-06-28", 'gym', "j", true);
    countUpFromTime("2022-03-01", 'gym', "j", true);
    countUpFromTime("2019-02-28", 'vegan', "j", true);
    countUpFromTime("2022-02-03", 'sleepmaster', "j", true);

    countUpFromTime("2100-01-01", 'vivaci2100', "w", false);
    countUpFromTime("2030-01-01", 'iaco2030', "w", false);
    countUpFromTime("3000-01-01", 'iacovivaci3000', "w", false);
  }

  function countUpFromTime(countFrom, id, type, date) {
    txtdate = countFrom;
    countFrom = new Date(countFrom).getTime();
    var now = new Date(),
        countFrom = new Date(countFrom),
        timeDifference = (now - countFrom);

    var secondsInADay = 60 * 60 * 1000 * 24,
        secondsInAHour = 60 * 60 * 1000;

    days = Math.floor(timeDifference / (secondsInADay) * 1);
    hours = Math.floor((timeDifference % (secondsInADay)) / (secondsInAHour) * 1);
    mins = Math.floor(((timeDifference % (secondsInADay)) % (secondsInAHour)) / (60 * 1000) * 1);
    secs = Math.floor((((timeDifference % (secondsInADay)) % (secondsInAHour)) % (60 * 1000)) / 1000 * 1);

    weeks = Math.floor(days / 7);

    if(type == "j")  txtVar = Math.abs(days) + 1;
    if(type == "w") txtVar = Math.abs(weeks)

    document.getElementById(id).innerHTML = txtVar + "<small>" + type + (date ? " " + txtdate.replaceAll("-", "&#x2011;") : "") + "</small>";
  }
</script>


<ul class="ll">
  <a href="https://iago.me">
    <li>
    asdfsadf asdkfsa  jksad fkjsad <br>po
    </li>
  </a>
    <a href="https://e-rotaract.me">
    <li>
    eclub eclub eclub eclub eclub eclub eclub eclub eclub eclub eclub eclub eclub <br>po
    </li>
  </a>
</ul>

<p style="text-align: center;">
  <a href="https://instagram.com/rotaract_eclub" target="_blank" class="button button-primary">
    <i class="fab fa-instagram fa-lg"></i> Follow us and<br> send a message @rotaract_eclub
  </a>
  <a href="mailto:hi@e-rotaract.com" target="_blank" class="button">
    <i class="fa fa-envelope fa-lg"></i> E-mail us<br>a
  </a>
  <!-- <a href="https://chat.whatsapp.com/INkMh1VrXbr3H77piY4Lrh" target="_blank" class="button button-success">
    <i class="fab fa-whatsapp fa-lg"></i> Join our WhatsApp
  </a> -->
</p>



# Let's make a partnership! {#partnership}

![]({{site.baseurl}}/assets/images/friends-toast.jpg "Let's make a partnership!")

We work on a variety of projects and causes!
<br>
If you have an idea, we can work together: send us a message, we are here to help make our world a better place for everyone.

<p style="text-align: center;">
  <a href="#social" class="button smoothscroll">
    <i class="fa fa-lightbulb fa-lg"></i> Tell us your idea!
  </a>
</p>



# Come and join us! {#join}

![]({{site.baseurl}}/assets/images/hands-heart.jpg "Join us!")

You and your friends are more than welcome!
<br>
We meet online at least once per month, and we can also meet face-to-face if our members live close by!
<br>
If you are interested in joining us, the best is to send us a message:

<p style="text-align: center;">
  <a href="#social" class="button smoothscroll">
    <i class="fa fa-user-friends fa-lg"></i> Send us a message!
  </a>
</p>
