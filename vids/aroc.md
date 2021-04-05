---
layout: page
title: "Average Rate of Change"
meta_title: "ARoC"
permalink: "/vids/aroc/"
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
    var vidchoice=getCookie("aroc");
    if (vidchoice==1){window.location.href = "https://ximera.osu.edu/calcvids2019/in/c/aroc";}
    else if (vidchoice==2){window.location.href = "https://ximera.osu.edu/calcvids2019/in/o/aroc";}
    else if (vidchoice==3){window.location.href = "https://ximera.osu.edu/calcvids2019/in/v/aroc";}
    else if (vidchoice==4){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/c/aroc";}
    else if (vidchoice==5){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/o/aroc";}
    else if (vidchoice==6){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/v/aroc";}
    else {
      var forwardchoice=Math.random();
      if (forwardchoice <= (1/6) ){
        setCookie("aroc", 1, 365);
        checkCookie();
        }
      else if (forwardchoice <= (2/6) ){
        setCookie("aroc", 2, 365);
        checkCookie();
        }
      else if (forwardchoice <= (3/6) ){
        setCookie("aroc", 3, 365);
        checkCookie();
        }
        else if (forwardchoice <= (4/6) ){
          setCookie("aroc", 4, 365);
          checkCookie();
          }
          else if (forwardchoice <= (5/6) ){
            setCookie("aroc", 5, 365);
            checkCookie();
            }
      else {
        setCookie("aroc", 6, 365);
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
