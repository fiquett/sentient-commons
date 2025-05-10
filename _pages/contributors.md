---
layout: single
title: "Contributors & Advisors"
permalink: /contributors/
author_profile: false
---

{% for person in site.data.contributors %}
<div class="person-card" style="display: flex; align-items: center; margin-bottom: 2rem;">
  <img src="{{ person.avatar }}" alt="{{ person.name }}" style="width: 142px; height: 142px; border-radius: 50%; margin-right: 1rem;">
  <div>
    <strong>{{ person.name }}</strong><br>
    <em>{{ person.role }}</em><br>
    <span style="font-size: 0.9em; color: #555;">{{ person.location }}</span><br>
    <p style="margin: 0.5rem 0;">{{ person.bio }}</p>
    {% if person.url %}
      <a href="{{ person.url }}" target="_blank">View Profile</a>
    {% endif %}
  </div>
</div>
{% endfor %}
