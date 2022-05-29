---
layout: blank
title: e-Rotaract
permalink: "/internal"
---

<html>

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>e-Rotaract</title>
    <link rel="stylesheet" href="/config/mini.css">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" integrity="sha384-oS3vJWv+0UjzBfQzYUhtDYW+Pj2yciDJxpsK1OYPAYjqT085Qq/1cq5FLXAZQ7Ay" crossorigin="anonymous">
    <style>
        @font-face { font-family: linja; src: url('../assets/fonts/linja-pona-4.9.otf'); } 
    </style>
</head>
<body class="en" tabIndex=0>
    <div class="author-photo">
        <a class="js-scroll-trigger" href="https://www.instagram.com/rotaract_eclub">
            <img src="{{ site.baseurl }}/assets/images/rotaract-logo-pink.png">
            <br>
            @rotaract_eclub
            <br>
            e-Rotaract Beyond Frontiers
            <br>
        </a>
    </div>
    <br>
    <ul>
        <li class="i-s shake">
            <a target="_blank" href='{%for i in site.links%}{%if i.id=="meeting"%}{{i.url}}{%break%}{%endif%}{%endfor%}'>
                <div class='logo'>
                    <i class='fas fa-laptop fa-2x'></i>
                </div>
                <p class='title'>
                    Videocall · Visio
                    <span>Sunday · Dimanche · Domingo</span>
                    <span>(see calendar for day & time)</span>
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <a target="_blank" href="https://forms.gle/8U4qf5KGMozELFnY7">
                <div class="logo" style="font-family: linja; font-size: 46px; overflow: hidden;">poki-toki</div>
                <p class="title">
                    poki-toki (anonymous)
                    <span>
                        (poki-toki: communication box)
                    </span>
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <a href="https://chat.whatsapp.com/INkMh1VrXbr3H77piY4Lrh" target="_blank">
                <div class='logo'>
                    <i class='far fa-comment fa-2x'></i>
                </div>
                <p class='title'>
                    Our Chat Group
                    <span>
                        (WhatsApp)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s">
            <a href="https://drive.google.com/drive/folders/1-61TDAwYQemlLU2fu3vOkEn6Wax-iLYB?usp=sharing" target="_blank">
                <div class='logo'>
                    <i class='fas fa-cloud fa-2x'></i>
                </div>
                <p class='title'>
                    Our Cloud
                    <span>
                        (Google Drive)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s">
            <a href="https://calendar.google.com/calendar/u/4?cid=cm90YXJhY3RiZXlvbmRmcm9udGllcnNAZ21haWwuY29t" target="_blank">
                <div class='logo'>
                    <i class='far fa-calendar-plus fa-2x'></i>
                </div>
                <p class='title'>
                    Add us to your Calendar
                    <span>
                        (Add to Google Agenda)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s">
            <a href="https://calendar.google.com/calendar/embed?height=600&wkst=7&bgcolor=%23ffffff&ctz=UTC&showTitle=0&showNav=1&showDate=1&showPrint=0&showTabs=1&showCalendars=1&mode=MONTH&hl=en_GB&src=cm90YXJhY3RiZXlvbmRmcm9udGllcnNAZ21haWwuY29t&src=bGY2b2hrZGNjZ24yY3Q2N2s0amc3MTFlaGMwYTdqOHVAaW1wb3J0LmNhbGVuZGFyLmdvb2dsZS5jb20&src=ZW4tZ2IuYnJhemlsaWFuI2hvbGlkYXlAZ3JvdXAudi5jYWxlbmRhci5nb29nbGUuY29t&src=ZW4tZ2IuZnJlbmNoI2hvbGlkYXlAZ3JvdXAudi5jYWxlbmRhci5nb29nbGUuY29t&src=ZW4tZ2Iubm9yd2VnaWFuI2hvbGlkYXlAZ3JvdXAudi5jYWxlbmRhci5nb29nbGUuY29t&src=OW9ybDA3NjZ1ZnRpZzZmamFkbnJrazlpZjNldXJnajhAaW1wb3J0LmNhbGVuZGFyLmdvb2dsZS5jb20&src=cGhsbm5pc3NoMjZlZ25rYWNxdjMxYTU5dDU2NzNmaDJAaW1wb3J0LmNhbGVuZGFyLmdvb2dsZS5jb20&src=b2FxNGx0cHJvaHZwb2w5cDliYjFta3JvZnFpcDRnMmRAaW1wb3J0LmNhbGVuZGFyLmdvb2dsZS5jb20&color=%234285F4&color=%23F09300&color=%230B8043&color=%233F51B5&color=%23D81B60&color=%23A79B8E&color=%23039BE5&color=%23616161" target="_blank">
                <div class='logo'>
                    <i class='fas fa-calendar-alt fa-2x'></i>
                </div>
                <p class='title'>
                    View our Calendar
                    <span>
                        (Open in the browser)
                    </span>
                </p>
            </a>
        </li>
    </ul>
    <br><br><br>
    <hr style="width: 100px;">
    <br><br><br>
    <center>
        Pick a card!
    </center>
    <br><br><br>
    <style>
        #pick-a-card .i-s:hover .title {
            visibility: visible;
            padding-left: 0%;
        }
        #pick-a-card .title {
            visibility: hidden;
            padding-left: 25%;
        }
        #pick-a-card .i-s:hover .logo span {
            display: none;
        }
        #pick-a-card .i-s:hover .logo {
            font-size: 50px !important;
            float: left;
            text-align: left;
            padding: 15px 15px;
            width: auto;
            position: static;
            right: auto;
            top: auto;
            transform: none;
        }
        #pick-a-card .i-s .logo {
            font-size: 100px !important;
            float: initial;
            position: absolute;
            padding: 0;
            width: 95%;
            max-width: none;
            right: 0;
            top: 50%;
            transform: translateY(-50%);
        }
    </style>
    <ul id="pick-a-card">
        <li class="i-s">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    jan
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;jan</span>
                </div>
                <p class="title">
                    🙂 I think I can invite someone to participate
                    <span>
                        (jan: person, someone)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s bg-orange">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    nimi
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;nimi</span>
                </div>
                <p class="title">
                    ✏️ One word or sentence to describe this moment
                    <span>
                        (nimi: word, name)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s bg-green">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    pona
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;pona</span>
                </div>
                <p class="title">
                    💌 Recommend an article, book, movie, video, event, recipe, website, game...
                    <span>
                        (pona: good, positive, useful)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    pana
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;pana</span>
                </div>
                <p class="title">
                    🤝‍ Looking for someone to give me a hand or give me some guidance
                    <span>
                        (pana: give, provide)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s bg-orange">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    tenpo
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;tenpo</span>
                </div>
                <p class="title">
                    🕰️ The speed of my week (slow-fast) and a reason
                    <span>
                        (tenpo: time, duration)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s bg-green">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    pilin
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;pilin</span>
                </div>
                <p class="title">
                    🎭 My mood today, or my mood for the past week
                    <span>
                        (pilin: feeling, emotion, mood)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    sona
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;sona</span>
                </div>
                <p class="title">
                    💡 An interesting idea I want to share with you all
                    <span>
                        (sona: idea, insight)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s bg-orange">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    pali
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;pali</span>
                </div>
                <p class="title">
                    ⚙️ The progress or result of an action or a project
                    <span>
                        (pali: work, action, project)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s bg-green">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    tawa
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;tawa</span>
                </div>
                <p class="title">
                     ⏭️ What I am going to do these next few days
                    <span>
                        (tawa: going to, advance)
                    </span>
                </p>
            </a>
        </li>
        <li class="i-s">
            <a>
                <div class="logo" style="font-family: linja; font-size: 50px;">
                    toki
                    <span style="font-family: 'Noto Sans', Tahoma, sans-serif; font-size: 16px;">&nbsp;&nbsp;toki</span>
                </div>
                <p class="title">
                    📣 A recent important thing I want to say/share
                    <span>
                        (toki: talk, inform)
                    </span>
                </p>
            </a>
        </li>
    </ul>
    <br><br><br>
    <hr style="width: 100px;">
    <br><br><br>
    <center>
        What is important to us!
        <br>
        (121 answers!!!)
    </center>
    <br><br><br>
    <ul>
        <li class="i-s">
            <a>
                <div class='logo'>
                    <i class='far fa-heart fa-2x'></i>
                </div>
                <p class='title'>
                    Our Values
                </p>
            </a>
        </li>
    </ul>
    <ul id="ourValues"></ul>
    <script>
        var colors = ["bg-orange", "", "bg-green"];
        var colorNum = 0;
        function nextColor() {
            colorNum = (colorNum + 1) % 3;
            return colors[colorNum];
        }
        document.getElementById("ourValues").innerHTML =
            // heath causes
            ["Blood Donation", "Bone Marrow Donation", "Organs Donation", "All Donations", "All Cancers Prevention", "Prostate Cancer", "Breast Cancer", "Lung Cancer", "Skin Cancer", "Colorectal/Bowel Cancer", "Healthy Habits", "Psychological Wellbeing", "Emotional Intelligence", "HIV/AIDS", "All Diseases Prevention/Cure", "Clean Water", "Nutrition Adequacy", "Sex/Relationship Education", "Contraception/Birth Control", "Coronavirus/Covid-19",
            // social causes
            "Accessibility", "Racism", "Veganism", "Feminism", "Ableism", "LGBT+", "Xenophobia", "Carnism ", "Speciesism", "Environment", "Islamophobia", "Data Privacy", "Human Rights", "Peace", "Net Neutrality", "Support Small Businesses", "Waste Reduction", "Minimalism", "Milk Tea Alliance", "Animal Rights/Welfare",
            // core values
            "Goodwill", "Open-mindedness", "Honesty/Transparency", "Diversity", "Transparency", "Justice", "Humility", "Solidarity", "Mutual Respect", "Good Manners", "Assertiveness", "Altruism", "Secularism", "Equality/Equity", "Collaboration", "Leadership", "Responsibility", "Engagement", "Communication", "Kindness", "Not forced to be 'nice/happy/smiley'"]
            .sort()
            .map(i => "<li class='i-v " + nextColor() + "' style='margin: 5px 8px;'><a><p class='title' style='margin: 10px; cursor: pointer;'>" + i + "</p></a></li>")
            .join("");
    </script>
    <br><br><br>
    <center>
        <script>document.write(new Date().getFullYear())</script> &copy; e-Rotaract Beyond Frontiers
        <br><span style="color: #FFFFFF00;">767709</span>
    </center>
    <br><br><br>
    <script src="/config/jquery/jquery.min.js"></script>
    <script src="/config/jquery-easing/jquery.easing.min.js"></script>
    <script src="/config/grayscale.js"></script>
</body>

</html>
