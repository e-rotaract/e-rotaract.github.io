---
layout: default
permalink: /speakeat
# featured: true
# hidden: true

author: eclub
# image: default-bg.jpg
# logo:
#   url: logo/rotaract.svg
#   position: center
#   width: 300px

pretitle: Hi, welcome to
title: SpeakEat Rotaract
description: A moment to exchange knowledge and experiences, promoting understanding and peace!

# categories: [ a, b ]
# tags: [ c, d, e ]

# show-logo: true
# show-home: false
# links-side: false

links-home:
    - name: Join Videocall
      icon: fas fa-video
      url: "#join"
      newtab: false
      show-home: true
      show-side: false
    - name: Next SpeakEat
      icon: fas fa-calendar-alt
      url: "https://www.facebook.com/rotaract.eclub.bf/events"
      newtab: true
      show-home: true
      show-side: false
    - name: Instagram
      icon: fab fa-instagram
      url: "https://instagram.com/speak.eat"
      newtab: true
      show-home: true
      show-side: false

# show-main: true

links-gallery:
  - left:
      name: FOLLOW SPEAKEAT<br>Get to know us on Instagram!
      image: instagram-logo.jpg
      url: https://instagram.com/speak.eat
      newtab: true
    right:
      name: E-ROTARACT BEYOND FRONTIERS<br>Join our e-Club today!
      image: default-bg.jpg
      url: /
      newtab: true

links-footer:
  - name: rotaract_eclub
    icon: fab fa-instagram
    url: /instagram
    newtab: true

# show-corner: true
show-notif: false

---

<script>
  var list_events = [
    {num: "01", sym: "🏳️‍🌈", date: "2020-12-13", title: "LGBT+"},
    {num: "02", sym: "👥", date: "2021-01-03", title: "Discrimination"},
    {num: "03", sym: "🧠", date: "2021-01-31", title: "Cognitive Bias (Biais Cognitif)"},
    {num: "04", sym: "❤️", date: "2021-02-14", title: "Self-Love"},
    {num: "05", sym: "💼", date: "2021-03-21", title: "Wellbeing at Work"},
    {num: "06", sym: "🌐", date: "2021-04-25", title: "Climate Change"},
    {num: "07", sym: "⛱️", date: "2021-07-04", title: "Summer Body"},
    {num: "08", sym: "😲", date: "2021-09-26", title: "Taboos at Work (Les Tabous au Travail) - <span style='font-size: small !important;'>with DJML</span>"},
    {num: "09", sym: "⚙️", date: "2021-11-06", title: "How to integrate differences and plurality in our Rotary Family? - <span style='font-size: small !important;'>with Uni Rotary D1990</span>"}, // https://rotary1990.ch/en/agenda/show/134393
    {num: "10", sym: "🗝️", date: "2021-11-21", title: "How to live the end of life?"},
    {num: "11", sym: "💗", date: "2021-12-05", title: "Relationships"},
    {num: "12", sym: "🤔", date: "2022-01-16", title: "How to make choices in life? - <span style='font-size: small !important;'>with DJML</span>"},
    {num: "13", sym: "🍸", date: "2023-01-15", title: "Alcohol - <span style='font-size: small !important;'>with DJML</span>"},
    {num: "14", sym: "❔", date: "2030-12-31", title: "(coming soon)"}
  ];
  const options = { weekday: 'long', month: 'long', day: 'numeric' };
  for(let i = 0; i < list_events.length; i++) {
    if(new Date(list_events[i].date) > new Date() && new Date(list_events[i].date).getYear() <= (new Date().getYear()+1)) {
      var current_event = new Date(list_events[i].date)
      break;
    }
  }
</script>

# Join Us Online {#join}

- 10:00 • UTC−3 (🇧🇷)
- 13:00 • UTC&ensp;0 (🇵🇹🇬🇧)
- 14:00 • UTC+1 (🇨🇭🇫🇷🇲🇦🇳🇴)
- 21:00 • UTC+8 (🇹🇼)

{% include btn
  url="/videocall"
  newtab=true
  class="button-primary"
  icon="fa fa-video fa-lg"
  text="SpeakEat Videocall<br><script>document.write(current_event == null ? 'Sunday • Dimanche • Domingo' : current_event.toLocaleDateString('en-UK', options))</script>"
%}

