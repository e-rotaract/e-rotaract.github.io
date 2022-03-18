---
layout: default
permalink: "/ctrl"
author: eclub

logo: "assets/images/rotaract-logo-white.png"
logo-center: true
pretitle: Join us, together we can
title: Make our world a better&nbsp;place!
description: We are e-Rotaract Beyond Frontiers,<br>And we are here to hear your idea, let's&nbsp;do&nbsp;it!

hide-menu: true
hide-home: false

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

<script>
  Date.prototype.getWeekNumber = function(){
    var d = new Date(Date.UTC(this.getFullYear(), this.getMonth(), this.getDate()));
    var dayNum = d.getUTCDay() || 7;
    d.setUTCDate(d.getUTCDate() + 4 - dayNum);
    var yearStart = new Date(Date.UTC(d.getUTCFullYear(), 0, 1));
    var w = Math.ceil((((d - yearStart) / 86400000) + 1)/7);
    if(this.getDay() == 0 | this.getDay() == 6) w = w + 1;
    return w;
  };
</script>

<ul class="showcase">
  <a onclick="document.location='https://www.timeanddate.com/calendar/custom.html?year='+new Date().getFullYear()+'&amp;country=5&amp;cols=0&amp;fdow=6&amp;wno=6&amp;wncs=2&amp;ctf=2&amp;wdf=1&amp;holmark=2&amp;hod=1&amp;hcl=1&amp;cdt=1&amp;ccg=1&amp;cci=6&amp;ccp=3&amp;ccu=10&amp;ccz=0&amp;cwd=2______2&amp;cwf=______&amp;holm=1&amp;doy=1&amp;dly=1&amp;hid=1&amp;typ=0&amp;display=3&amp;df=1'">
    <li>
      📆 <b id="yeardayspassed">_</b>&nbsp;<i class="fas fa-angle-right"></i>&nbsp;<b id="yeardaystogo">_</b>
      <br>
      📆 <script>document.write(new Date().getWeekNumber());</script><small>w</small>&nbsp;<i class="fas fa-angle-right"></i>&nbsp;<script>document.write(new Date(new Date().getFullYear(), 11, 30).getWeekNumber() - new Date().getWeekNumber());</script><small>w</small>
    </li>
  </a>
  <li>
    IΛCO 🌟 <b id="borndayspassed">_</b><br>
    IΛCO 🌟 <b id="bornweekspassed">_</b>
  </li>
</ul>
<ul class="showcase">
  <li>
    💪 <b id="gym">_</b><br>
    🌱 <b id="vegan">_</b><br>
    😴 <b id="sleepmaster">_</b>
  </li>
  <li>
    🐢 <b id="iaco2030">_</b><small> 2030</small><br>
    🌲 <b id="vivaci2100">_</b><small> 2100</small><br>
    🔮 <b id="iacovivaci3000">_</b><small> 3000</small>
  </li>
</ul>


<script>
  window.onload = function() {
    countUpFromTime(new Date().getFullYear()+"-01-01", 'yeardayspassed', "j", false);
    countUpFromTime(new Date().getFullYear()+"-12-30", 'yeardaystogo', "j", false);

    countUpFromTime("1994-02-01", 'borndayspassed', "j");
    countUpFromTime("1994-02-01", 'bornweekspassed', "w");

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

<hr>

<ul class="showcase" id="list"></ul>

<script>
  var links = [
    ["📨 My E-mails", "https://mail.ovh.net/roundcube/?_task=login", ""],
    ["🥕 iago-food-1w", "https://lite.framacalc.org/iago-food-1w", ""],
    ["🎨 Creator Studio", "https://business.facebook.com/creatorstudio", ""],
    ["💼 Business Suite", "https://business.facebook.com/latest/inbox/messenger", ""]
  ];
  for(l of links) {
    $("#list").append(
        "<a href='" + l[1] + "'>" +
          "<li>" +
            l[0] +
            (l[2] != "" ? "<br><small>" + l[2] + "</small>" : "") +
          "</li>" +
        "</a>");
  }
</script>

