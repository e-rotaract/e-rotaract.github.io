---
layout: default
permalink: /be-member
# featured: true
# hidden: true

author: eclub
image: default-bg.jpg
logo:
  url: logo/rotaract.svg
  position: center
  width: 300px

pretitle: Here you can
title: Become a Member!
description: We are happy to hear you are interested, let's start!

# categories: [ a, b ]
# tags: [ c, d, e ]

show-home: true
links-side: true

links-home:
    - name: How to become a Member?
      icon: fab fa-slideshare
      url: "#q1"
      newtab: false
      show-home: true
      show-side: true

links-gallery:
  - left:
      url: /
      newtab: false
      title: DO YOU FOLLOW THE E-CLUB ALREADY?
      description: Click here to check our page!
      image: instagram-logo.jpg
    right:
      url: /instagram
      newtab: true
      title: CLICK HERE TO REQUEST MEMBERSHIP
      description: We will get in touch with you soon ;)
      image: logo/rotaract-pink.png

links-footer:
  - icon: fab fa-instagram
    name: rotaract_eclub
    url: /instagram
    newtab: true

show-corner: true

show-notif: false

---

# Question 1 {#q1}

{% include gallery
  items='[
    { img: "be-member/q1.png", grid: 2 },
    { url: "#q2", img: "be-member/yes.gif", grid: 4, newtab: false },
    { img: "be-member/no.gif", grid: 4 }
  ]'
%}

<br><br><br>

# Question 2 {#q2}

{% include gallery
  items='[
    { img: "be-member/q2.png", grid: 2 },
    { url: "#q3", img: "be-member/yes.gif", grid: 4, newtab: false },
    { img: "be-member/no.gif", grid: 4 }
  ]'
%}

<br><br><br>

# Question 3 {#q3}

{% include gallery
  items='[
    { img: "be-member/q3.png", grid: 2 },
    { url: "#q4", img: "be-member/yes.gif", grid: 4, newtab: false },
    { img: "be-member/no.gif", grid: 4 }
  ]'
%}

<br><br><br>

# Question 4 {#q4}

{% include gallery
  items='[
    { img: "be-member/q4.png", grid: 2 },
    { url: "#q4", img: "be-member/yes.gif", grid: 4, newtab: false },
    { img: "be-member/no.gif", grid: 4 }
  ]'
%}