---
layout: default
permalink: "/"
author: eclub

logo:
  url: "assets/images/rotaract-logo-white.png"
  position: "center"

pretitle: Hi, welcome to
title: e-Rotaract Beyond Frontiers
description: Together we can make our world a better place!

site-links: true     # show the default site menu
links:
    - name: "Join us!"
      icon: "fa fa-hands-helping"
      url: "#join"
      newtab: false
      show-in-intro: true
      show-in-menu: true
    - name: "Our actions" 
      icon: "fa fa-hand-holding-heart"
      url: "#actions"
      newtab: false
      show-in-intro: true
      show-in-menu: true
    - name: "Our volunteers"
      icon: "fa fa-seedling"
      url: "#volunteers"
      newtab: false
      show-in-intro: true
      show-in-menu: true

morelinks:
  - left:
      url: "/speakeat"
      newtab: true
      cta: "Come to our SpeakEat"
      title: "A moment to share knowledge and experiences!"
      image: "/assets/images/speakeat-logo-only.jpg"
    right:
      url: "/street-kids"
      newtab: true
      cta: "Street Kids Project"
      title: "Let's help kids from Kenya"
      image: "/assets/images/street-kids/cover.png"
  - left:
      url: "/human-movie"
      newtab: false
      cta: "Human Movie"
      title: "Watch with us!"
      image: "/assets/images/human-movie.png"
    right:
      url: "/instagram"
      newtab: true
      cta: "Follow us"
      title: "Get to know us on Instagram!"
      image: "/assets/images/instagram-logo.jpg"
#    right:
#      url: "#social"
#      newtab: false
#      cta: "We are Rotaract"
#      title: "Join us today!"
#      image: "/assets/images/rotaract-logo-pink.png"

footer:
  - icon: "<i class='fab fa-instagram'></i>"
    text: "rotaract_eclub"
    url: "https://instagram.com/rotaract_eclub"
    newtab: true

---

We are an international group of friends sharing one goal: do our best to help the world, because together we can make it a better place.

Our e-club is part of the global network of volunteers in Rotary International, and everyone is welcome to join our virtual meetings!



# Can I join? {#join}

![]({{site.baseurl}}/assets/images/friends-toast.jpg)

Everyone is welcome! We have monthly meetings on **Sundays**.

You can help as a volunteer in social actions when you have the time, and if interested you can become a member of our e-club!

Members also help in social projects, as well as develop their professional and personal skills in our e-club.

To know more you can contact us!

<p style="text-align: center;">
  <a href="/instagram" target="_blank" class="button button-primary">
    <i class="fab fa-instagram fa-lg"></i> Follow us and<br> send a message @rotaract_eclub
  </a>
</p>
<p style="text-align: center;">
  <a href="mailto:hi@e-rotaract.com" target="_blank" class="button">
    <i class="fa fa-envelope fa-lg"></i> E-mail us: hi@e-rotaract.com
  </a>
</p>



# What do we do? {#actions}

We work on a variety of social projects and causes! When an action is beneficial to all concerned, we will support and help as much we can!

If you have an idea, send us a message, we can surely work together!

<p style="text-align: center;">
  <a href="#join" class="button">
    <i class="fa fa-lightbulb fa-lg"></i> Tell us your idea!
  </a>
</p>

Some of the actions we worked and helped on are:

<script>
  var actions = [
    { url: "/street-kids", img: "/assets/images/actions/street-kids.png" },
    { url: "/speakeat", img: "/assets/images/actions/speakeat.png" },
    { url: "/human-movie", img: "/assets/images/actions/human-movie.png" }
  ];

  shuffle(actions)

  for (it in actions) {
    document.write('<a target="_blank" href="' + actions[it].url  + '">' +
      '<img class="half" src="' + actions[it].img + '">' +
      '</a>'
      )
  }
</script>



# Who are we? {#volunteers}

![]({{site.baseurl}}/assets/images/hands-heart.jpg)

Our past and current volunteers are from all around the world, from different countries and Rotary International Discricts, including:
Brasil 🇧🇷 (<a target="_blank" href="https://www.rotary4700.org.br/home">4700</a>),
France 🇫🇷 (<a target="_blank" href="https://rotary1710.org">1710</a>, <a target="_blank" href="https://www.rotary1730.org">1730</a>, <a target="_blank" href="https://www.rotary1780.org">1780</a>),
and Norge 🇳🇴 (<a target="_blank" href="https://d2310.rotary.no">2310</a>).
Come and join us!

<script>
  var participants = [
    { img: "/assets/images/participants/alex.png" },
    { img: "/assets/images/participants/debora.png" },
    { img: "/assets/images/participants/emiline.png" },
    { img: "/assets/images/participants/iaco.png" },
    { img: "/assets/images/participants/leo.png" },
    { img: "/assets/images/participants/magali.png" }
  ];

  shuffle(participants)

  for (it in participants) {
    document.write('<img class="half2" src="' + participants[it].img + '">')
  }

  document.write('<a href="#join"><img class="half2" src="/assets/images/participants/you.gif"></a>')
</script>
