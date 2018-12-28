---
layout: default
title: News

---
<h1 class="header center blue-text">{{ page.title | escape }}</h1>

<div style="background: #FFF">
    <div class="container last-post">
    <section>
        <h5>Latest Post</h5>
        <ul class="collection">
        {% for post in site.posts %}
        <li class="collection-item avatar1">
          {% assign date_format = site.minima.date_format | default: "%y/%m/%d" %}
          <div class="title-form"><span class="post-title" style="font-size: 20px"><a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></span></div>
          <div class="data-form" style="font-size: 10px">{{ post.date | date: date_format }}</div>
          <p style="font-size: 13px">
            {{ post.content | strip_html | truncatewords:5}}
          </p>
          <a href="{{ post.url | relative_url }}" class="secondary-content"><i class="material-icons">navigate_next</i></a>
        </li>
        {% endfor %}
        </ul>
    </section>
    </div>