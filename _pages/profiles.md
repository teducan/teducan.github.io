---
layout: page
permalink: /people/
title: People
description: Members of the research group
nav: true
nav_order: 2
---

# 🧑‍🔬 Current Members

<div class="row">
  {% assign current = site.data.team.current %}
  {% for member in current %}
    <div class="col-md-4 mb-4">
      <div class="card h-100 border-0">
        {% if member.image %}
          <img src="{{ member.image }}" class="card-img-top rounded-circle w-50 mx-auto mt-3" alt="{{ member.name }}">
        {% endif %}
        <div class="card-body text-center">
          <h5 class="card-title">{{ member.name }}</h5>
          <p class="card-text"><strong>{{ member.role }}</strong><br>{{ member.affiliation }}</p>
          <p class="card-text small">{{ member.bio }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>
---

# 🏛️ Founding Members

<div class="row">
  {% assign founding = site.data.team.founding %}
  {% for member in founding %}
    <div class="col-md-4 mb-4">
      <div class="card h-100 border-0">
        {% if member.image %}
          <img src="{{ member.image }}" class="card-img-top rounded-circle w-50 mx-auto mt-3" alt="{{ member.name }}">
        {% endif %}
        <div class="card-body text-center">
          <h5 class="card-title">{{ member.name }}</h5>
          <p class="card-text"><strong>{{ member.role }}</strong><br>{{ member.affiliation }}</p>
          <p class="card-text small">{{ member.bio }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>

---

# 🕰️ Past Members

<div class="row">
  {% assign past = site.data.team.past %}
  {% for member in past %}
    <div class="col-md-4 mb-4">
      <div class="card h-100 border-0">
        {% if member.image %}
          <img src="{{ member.image }}" class="card-img-top rounded-circle w-50 mx-auto mt-3" alt="{{ member.name }}">
        {% endif %}
        <div class="card-body text-center">
          <h5 class="card-title">{{ member.name }}</h5>
          <p class="card-text"><strong>{{ member.role }}</strong><br>{{ member.affiliation }}</p>
          <p class="card-text small">{{ member.bio }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>

---

# 🌍 Visiting Researchers

<div class="row">
  {% assign visiting = site.data.team.visiting %}
  {% for member in visiting %}
    <div class="col-md-4 mb-4">
      <div class="card h-100 border-0">
        {% if member.image %}
          <img src="{{ member.image }}" class="card-img-top rounded-circle w-50 mx-auto mt-3" alt="{{ member.name }}">
        {% endif %}
        <div class="card-body text-center">
          <h5 class="card-title">{{ member.name }}</h5>
          <p class="card-text"><strong>{{ member.role }}</strong><br>{{ member.affiliation }}</p>
          <p class="card-text small">{{ member.bio }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>

---

# 🤝 Associate Researchers

<div class="row">
  {% assign associate = site.data.team.associate %}
  {% for member in associate %}
    <div class="col-md-4 mb-4">
      <div class="card h-100 border-0">
        {% if member.image %}
          <img src="{{ member.image }}" class="card-img-top rounded-circle w-50 mx-auto mt-3" alt="{{ member.name }}">
        {% endif %}
        <div class="card-body text-center">
          <h5 class="card-title">{{ member.name }}</h5>
          <p class="card-text"><strong>{{ member.role }}</strong><br>{{ member.affiliation }}</p>
          <p class="card-text small">{{ member.bio }}</p>
        </div>
      </div>
    </div>
  {% endfor %}
</div>
