---
layout: blank
title: e-Rotaract Match Generator
permalink: "/pairs"
---

<html>

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>e-Rotaract Pairs Generator</title>
    <link rel="stylesheet" href="/config/mini.css">
    <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.2/css/all.css" integrity="sha384-oS3vJWv+0UjzBfQzYUhtDYW+Pj2yciDJxpsK1OYPAYjqT085Qq/1cq5FLXAZQ7Ay" crossorigin="anonymous">
</head>
<body class="en" tabIndex=0>
    <div class="author-photo">
        <a class="js-scroll-trigger" href="https://www.instagram.com/rotaract_eclub">
            <img src="/assets/images/logo/rotaract-pink.png">
            <br>
            e-Rotaract Beyond Frontiers
            <br>
            Pairs Generator
            <br>
        </a>
    </div>
    <br>
    <ul id="displaying" style="display: none;">
        <li class="i-s">
            <p class='title' id="display">
                Error displaying result...
            </p>
        </li>
    </ul>
    <span id="generation">
        <ul>
            <li class="i-s">
                <div class='logo'>
                    <i class='fas fa-edit fa-2x'></i>
                </div>
                <p class='title'>
                    - Write 1 name per line
                    <br>
                    - Use A-Z letters or spaces
                    <br>
                    - No special characters
                    <br>
                    - No accents
                </p>
            </li>
        </ul>
        <ul id="form">
            <li class="i-s">
                <div class='logo'>
                    <i class='fas fa-list fa-2x'></i>
                </div>
                <p class='title'>
                    <textarea id="input" class="input" autofocus style="height: 150px;"></textarea>
                </p>
            </li>
        </ul>
        <ul>
            <li class="i-s">
                <div class='logo'>
                    <i class='fas fa-key fa-2x'></i>
                </div>
                <p class='title'>
                    <input type="checkbox" id="secret" name="secret" value="Secret">
                    <label for="secret">Check it to generate secret links!</label>
                </p>
            </li>
        </ul>
        <ul>
            <li class="i-s" onclick="generate()">
                <div class='logo'>
                    <i class='fas fa-dice fa-2x'></i>
                </div>
                <p class='title'>
                        Generate!
                </p>
            </li>
        </ul>
        <ul id="result-list">
        </ul>
    </span>
    <script>
        var dict = {
            "A": "_",
            "B": "9",
            "C": "8",
            "D": "7",
            "E": "6",
            "F": "5",
            "G": "4",
            "H": "3",
            "I": "2",
            "J": "1",
            "K": "0",
            "L": "Z",
            "M": "Y",
            "N": "X",
            "O": "W",
            "P": "V",
            "Q": "U",
            "R": "T",
            "S": "S",
            "T": "R",
            "U": "Q",
            "V": "P",
            "W": "O",
            "X": "N",
            "Y": "M",
            "Z": "L",
            "0": "K",
            "1": "J",
            "2": "I",
            "3": "H",
            "4": "G",
            "5": "F",
            "6": "E",
            "7": "D",
            "8": "C",
            "9": "B",
            "_": "A"
        }
    ;
        var vars = {};
        window.location.href.replace(/[?&]+([^=&]+)=([^&]*)/gi, function(m, key, value) {
            vars[key] = value;
        });
    ;
        if(vars["i1"] != null) {
            document.getElementById("generation").style.display = "none";
            document.getElementById("displaying").style.display = "";
            document.getElementById("display").innerHTML = "<center>"
                + "👼 "
                + vars["i1"]
                + "<br><i class='fas fa-arrow-down'></i><br>"
                + "💎 "
                + decypherString(vars["i2"])
                + "</center>"
                ;
        }
    ;
        function arrayRemove(arr, value) {
            return arr.filter(function(element) {
                return element != value;
            });
        }
    ;
        function getRandomInt(min, max) {
            min = Math.ceil(min);
            max = Math.floor(max);
            return Math.floor(Math.random() * (max - min + 1)) + min;
        }
    ;
        function setCharAt(str, index, chr) {
            if(index > str.length-1) return str;
            return str.substring(0,index) + chr + str.substring(index+1);
        }
    ;
        function getKeyByValue(object, value) {
            return Object.keys(object).find(key => object[key] === value);
        }
    ;
        function cypherCharAt(str, index, chr) {
            if(index > str.length-1) return str;
        ;
            var randomNum = getRandomInt(10, 99).toString();
            for(let i=0; i < randomNum.length; i++) {
                randomNum = setCharAt(randomNum, i, dict[randomNum[i]]);
            }
        ;
            var randomNum2 = getRandomInt(10, 99).toString();
            for(let i=0; i < randomNum2.length; i++) {
                randomNum2 = setCharAt(randomNum2, i, dict[randomNum2[i]]);
            }
        ;
            return str.substring(0,index) + randomNum + chr + randomNum2 + str.substring(index+1);
        }
    ;
        function decypherString(str) {
            var name = "";
            for(let i=2; i < str.length; i+=5) {
                name += getKeyByValue(dict, str[i]);
            }
            return name;
        }
    ;
        function shuffleArray(a) {
            var j, x, i;
            for (i = a.length - 1; i > 0; i--) {
                j = Math.floor(Math.random() * (i + 1));
                x = a[i];
                a[i] = a[j];
                a[j] = x;
            }
            return a;
        }
    ;
        function generate() {
            var names = document.getElementById("input").value;
        ;
            if(!/^[A-Za-z \n]+$/.test(names)) {
                document.getElementById("result-list").innerHTML = "❌ Names contain invalid characters...";
                return;
            }
        ;
            names = names.replace(/ /gu, "_").toUpperCase().normalize("NFD").replace(/\p{Diacritic}/gu, "").trim().split("\n");
            names = shuffleArray(names);
        ;
            pairings = new Map();
            for(let i=0; i < names.length; i++) {
                pairings.set(names[i], names[(i+1)%names.length]);
            }
        ;
            document.getElementById("result-list").innerHTML = "";
        ;
            var url1 = "http://" + window.location.host + "/pairs?i1=";
            var url2 = "&i2=";
        ;
            if(document.getElementById("secret").checked) {
                pairings.forEach((k, v) => {
                    for(let i=0; i < v.length; i+=5) {
                        v = cypherCharAt(v, i, dict[v[i]]);
                    }
                ;
                    var item = "<li class='i-s'>"
                        + "<div class='logo'>"
                        + "<a href='javascript:navigator.clipboard.writeText($(\"#id-" + k + "\").val())'>"
                        + "<i class='fas fa-copy fa-2x'></i>"
                        + "</a>"
                        + "</div>"
                        + "<p class='title'>"
                        + "👼 " + k + "<br>"
                        + "💎 <input type='text' id='id-" + k + "' value='" + url1 + k + url2 + v + "'>"
                        + "</p>"
                        + "</li>";
                    if(getRandomInt(0, 1) == 0) {
                        document.getElementById("result-list").innerHTML = item + document.getElementById("result-list").innerHTML;
                    } else {
                        document.getElementById("result-list").innerHTML += item;
                    }
                });
            } else {
                document.getElementById("result-list").innerHTML = "<li class='i-s'>"
                        + "<div class='logo'>"
                        + "<a href='javascript:navigator.clipboard.writeText($(\"#result\").text())'>"
                        + "<i class='fas fa-copy fa-2x'></i>"
                        + "</a>"
                        + "</div>"
                        + "<p class='title' id='result'>"
                        + "</p>"
                        + "</li>";
                pairings.forEach((k, v) => document.getElementById("result").innerHTML += "<p>👼 " + k + " → 💎 " + v + ", </p>");
            }
        }
    </script>
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
