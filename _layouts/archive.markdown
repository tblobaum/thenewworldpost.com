---
layout: default 
---

<h1>Archive of posts with {{ page.type }} '{{ page.title }}'</h1>
<ul class="post-list posts archives">
  {% for post in page.posts %}
      <li class="bomb-staggered">
    <div class="bomb-img">
      {% if post.featured-image %}{% include post-featured-image.html image=post.featured-image alt=post.featured-image-alt %}{% endif %}
      {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
    </div>
    <div class="bomb-text">
      <span class="post-meta">{{ post.date | date: date_format }}</span>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h3> 
        <!-- {{ post.excerpt | truncate: 140 }}  -->
    </div>
  </li>
  {% endfor %}
</ul>