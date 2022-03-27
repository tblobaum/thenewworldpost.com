---
layout: page
title: 
---

<div class="w100">
<h1 class="archives-header">
    Authors <span>on this research project</span>
    <div class="right">{% octicon people height:24 class:"right left" aria-label:Authors %}</div>
</h1>
<ul class="left post-list posts archives box">
    {% for author in site.authors %}
<li><img class="avatar avatar-small" src="https://avatars3.githubusercontent.com/{{ author.github }}?v=3&amp;s=40" alt="{{ author.name }}" srcset="https://avatars3.githubusercontent.com/{{ author.github }}?v=3&amp;s=40 1x, https://avatars3.githubusercontent.com/{{ author.github }}?v=3&amp;s=80 2x, https://avatars3.githubusercontent.com/{{ author.github }}?v=3&amp;s=120 3x, https://avatars3.githubusercontent.com/{{ author.github }}?v=3&amp;s=160 4x" width="40" height="40" /> &nbsp;  
<span itemprop="author" itemscope itemtype="http://schema.org/Person">
    <span class="p-author h-card" itemprop="name">
        <a href="{{ site.baseurl }}{{ author.url }}">{{ author.name }}</a>
    </span>
</span></li>
    {% endfor %} 
</ul> 
</div>

