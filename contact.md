---
layout: page
title: Contact
permalink: /Contact/
---

<h1 class="header center blue-text">{{ page.title | escape }}</h1>

<script type="text/javascript" src="https://webapi.amap.com/maps?v=1.4.12&key=6720218a5e53ddb5b9da631836f4c8eb">
</script>
<div id="container" ></div>
<script>
    var map = new AMap.Map("container", {
        zoom: 18,
        center:[116.473188,39.993253]
    });
    var marker = new AMap.Marker({
        map:map,
        position:[116.473188,39.993253],  
    })
    marker.on('click',function(e){
        marker.markOnAMAP({
            name:'首开广场',
            position:marker.getPosition()
        })
    })
    if(AMap.UA.mobile){
        document.getElementsByClassName('info')[0].style.display='none';
    }
</script>

