---
layout: default
permalink: /
# featured: true
# hidden: true

author: eclub
image: default-bg.jpg
logo:
  url: logo/rotaract.svg
  position: center
  width: 300px

pretitle: Hi, welcome to
title: e-Rotaract Beyond Frontiers
description: Together we can make our world a better place!

# categories: [ a, b ]
# tags: [ c, d, e ]

show-home: true
links-side: true

links-home:
    - name: Join us!
      icon: fas fa-hands-helping
      url: "#join"
      newtab: false
      show-home: true
      show-side: true
    - name: Our actions
      icon: fas fa-hand-holding-heart
      url: "#actions"
      newtab: false
      show-home: true
      show-side: true
    - name: Our volunteers
      icon: fas fa-seedling
      url: "#volunteers"
      newtab: false
      show-home: true
      show-side: true

links-gallery:
  - left:
      url: /speakeat
      newtab: true
      title: COME TO OUR SPEAKEAT
      description: A moment to share knowledge and experiences!
      image: speakeat-logo-only.jpg
    right:
      url: /street-kids
      newtab: true
      title: STREET KIDS PROJECT
      description: Let's help kids from Kenya
      image: actions/street-kids/cover.png
  - left:
      url: /human-movie
      newtab: false
      title: HUMAN MOVIE
      description: Watch with us!
      image: human-movie.png
    right:
      url: /instagram
      newtab: true
      title: FOLLOW US
      description: Get to know us on Instagram!
      image: instagram-logo.jpg

links-footer:
  - icon: fab fa-instagram
    name: rotaract_eclub
    url: /instagram
    newtab: true

show-corner: true

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

# What do we do? {#actions}

We work on a variety of social projects and causes! When an action is beneficial to all concerned, we will support and help as much we can!

If you have an idea, send us a message, we can surely work together!

{% include btn url="#join" icon="fa fa-lightbulb fa-lg" text="Tell us your idea!" %}

Some of the actions we worked and helped on are:

{% include gallery
  shuffle_pre=true
  shuffle=true
  grid=2
  pre='[
    { url: "#join", img: "actions/awareness.png", newtab: false },
    { url: "#join", img: "actions/online-crime.png", newtab: false },
    { url: "#join", img: "actions/meeting-people.png", newtab: false },
    { url: "/street-kids", img: "actions/street-kids.png", newtab: true }
  ]'
  items='[
    { url: "/bone-marrow", img: "actions/bone-marrow-donation.png", newtab: false },
    { url: "/speakeat", img: "actions/speakeat.png", newtab: true },
    { url: "/human-movie", img: "actions/human-movie.png", newtab: true }
  ]'
%}

# Who are we? {#volunteers}

{% include img src="hands-heart.jpg" %}

Our past and current volunteers are from all around the world, from different countries and Rotary International Discricts, including:
Brasil 🇧🇷 ([4700](https://www.rotary4700.org.br/home)),
France 🇫🇷 ([1710](https://rotary1710.org), [1730](https://www.rotary1730.org), [1780](https://www.rotary1780.org)),
and Norge 🇳🇴 ([2310](https://d2310.rotary.no)).
Join us!

{% include gallery
  shuffle=true
  grid=4
  items='[
    { img: "participants/alex.png" },
    { img: "participants/debora.png" },
    { img: "participants/emiline.png" },
    { img: "participants/iaco.png" },
    { img: "participants/leo.png" },
    { img: "participants/magali.png" }
  ]'
  post='[ { url: "#join", img: "participants/you.gif" } ]'
%}
