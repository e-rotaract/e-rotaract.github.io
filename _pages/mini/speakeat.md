---
layout: blank
title: SpeakEat Rotaract
permalink: /speakeat
---

<html>

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>SpeakEat</title>
    <link rel="stylesheet" href="{{ site.baseurl }}/assets/css/mini.css">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" integrity="sha384-oS3vJWv+0UjzBfQzYUhtDYW+Pj2yciDJxpsK1OYPAYjqT085Qq/1cq5FLXAZQ7Ay" crossorigin="anonymous">
    
    <script>
        var list_events = [
            {num: "01", sym: "🏳️‍🌈", date: "2020-12-13", title: "LGBT+"},
            {num: "02", sym: "👥", date: "2021-01-03", title: "Discrimination"},
            {num: "03", sym: "🧠", date: "2021-01-31", title: "Cognitive Bias (Biais Cognitif)"},
            {num: "04", sym: "❤️", date: "2021-02-14", title: "Self-Love"},
            {num: "05", sym: "💼", date: "2021-03-21", title: "Wellbeing at Work"},
            {num: "06", sym: "🌐", date: "2021-04-25", title: "Climate Change"},
            {num: "07", sym: "⛱️", date: "2021-07-04", title: "Summer Body"},
            {num: "08", sym: "😲", date: "2021-09-26", title: "Taboos at Work (Les Tabous au Travail) - with DJML"},
            {num: "09", sym: "⚙️", date: "2021-11-06", title: "How to integrate differences and plurality in our Rotary Family? - with <a target='_blank' href='https://rotary1990.ch/en/agenda/show/134393'>Uni Rotary D1990</a>"},
            {num: "10", sym: "🗝️", date: "2021-11-21", title: "How to live the end of life?"},
            {num: "11", sym: "💗", date: "2021-12-05", title: "Relationships"},
            {num: "12", sym: "🤔", date: "2022-01-16", title: "How to make choices in life? - with DJML"},
            {num: "13", sym: "🍸", date: "2023-01-15", title: "Alcohol"}
            //{num: "14", sym: "", date: "2030-12-31", title: "(coming soon, stay tuned)"}
        ];
        
        var next_event = list_events[list_events.length-1];
        for(var i = 0; i < list_events.length; i++){
       	    if(new Date(list_events[i].date) > new Date()) {
                next_event = list_events[i];
                break;
            }
        }
        
        var next_d = next_event.date.split("-")[2];
        var next_m = next_event.date.split("-")[1];
        var next_y = next_event.date.split("-")[0];
        
        var start = {y: next_y,  m: next_m,  d: next_d,  h: "17", min: "00"};
        var end =   {y: start.y, m: start.m, d: start.d, h: "19", min: start.min};
        var title = "SpeakEat Rotaract - " + next_event.title;
        var link = "https://tinyurl.com/speakeat"
        
        var description = "Details and videocall link: " + link;

        var titleEncoded = escape(title);
        var linkEncoded = escape(link);
        var descriptionEncoded = escape(description);

        var dateStartGoogle = start.y + start.m + start.d + "T" + start.h + start.min;
        var dateEndGoogle = end.y + end.m + end.d + "T" + end.h + end.min;
        var urlGoogle = "https://calendar.google.com/calendar/render?action=TEMPLATE&dates=" + dateStartGoogle + "00Z%2F" + dateEndGoogle + "00Z&details=" + descriptionEncoded + "&text=" + titleEncoded;

        var dateStartOutlook = start.y + "-" + start.m + "-" + start.d + "T" + start.h + "%3A" + start.min;
        var dateEndOutlook = end.y + "-" + end.m + "-" + end.d + "T" + end.h + "%3A" + end.min;
        var urlOutlook = "https://outlook.live.com/calendar/0/deeplink/compose?body=" + descriptionEncoded + "&enddt=" + dateEndOutlook + "%3A00%2B00%3A00&path=%2Fcalendar%2Faction%2Fcompose&rru=addevent&startdt=" + dateStartOutlook + "%3A00%2B00%3A00&subject=" + titleEncoded;

        var urlOffice = "https://outlook.office.com/calendar/0/deeplink/compose?body=" + descriptionEncoded + "&enddt=" + dateEndOutlook + "%3A00%2B00%3A00&path=%2Fcalendar%2Faction%2Fcompose&rru=addevent&startdt=" + dateStartOutlook + "%3A00%2B00%3A00&subject=" + titleEncoded;

        var icsFile = "BEGIN:VCALENDAR\nVERSION:2.0\nPRODID:-//www.iaco.io//SpeakEat Rotaract\nBEGIN:VEVENT\nUID:" + dateStartGoogle + "hi@iaco.io\nDTSTAMP:" + dateStartGoogle + "00Z\n" + /*ATTENDEE;CN=My Self ;RSVP=TRUE:MAILTO:me@gmail.com\nORGANIZER;CN=Me:MAILTO:me@gmail.com\n*/ "DTSTART:" + dateStartGoogle +"00Z\nDTEND:" + dateEndGoogle +"00Z\nSUMMARY:" + title + "\nURL:" + link + "\nDESCRIPTION:" + description + "\nTRANSP:OPAQUE\nX-MICROSOFT-CDO-BUSYSTATUS:BUSY\nBEGIN:VALARM\nACTION:DISPLAY\nDESCRIPTION:" + title + "\nTRIGGER:-PT1H\nEND:VALARM\nEND:VEVENT\nEND:VCALENDAR";
    </script>
