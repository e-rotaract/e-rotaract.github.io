---
layout: blank
title: e-Rotaract Guardian-Protégé Generator
permalink: "/guardian-protege"
---

<html>

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>e-Rotaract Guardian-Protégé Generator</title>
    <link rel="stylesheet" href="/config/mini.css">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" integrity="sha384-oS3vJWv+0UjzBfQzYUhtDYW+Pj2yciDJxpsK1OYPAYjqT085Qq/1cq5FLXAZQ7Ay" crossorigin="anonymous">
    <style>
        @font-face { font-family: linja; src: url('../assets/fonts/linja-pona-4.9.otf'); } 
    </style>

    <script src="/guardian-protege/vendors/Lodash-3.10.1.js"></script>
    <script src="/guardian-protege/vendors/Cryptojs.aes-3.1.2.js"></script>

    <script src="/guardian-protege/SecretSanta.js"></script>
</head>
<body class="en" tabIndex=0>
    <div class="author-photo">
        <a class="js-scroll-trigger" href="https://www.instagram.com/rotaract_eclub">
            <img src="/assets/images/rac-e-club-logo.jpeg">
            <br>
            e-Rotaract Beyond Frontiers
            <br>
            Guardian-Protégé Generator
            <br>
        </a>
    </div>
    <br>
    <ul>
        <li class="i-s shake">
            <a target="_blank" href="https://univ-grenoble-alpes-fr.zoom.us/j/93915103056?pwd=VXl2dEVCd1dNUUhqNFd6Mk9nYmZTQT09"><!--https://meet.google.com/vue-vhfn-tec-->
                <div class='logo'>
                    <i class='fas fa-laptop fa-2x'></i>
                </div>
                <p class='title'>
                    <form id="form" class="part">
                        <textarea id="input" class="input" autofocus></textarea>
                        <button type="submit" class="generate">Generate your pairings</button>
                        <div id="result" class="result none"></div>
                    </form>
                    <script id="input-placeholder" type="text/placeholder">
                        # You can add a user by adding a line
                        Santa

                        # You can add some details if you want to, using parentheses after the name
                        Nicholas (the elf)

                        # You can prevent someone from being paired with someone else
                        Maël !Aurélie
                        Aurélie !Maël

                        # You can also exclude someone from being paired with multiple people
                        # Careful: too many exclusion rules can make your secret santa less interesting!
                        Rudolph !Santa !Nicholas (the elf)

                        # You can also cheat a bit and force someone to be paired with another
                        Nicholas (the saint) =Nicholas (the elf)

                        ...
                    </script>
                </p>
            </a>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <a target="_blank" href="https://forms.gle/8U4qf5KGMozELFnY7">
                <div class="logo" style="font-family: linja; font-size: 46px; overflow: hidden;">poki-toki</div>
                <p class="title">
                    Anonymous Form
                    <span>
                        (poki-toki: communication box)
                    </span>
                </p>
            </a>
        </li>
    </ul>
    <br><br><br>
    <hr style="width: 100px;">
    <br><br><br>
    <center>
        <script>document.write(new Date().getFullYear())</script> &copy; e-Rotaract Beyond Frontiers
    </center>
    <br><br><br>
    <script src="/config/jquery/jquery.min.js"></script>
    <script src="/config/jquery-easing/jquery.easing.min.js"></script>
    <script src="/config/grayscale.js"></script>
</body>

</html>
