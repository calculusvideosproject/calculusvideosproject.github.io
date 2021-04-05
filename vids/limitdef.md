---
layout: page
title: "Limit Definition of Derivative"
meta_title: "limitdef"
permalink: "/vids/limitdef/"
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
    var vidchoice=getCookie("limitdef");
    if (vidchoice==1){window.location.href = "https://ximera.osu.edu/calcvids2019/in/c/limitdef";}
    else if (vidchoice==2){window.location.href = "https://ximera.osu.edu/calcvids2019/in/o/limitdef";}
    else if (vidchoice==3){window.location.href = "https://ximera.osu.edu/calcvids2019/in/v/limitdef";}
    else if (vidchoice==4){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/c/limitdef";}
    else if (vidchoice==5){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/o/limitdef";}
    else if (vidchoice==6){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/v/limitdef";}
    else {
      var forwardchoice=Math.random();
      if (forwardchoice <= (1/6) ){
        setCookie("limitdef", 1, 365);
        checkCookie();
        }
      else if (forwardchoice <= (2/6) ){
        setCookie("limitdef", 2, 365);
        checkCookie();
        }
      else if (forwardchoice <= (3/6) ){
        setCookie("limitdef", 3, 365);
        checkCookie();
        }
        else if (forwardchoice <= (4/6) ){
          setCookie("limitdef", 4, 365);
          checkCookie();
          }
          else if (forwardchoice <= (5/6) ){
            setCookie("limitdef", 5, 365);
            checkCookie();
            }
      else {
        setCookie("limitdef", 6, 365);
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
