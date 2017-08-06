---
layout: default
---

Hi! Welcome to my homepage. I am a data scientist and consultant currently based in London.
You can read more about me [here](/about).


<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
      
      <p>{{ post.content }}</p>
      
      <!-- | strip_html | truncatewords:75 -->
     <!-- {{ post.excerpt }}  -->
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>