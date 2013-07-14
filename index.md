---
layout: page
title: IanWhitney.github.io
tagline: Even my posts got posts
---
{% include JB/setup %}

{% for post in site.posts %}
  <article>
    <h1>
      <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    </h1>
    <p class="meta">
      {{ post.date | date_to_long_string }} 
    </p>
   {{ post.content }} 
  </article>
{% endfor %}