</head>


<body class="en">
    <div class="author-photo">
        <a class="js-scroll-trigger" href="https://instagram.com/speak.eat">
            <img src="{{ site.baseurl }}/assets/images/speakeat-logo.png">
            <br>
            @speak.eat
            <br>
            SpeakEat Rotaract
            <br>
        </a>
    </div>

    <br>

    <ul>
        <li class="i-s shake">
            <a href="https://univ-grenoble-alpes-fr.zoom.us/j/91040901669?pwd=UHNKVkNUMDl3VkFhU3FwRHQ0U1ZRZz09"><!--https://meet.google.com/vue-vhfn-tec-->
                <div class='logo'>
                    <i class='fas fa-laptop fa-2x'></i>
                </div>
                <p class='title'>
                    Videocall · Visio
                    <span>Sunday · Dimanche · Domingo</span>
                    <span>18:30 UTC+1 (Central EU 🇪🇺)</span>
                    <span>14:30 UTC&minus;3 (BR 🇧🇷)</span>
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <a href="https://instagram.com/speak.eat">
                <div class='logo'>
                    <i class='fab fa-instagram fa-2x'></i>
                </div>
                <p class='title'>
                    Instagram
                    <span>
                        @speak.eat
                    </span>
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <a href="https://www.facebook.com/speak.eat.page/events">
                <div class='logo'>
                    <i class='fab fa-facebook fa-2x'></i>
                </div>
                <p class='title'>
                    Facebook (next SpeakEat)
                    <span>
                        (prochain · próximo SpeakEat)
                    </span>
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <a onclick="window.open('data:text/calendar;charset=utf8,' + escape(icsFile));" target="_blank" style="cursor: pointer;">
                <div class='logo'>
                    <i class='far fa-calendar-plus fa-2x'></i>
                </div>
                <p class='title'>
                    Add to Your Calendar
                    <span>(click for .ICS, or choose below)</span>
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-v" style="margin: 0 8px 8px;">
            <a onclick="window.open(urlGoogle);" target="_blank">
                <p class='title' style="margin: 10px; cursor: pointer;">
                    Google
                </p>
            </a>
        </li>
        <li class="i-v" style="margin: 0 8px 8px;">
            <a onclick="window.open(urlOutlook);" target="_blank">
                <p class='title' style="margin: 10px; cursor: pointer;">
                    Outlook
                </p>
            </a>
        </li>
        <li class="i-v" style="margin: 0 8px 8px;">
            <a onclick="window.open(urlOffice);" target="_blank">
                <p class='title' style="margin: 10px; cursor: pointer;">
                    Office 365
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <a href="#topics">
                <div class='logo'>
                    <i class='fas fa-list-ol fa-2x'></i>
                </div>
                <p class='title'>
                    List of Topics
                    <span>
                        Thèmes · Temas
                    </span>
                </p>
            </a>
        </li>
    </ul>
    <hr style="width: 100px;">
    <ul>
        <li class="i-v">
            <a onclick="document.body.className='en'">
                <p class='title' style="margin: 10px; cursor: pointer;">
                    &nbsp;EN&nbsp;
                </p>
            </a>
        </li>
        <li class="i-v">
            <a onclick="document.body.className='fr'">
                <p class='title' style="margin: 10px; cursor: pointer;">
                    &nbsp;FR&nbsp;
                </p>
            </a>
        </li>
        <li class="i-v">
            <a onclick="document.body.className='pt'">
                <p class='title' style="margin: 10px; cursor: pointer;">
                    &nbsp;PT&nbsp;
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s" title="Why plant-based food for SpeakEat? In order to join a SpeakEat, it is important that participants are open-minded. Socially, it is still not common to eat plant-based, although it can have a positive impact on our environment and overall health. SpeakEat asks, for those who want to eat, to choose a plant-based snack or meal. Such an aspect of SpeakEat is an invitation to open-mindedly try something new.">
            <span lang="en">
                <p class='title' id="info" style="font-weight: normal; margin: 20px;">
                    Hello 😉
                    <br><br>
                    ❇️ Welcome to SpeakEat, a Rotaract project aiming to promote the exchange of knowledge and experiences!
                    <br><br>
                    👥 We will have a time together, to get to know each other and exchange around the main topic.
                    <br><br>
                    🍓 If you will eat, you can share your plant-based recipe with us all when you present yourself.
                    <br><br>
                    —
                    <br><br>
                    💬 The aim of SpeakEat is to encourage conversation about important topics, with respect and goodwill!
                    <br><br>
                    🌍 It is inspired by the Rotary International cause of promoting peace to foster mutual understanding.
                    <br><br>
                    😋 It's a conversation similar to Free IC/Vegan Party, but by videocall and with a plant-based snack.
                    <br><br>
                    🏳️ We start with the main topic, and the participants decide how we will move the conversation forward.
                    <br><br>
                    —
                    <br><br>
                    🌐 Share the event with your friends and family! Everyone is welcome!
                    <br><br>
                    ⁉️ If you have any questions or suggestions, please contact us at <a href="https://e-rotaract.com">www.e-rotaract.com</a>
                </p>
            </span>
            <span lang="fr">
                <p class='title' id="info" style="font-weight: normal; margin: 20px;">
                    Salut 😉
                    <br><br>
                    ❇️ Bienvenue au SpeakEat, un projet Rotaract visant à promouvoir l'échange de connaissances et d'expériences !
                    <br><br>
                    👥 Nous aurons un moment ensemble, pour apprendre à nous connaître et échanger autour du thème principal.
                    <br><br>
                    🍓 Si vous voulez manger, vous pouvez partager votre recette plant-based avec nous tous lorsque vous vous présenterez.
                    <br><br>
                    —
                    <br><br>
                    💬 Le but de SpeakEat est d'encourager la conversation sur des sujets importants, dans le respect et la bienveillance !
                    <br><br>
                    🌍 L'action s'inspire de l'axe du Rotary International de promotion de la paix pour favoriser la compréhension mutuelle.
                    <br><br>
                    😋 C'est une conversation similaire à Free IC/Vegan Party, mais en visio et avec un petit repas plant-based.
                    <br><br>
                    🏳️ Nous démarrons par le thème principal, et les participants décident comment nous allons faire avancer la conversation.
                    <br><br>
                    —
                    <br><br>
                    🌐 Partagez l'événement à vos proches ! Toustes sont les bienvenu·e·s !
                    <br><br>
                    ⁉️ Si vous avez des questions ou suggestions, contactez nous sur <a href="https://e-rotaract.com">www.e-rotaract.com</a>
                </p>
            </span>
            <span lang="pt">
                <p class='title' id="info" style="font-weight: normal; margin: 20px;">
                    Olá 😉
                    <br><br>
                    ❇️ Bem-vinde ao SpeakEat, projeto do Rotaract que visa promover a troca de conhecimentos e experiências!
                    <br><br>
                    👥 Nós teremos um momento juntos, para nos conhecer e conversar sobre o tema principal.
                    <br><br>
                    🍓 Se você comer conosco, poderá compartilhar a sua receita plant-based no momento em que se apresentar.
                    <br><br>
                    —
                    <br><br>
                    💬 O objetivo do SpeakEat é incentivar a conversa sobre temas importantes, com respeito e boa vontade!
                    <br><br>
                    🌍 Ele é inspirado na causa do Rotary International de promover a paz para fomentar a compreensão mútua.
                    <br><br>
                    😋 É uma conversa semelhante ao Free IC/Vegan Party, mas em videochamada e com um lanche plant-based.
                    <br><br>
                    🏳️ Começamos com o tema principal, e os participantes decidem como vamos avançar a conversa.
                    <br><br>
                    —
                    <br><br>
                    🌐 Compartilhe o evento com seus amigos e familiares! Todes são bem-vindes!
                    <br><br>
                    ⁉️ Se você tiver alguma dúvida ou sugestão, pode entrar em contato conosco em <a href="https://e-rotaract.com">www.e-rotaract.com</a>
                </p>
            </span>
        </li>
    </ul>
    <hr style="width: 100px;" id="topics">
    <ul>
        <li class="i-s">
            <p class='title' id="info" style="font-weight: normal; margin: 20px;">
                <script>
                    for(let i = 0; i < list_events.length; i++) {
                        document.write(list_events[i].sym + " " + list_events[i].title +
                            " <br><a target='_blank' href='https://www.facebook.com/speak.eat.page/events'>" +
                            "<span style='float:left;'>— SpeakEat " + list_events[i].num + "</span>" +
                            "<span style='float:right;'>" + list_events[i].date + "</span></a><br><br>");
                        if(new Date(list_events[i].date) > new Date()) {
                            break;
                        }
                    }
                </script>
            </p>
        </li>
    </ul>

    <br>
    <br>

    <center><script>document.write(new Date().getFullYear())</script> &copy; SpeakEat Rotaract</center>

    <br>
    <br>
    <br>
    <br>

    <script src="{{ site.baseurl }}/assets/js/jquery.min.js"></script>
    <script src="{{ site.baseurl }}/assets/js/jquery.easing.min.js"></script>
    <script src="{{ site.baseurl }}/assets/js/grayscale.js"></script>
</body>

</html>
