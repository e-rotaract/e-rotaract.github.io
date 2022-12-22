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
</head>
<body class="en" tabIndex=0>
    <div class="author-photo">
        <a class="js-scroll-trigger" href="https://www.instagram.com/rotaract_eclub">
            <img src="/assets/images/logo/rotaract-pink.png">
            <br>
            e-Rotaract Beyond Frontiers
            <br>
            Guardian-Protégé Generator
            <br>
        </a>
    </div>
    <br>
    <ul id="form">
        <li class="i-s">
            <div class='logo'>
                <i class='fas fa-list fa-2x'></i>
            </div>
            <p class='title'>
                    <textarea id="input" class="input" autofocus style="height: 100px;"></textarea>
                    <br>
                    <input type="checkbox" id="secret" name="secret" value="Secret">
                    <label for="secret"> is it secret?</label>
            </p>
        </li>
    </ul>
    <ul id="generate">
        <li class="i-s" onclick="generate()">
            <div class='logo'>
                <i class='fas fa-dice fa-2x'></i>
            </div>
            <p class='title'>
                    Generate!
            </p>
        </li>
    </ul>
    <ul>
        <li class="i-s">
            <div class='logo'>
                <i class='far fa-user-friends fa-2x'></i>
            </div>
            <p class='title' id="result">
                    Result...
            </p>
        </li>
    </ul>
    <script>
        var dict = {
            "a": "9",
            "b": "8",
            "c": "7",
            "d": "6",
            "e": "5",
            "f": "4",
            "g": "3",
            "h": "2",
            "i": "1",
            "j": "0",
            "k": "z",
            "l": "y",
            "m": "x",
            "n": "w",
            "o": "v",
            "p": "u",
            "q": "t",
            "r": "s",
            "s": "r",
            "t": "q",
            "u": "p",
            "v": "o",
            "w": "n",
            "x": "m",
            "y": "l",
            "z": "k",
            "0": "j",
            "1": "i",
            "2": "h",
            "3": "g",
            "4": "f",
            "5": "e",
            "6": "d",
            "7": "c",
            "8": "b",
            "9": "a"
        }

        var vars = {};
        window.location.href.replace(/[?&]+([^=&]+)=([^&]*)/gi, function(m,key,value) {
            vars[key] = value;
        });

        if(vars["guardian"] != null) {
            document.getElementById("form").style.display = "none";
            document.getElementById("generate").style.display = "none";
            document.getElementById("result").innerHTML = "Guradian: " + vars["guardian"] + "<br>Protégé: " + decypherString(vars["protege"]);
        }
        
        function arrayRemove(arr, value) {     
            return arr.filter(function(ele) { 
                return ele != value;
            });
        }

        function getRandomInt(min, max) {
            min = Math.ceil(min);
            max = Math.floor(max);
            return Math.floor(Math.random() * (max - min + 1)) + min;
        }

        function setCharAt(str, index, chr) {
            if(index > str.length-1) return str;
            return str.substring(0,index) + chr + str.substring(index+1);
        }

        function getKeyByValue(object, value) {
            return Object.keys(object).find(key => object[key] === value);
        }

        function cypherCharAt(str, index, chr) {
            if(index > str.length-1) return str;

            var randomNum = getRandomInt(10, 99).toString();
            for(let i=0; i < randomNum.length; i++) {
                randomNum = setCharAt(randomNum, i, dict[randomNum[i]]);
            }

            var randomNum2 = getRandomInt(10, 99).toString();
            for(let i=0; i < randomNum2.length; i++) {
                randomNum2 = setCharAt(randomNum2, i, dict[randomNum2[i]]);
            }

            return str.substring(0,index) + randomNum + chr + randomNum2 + str.substring(index+1);
        }

        function decypherString(str) {
            var name = "";
            for(let i=2; i < str.length; i+=5) {
                name += getKeyByValue(dict, str[i]);
            }
            return name;
        }

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

        function generate() {
            var names = document.getElementById("input").value;
            names = names.toLowerCase().normalize("NFD").replace(/\p{Diacritic}/gu, "").trim().split("\n");
            names = shuffleArray(names);
            
            pairings = new Map();
            for(let i=0; i < names.length; i++) {
                pairings.set(names[i], names[(i+1)%names.length]);
            }

            document.getElementById("result").innerHTML = "";
            
            var url1 = "https://e-rotaract.com/guardian-protege?guardian=";
            var url2 = "&protege=";

            if(document.getElementById("secret").checked) {
                pairings.forEach((k, v) => {
                    for(let i=0; i < v.length; i+=5) {
                        v = cypherCharAt(v, i, dict[v[i]]);
                    }

                    if(getRandomInt(0, 1) == 0) {
                        document.getElementById("result").innerHTML = k + ":<br><input type='text' value='" + url1 + k + url2 + v + "'><br><br>" + document.getElementById("result").innerHTML;
                    } else {
                        document.getElementById("result").innerHTML += k + ":<br><input type='text' value='" + url1 + k + url2 + v + "'><br><br>";
                    }
                    
                });
            } else {
                pairings.forEach((k, v) => document.getElementById("result").innerHTML += k + " -> " + v + "<br><br>");
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
