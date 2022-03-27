---
layout: default
---
<div class="left w50">
<h1 class="archives-header">
    Posts <span>by {{ page.name }}</span>
    <div class="right">{% octicon pencil height:24 class:"right left" aria-label:Author %}</div>
</h1>
<ul class="left post-list posts archives box">
    {% for post in site.posts offset:0 %} 
        {% if post.author == page.github %}
            {% include postbox.html %} 
        {% endif %}
    {% endfor %} 
</ul> 
</div>

<div class="right w50" style="width: 49%; max-width: 49%; min-width: 49%; margin-left: 10px;">

<h1 class="archives-header">
    {{ page.name }} <span>Author</span>
    <div class="right">{% octicon person height:24 class:"right left" aria-label:Author %}</div>
</h1>


<p>{% octicon location height:16 class:"" aria-label:hi %} &nbsp; {{ page.location }}</p]>
<img class="avatar avatar-small right" src="https://avatars3.githubusercontent.com/{{ page.github }}?v=3&amp;s=40" alt="{{ page.name }}" srcset="https://avatars3.githubusercontent.com/{{ page.github }}?v=3&amp;s=40 1x, https://avatars3.githubusercontent.com/{{ page.github }}?v=3&amp;s=80 2x, https://avatars3.githubusercontent.com/{{ page.github }}?v=3&amp;s=120 3x, https://avatars3.githubusercontent.com/{{ page.github }}?v=3&amp;s=160 4x" width="80" height="80" /> &nbsp;  

<p>{% octicon mail height:16 class:"" aria-label:hi %} &nbsp; {{ page.email }}</p>
<p>{% octicon home height:16 class:"" aria-label:hi %} &nbsp; {{ page.website }}</p>

<p><a href="https://github.com/{{ page.github }}"><span class="icon icon--github">{% include icon-github.svg %}</span> &nbsp; <span class="username">{{ page.github }}</span></a></p>
<p> <a href="https://twitter.com/{{ page.twitter }}"><span class="icon icon--twitter">{% include icon-twitter.svg %}</span> &nbsp; <span class="username">{{ page.twitter }}</span></a></p>

{{ content }}

<br> 
<br>

<form action="{{ site.baseurl }}/authors">
    <button class="btn btn-secondary" type="submit" style="line-height:16px;">{% octicon arrow-left height:16 class:"right left" aria-label:Edit %} &nbsp; More Authors</button>
</form>

</div>
