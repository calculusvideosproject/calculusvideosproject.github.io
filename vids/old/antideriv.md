---
layout: page
title: "Antiderivatives"
meta_title: "Antiderivatives"
permalink: "/vids/antideriv/"
---

<html>
<head>
<script>

function setCookie(cname,cvalue,exdays) {
    var d = new Date();
    d.setTime(d.getTime() + (exdays*24*60*60*1000));
    var expires = "expires=" + d.toGMTString();
    document.cookie = cname + "=" + cvalue + ";" + expires + ";path=/";
}

function getCookie(cname) {
    var name = cname + "=";
    var decodedCookie = decodeURIComponent(document.cookie);
    var ca = decodedCookie.split(';');
    for(var i = 0; i < ca.length; i++) {
        var c = ca[i];
        while (c.charAt(0) == ' ') {
            c = c.substring(1);
        }
        if (c.indexOf(name) == 0) {
            return c.substring(name.length, c.length);
        }
    }
    return "";
}

function checkCookie() {
    var vidchoice=getCookie("antideriv");
    if (vidchoice==1){window.location.href = "https://ximera.osu.edu/calcvids/o/antideriv";}
    else if (vidchoice==2){window.location.href = "https://ximera.osu.edu/calcvids/q/antideriv";}
    else if (vidchoice==3){window.location.href = "https://ximera.osu.edu/calcvids/c/antideriv";}
    else {
      var forwardchoice=Math.random();
      if (forwardchoice <= 0.33 ){
        setCookie("antideriv", 1, 365);
        checkCookie();
        }
      else if (forwardchoice <= 0.66 ){
        setCookie("antideriv", 2, 365);
        checkCookie();
        }
      else {
        setCookie("antideriv", 3, 365);
        checkCookie();
        }
      }
}


</script>
</head>
<body onload="checkCookie()">
Loading...
</body>
</html>
