---
layout: page
title: "Product Rule"
meta_title: "product"
permalink: "/vids/product/"
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
    var vidchoice=getCookie("product");
    if (vidchoice==1){window.location.href = "https://ximera.osu.edu/calcvids2019/in/c/product";}
    else if (vidchoice==2){window.location.href = "https://ximera.osu.edu/calcvids2019/in/o/product";}
    else if (vidchoice==3){window.location.href = "https://ximera.osu.edu/calcvids2019/in/v/product";}
    else if (vidchoice==4){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/c/product";}
    else if (vidchoice==5){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/o/product";}
    else if (vidchoice==6){window.location.href = "https://ximera.osu.edu/calcvids2019/nin/v/product";}
    else {
      var forwardchoice=Math.random();
      if (forwardchoice <= (1/6) ){
        setCookie("product", 1, 365);
        checkCookie();
        }
      else if (forwardchoice <= (2/6) ){
        setCookie("product", 2, 365);
        checkCookie();
        }
      else if (forwardchoice <= (3/6) ){
        setCookie("product", 3, 365);
        checkCookie();
        }
        else if (forwardchoice <= (4/6) ){
          setCookie("product", 4, 365);
          checkCookie();
          }
          else if (forwardchoice <= (5/6) ){
            setCookie("product", 5, 365);
            checkCookie();
            }
      else {
        setCookie("product", 6, 365);
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
