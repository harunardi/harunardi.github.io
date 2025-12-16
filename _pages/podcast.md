---
title: "Bicara Nuklir Podcast"
permalink: /podcast/
author_profile: true
---

Welcome to Bicara Nuklir Podcast! 🎙️

<p>
<a href="https://open.spotify.com/show/7Ccn9sv462INHxCBosDr6v" target="_blank">
🎧 Listen on Spotify
</a>
</p>

---

<ul class="cv-list">
{% for ep in site.data.podcast reversed %}
  <li class="cv-item">

    <div class="cv-item-header">
      <div class="cv-item-title">
        S{{ ep.season }}E{{ ep.episode }}: {{ ep.title }}
      </div>
      <div class="cv-item-date">
        <a href="{{ ep.spotify }}" target="_blank">Spotify</a>
      </div>
    </div>

    {% if ep.description %}
    <div class="cv-item-content">
      <div class="cv-item-detail">
        {{ ep.description }}
      </div>
    </div>
    {% endif %}

  </li>
{% endfor %}
</ul>