{% include btn
  url="https://www.facebook.com/rotaract.eclub.bf/events"
  newtab=true
  class="button"
  icon="fas fa-calendar-alt fa-lg"
  text="Next SpeakEat Event<br>(add to your <i class='fab fa-facebook'></i> calendar)"
%}

{% include btn
  url="/"
  newtab=false
  class="button-success"
  icon="fa fa-hand-holding-heart fa-lg"
  text="Join Our e-Club Today!"
%}

{% include img src="actions/speakeat.png" %}

# SpeakEat

{% include btn
  url="https://instagram.com/speak.eat"
  newtab=true
  class="button"
  icon="fab fa-instagram fa-lg"
  text="Check Our Instagram"
%}

- [What is SpeakEat?](#en)
- [Qu'est-ce le SpeakEat ?](#fr)
- [O que é SpeakEat?](#pt)

## List of SpeakEat's

<ol>
  <script>
    for(let i = 0; i < list_events.length; i++) {
        document.write(
          "<li>" +
          "<a target='_blank' href='https://www.facebook.com/rotaract.eclub.bf/events'>" +
          list_events[i].sym + " " + list_events[i].title +
          "</a> <span style='font-size: small;'>(" +
          list_events[i].date +
          ")<span></li>"
        );
        if(new Date(list_events[i].date) > new Date()) {
            break;
        }
    }
  </script>
</ol>

## Hello! {#en}

❇️ Welcome to SpeakEat, a Rotaract project aiming to promote the exchange of knowledge and experiences!

👥 We will have a time together, to get to know each other and exchange around the main topic.

🍓 If you would like to eat a plant-based snack, you can share your recipe with us when you present yourself.

—

💬 The aim of SpeakEat is to encourage conversation about important topics, with respect and goodwill!

🌍 It is inspired by the Rotary International cause of promoting peace to foster mutual understanding.

😋 It's a conversation similar to Free IC/Vegan Party, but by videocall and with a plant-based snack.

🏳️ We start with the main topic, and the participants decide how we will move the conversation forward.

—

🌐 Share the events with your friends and family! Everyone is welcome!

⁉️ If you have any questions or suggestions, please contact us at [e-rotaract.com](/)

## Salut ! {#fr}

❇️ Bienvenue au SpeakEat, un projet Rotaract visant à promouvoir l'échange de connaissances et d'expériences !

👥 Nous aurons un moment ensemble, pour apprendre à nous connaître et échanger autour du thème principal.

🍓 Si vous voulez manger un petit goûter plant-based, vous pouvez partager votre recette avec nous tous lorsque vous vous présenterez.

—

💬 Le but de SpeakEat est d'encourager la conversation sur des sujets importants, dans le respect et la bienveillance !

🌍 L'action s'inspire de l'axe du Rotary International de promotion de la paix pour favoriser la compréhension mutuelle.

😋 C'est une conversation similaire à Free IC/Vegan Party, mais en visio et avec un petit repas plant-based.

🏳️ Nous démarrons par le thème principal, et les participants décident comment nous allons faire avancer la conversation.

—

🌐 Partagez l'événement à vos proches ! Toustes sont les bienvenu·e·s !

⁉️ Si vous avez des questions ou suggestions, contactez nous sur [e-rotaract.com](/)

## Olá! {#pt}

❇️ Bem-vinde ao SpeakEat, projeto do Rotaract que visa promover a troca de conhecimentos e experiências!

👥 Nós teremos um momento juntos, para nos conhecer e conversar sobre o tema principal.

🍓 Se você quiser comer um lanche plant-based, você pode compartilhar sua receita conosco quando se apresentar.

—

💬 O objetivo do SpeakEat é incentivar a conversa sobre temas importantes, com respeito e boa vontade!

🌍 Ele é inspirado na causa do Rotary International de promover a paz para fomentar a compreensão mútua.

😋 É uma conversa semelhante ao Free IC/Vegan Party, mas em videochamada e com um lanche plant-based.

🏳️ Começamos com o tema principal, e os participantes decidem como vamos avançar a conversa.

—

🌐 Compartilhe o evento com seus amigos e familiares! Todes são bem-vindes!

⁉️ Se você tiver alguma dúvida ou sugestão, pode entrar em contato conosco em [e-rotaract.com](/)
