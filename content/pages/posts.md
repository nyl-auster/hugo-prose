+++
draft = false
date = "2017-03-15T22:54:29+01:00"
title = "Blog"
url = "/posts/"
menu = "main"
+++

<div class="posts">
  {% for post in site.posts %}
    <article class="post">
      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>
      <div class="entry">
        {{ post.excerpt }}
      </div>
      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Lire plus</a>
    </article>
  {% endfor %}
</div>