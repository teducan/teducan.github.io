---
layout: page
title: Team
permalink: /team/
---

<div class="row">
  {% for member in site.data.team %}
    <div class="col-md-4 mb-4">
      <div class="card h-100 border-0">
        <img src="{{ member.photo }}" class="card-img-top rounded-circle w-50 mx-auto mt-3" alt="{{ member.name }}">
        <div class="card-body text-center">
          <h5 class="card-title">{{ member.name }}</h5>
          <p class="card-text"><strong>{{ member.role }}</strong><br>{{ member.affiliation }}</p>
          <p class="card-text small">{{ member.bio }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>
