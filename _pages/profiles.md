---
layout: page
permalink: /people/
title: People
description: Members of the research group
nav: true
nav_order: 2
---

<style>
.profile-row {
  display: flex;
  flex-direction: row;
  margin-bottom: 2rem;
  align-items: flex-start;
}

.profile-img {
  max-width: 150px;
  margin-right: 2rem;
  border-radius: 8px;
}

.profile-info {
  flex: 1;
}
.profile-info h3 {
  margin-top: 0;
  margin-bottom: 0.2rem;
}
.profile-info .role {
  font-weight: bold;
  font-size: 0.95em;
  color: #555;
}
.profile-info .affiliation {
  font-style: italic;
  font-size: 0.9em;
  color: #666;
}
</style>

{% assign sections = "current,founding,past,associate,visiting" | split: "," %}

{% for section in sections %}
  {% assign members = site.data.team[section] %}
  {% if members %}
    <h2 style="margin-top:3rem">{{ section | capitalize }} Members</h2>
    {% for person in members %}
    <div class="profile-row">
      {% if person.image %}
        <img class="profile-img" src="{{ person.image }}" alt="{{ person.name }}">
      {% endif %}
      <div class="profile-info">
        <h3>
          {% if person.link %}
            <a href="{{ person.link }}">{{ person.name }}</a>
          {% else %}
            {{ person.name }}
          {% endif %}
        </h3>
        {% if person.role %}<div class="role">{{ person.role }}</div>{% endif %}
        {% if person.affiliation %}<div class="affiliation">{{ person.affiliation }}</div>{% endif %}
        <p>{{ person.bio }}</p>
      </div>
    </div>
    {% endfor %}
  {% endif %}
{% endfor %}
