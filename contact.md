---
layout: page
title: Contact
permalink: /Contact/
---

<h1 class="header center blue-text">{{ page.title | escape }}</h1>

<h4>Email:</h4>

<h6 style="font-size:18px;font-style:italic">Director:<h6>
<h6 style="font-size:18px">Kai Ye: kaiye@xjtu.edu.cn<h6>

<h6 style="font-size:18px;font-style:italic">Secretary:</h6>
<h6 style="font-size:18px">Jing Hai: haijing@xjtu.edu.cn</h6>

<h4>    Address:</h4>
<h6 style="font-size:18px">Ye-lab For Omics And Omic's Informatics<h6>
<h6 style="font-size:18px">Room 107, Pengkang Building<h6>
<h6 style="font-size:18px">Xi'an Jiaotong University<h6>
<h6 style="font-size:18px">No.28, Xianning West Road, Xi'an, Shaanxi<h6>
<h6 style="font-size:18px">Mail Code: 710049<h6>

<script type="text/javascript" src="https://webapi.amap.com/maps?v=1.4.12&key=6720218a5e53ddb5b9da631836f4c8eb">
</script>
<div id="container" style="height:350px;width:350px"></div>
<script>
    var map = new AMap.Map("container", {
        zoom: 17,
        center:[108.98273,34.244847]
    });
    var marker = new AMap.Marker({
        map:map,
        position:[108.98273,34.244847],  
    })
    marker.on('click',function(e){
        marker.markOnAMAP({
            name:'Pengkang Building',
            position:marker.getPosition()
        })
    })
    if(AMap.UA.mobile){
        document.getElementsByClassName('info')[0].style.display='none';
    }
</script>

