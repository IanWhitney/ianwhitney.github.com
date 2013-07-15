---
layout: page
title: IanWhitney.github.io
tagline: Even my posts got posts
---
{% include JB/setup %}

{% for post in site.posts %}
  <article>
    <h1>
      {{ post.title }}
    </h1>
    <p class="meta">
      {{ post.date | date_to_long_string }} 
    </p>
    {{ post.content }}
    <p>
      <a href="{{ BASE_PATH }}{{ post.url }}">Leave a comment</a>
    </p>
  </article>
  <hr />
{% endfor %}
