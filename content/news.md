---
title: HYDDA
layout: default
---
<div class="home">

  <h2 class="alt-h2">News</h2>

  <ul class="list-style-none blog-posts-list-hydda">
    {% for post in site.posts %}
      <li>
        <a class="alt-h3" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        <span class="float-right ml-2">{{ post.date | date: "%b %d, %Y" }}</span>
        {% if post.tags.first == 'index' %}
          {% for tag in post.tags offset:1 %}
            <span class="float-right Label bg-hydda mt-3 mr-1">{{ tag }}</span>
          {% endfor %}
        {% endif %}
      </li>
    {% endfor %}
  </ul>

</div>