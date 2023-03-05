---
layout: default
permalink: /
# featured: true
# hidden: true

author: eclub
# image: default-bg.jpg
# logo:
#   url: logo/rotaract.svg
#   position: center
#   width: 300px

pretitle: Hi, welcome to
title: e-Rotaract Beyond Frontiers
description: Together we can make our world a better place!

# categories: [ a, b ]
# tags: [ c, d, e ]

# show-logo: true
# show-home: false
# links-side: false

links-home:
    - name: Join us!
      icon: fas fa-hands-helping
      url: "#join"
      newtab: false
      show-home: true
      show-side: false
    - name: Our actions
      icon: fas fa-hand-holding-heart
      url: "#actions"
      newtab: false
      show-home: true
      show-side: false
    - name: Our volunteers
      icon: fas fa-seedling
      url: "#volunteers"
      newtab: false
      show-home: true
      show-side: false

# show-main: true

links-gallery:
  - left:
      name: FOLLOW US<br>Get to know us on Instagram!
      image: instagram-logo.jpg
      url: /instagram
      newtab: true
    right:
      name: STREET KIDS PROJECT<br>Let's help kids from Kenya
      image: actions/street-kids/cover.png
      url: /street-kids
      newtab: true

links-footer:
  - name: rotaract_eclub
    icon: fab fa-instagram
    url: /instagram
    newtab: true

# show-corner: true
show-notif: false

---

We are an international group of friends sharing one goal: do our best to help the world, because together we can make it a better place.

Our e-club is part of the global network of volunteers in Rotary International, and everyone is welcome to join our virtual meetings!

# Can I join? {#join}

{% include img src="friends-toast.jpg" %}

Everyone is welcome! We have monthly meetings on **Sundays**.

You can help as a volunteer in social actions when you have the time, and if interested you can become a member of our e-club!

Members also help in social projects, as well as develop their professional and personal skills in our e-club.

To know more you can contact us!

{% include btn
  url="/instagram"
  newtab=true
  class="button-primary"
  icon="fab fa-instagram fa-lg"
  text="Follow us and<br>send a message @rotaract_eclub"
%}

{% include btn
  url="mailto:hi@e-rotaract.com"
  icon="fa fa-envelope fa-lg"
  text="E-mail us: hi@e-rotaract.com"
%}

{% include btn
  url="/join-us"
  newtab=true
  class="button-success"
  icon="fas fa-file-signature fa-lg"
  text="Interested to join as member?<br>Click here to check how to apply!"
%}

# What do we do? {#actions}

We work on a variety of social projects and causes! When an action is beneficial to all concerned, we will support and help as much we can!

If you have an idea, send us a message, we can surely work together!

{% include btn url="#join" icon="fa fa-lightbulb fa-lg" text="Tell us your idea!" %}

Some of the actions we worked and helped on are:

{% include gallery
  shuffle=true
  shuffle_post=true
  grid=2
  items='[
    { url: "/instagram", img: "actions/awareness.png", newtab: true },
    { url: "/safe-web", img: "actions/safe-web.png" },
    { url: "/meeting-volunteers", img: "actions/meeting-people.png" },
    { url: "/street-kids", img: "actions/street-kids.png", newtab: true }
  ]'
  post='[
    { url: "https://www.worldcleanupday.org", img: "actions/world-clean-up-day.png" },
    { url: "/bone-marrow", img: "actions/bone-marrow-donation.png" },
    { url: "/speakeat", img: "actions/speakeat.png", newtab: true },
    { url: "/human-movie", img: "actions/human-movie.png", newtab: true }
  ]'
%}

# Who are we? {#volunteers}

{% include img src="hands-heart.jpg" %}

Our past and current volunteers are from all around the world, located in different countries and Rotary International Discricts, including:
Brasil 🇧🇷 ([4700](https://www.rotary4700.org.br/home)),
France 🇫🇷 ([1710](https://rotary1710.org), [1730](https://www.rotary1730.org), [1780](https://www.rotary1780.org)),
Maroc 🇲🇦 ([9010](https://rotary-d9010.org)),
Norge 🇳🇴 ([2310](https://d2310.rotary.no)),
and Taiwan 🇹🇼 ([3481](https://www.rid3481.org)).
Join us!

{% include gallery
  shuffle_pre=true
  grid=4
  pre='[
    { img: "participants/alex.png" },
    { img: "participants/debora.png" },
    { img: "participants/emiline.png" },
    { img: "participants/iaco.png" },
    { img: "participants/leo.png" }
  ]'
  items='[ { img: "participants/magali.png" } ]'
  post='[ { url: "#join", img: "participants/you.gif" } ]'
%}
