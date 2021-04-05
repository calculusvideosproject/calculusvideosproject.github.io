---
layout: page
title: "Optimization"
meta_title: "Optimization"
permalink: "/vids/opt/"
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
    var vidchoice=getCookie("vid6");
    if (vidchoice==1){window.location.href = "https://ximera.osu.edu/calcvids/o/opt";}
    else if (vidchoice==2){window.location.href = "https://ximera.osu.edu/calcvids/q/opt";}
    else if (vidchoice==3){window.location.href = "https://ximera.osu.edu/calcvids/v/opt";}
    else if (vidchoice==4){window.location.href = "https://ximera.osu.edu/calcvids/c/opt";}
    else {
      var forwardchoice=Math.random();
      if (forwardchoice <= 0.25 ){
        setCookie("vid6", 1, 365);
        checkCookie();
        }
      else if (forwardchoice <= 0.5 ){
        setCookie("vid6", 2, 365);
        checkCookie();
        }
      else if (forwardchoice <= 0.75 ){
        setCookie("vid6", 3, 365);
        checkCookie();
        }
      else {
        setCookie("vid6", 4, 365);
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
