---
layout: page
title: "Team"
permalink: /team/
---

<style>
.page-title, h1 {
  text-align: center;
}
.team-list {
  display: flex;
  flex-wrap: wrap;
  gap: 2em;
  justify-content: center;
  margin-top: 2em;
}
.team-member {
  text-align: center;
  max-width: 200px;
}
.team-member img {
  width: 250px;
  height: 250px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 1em;
  border: 3px solid #eee;
  transition: box-shadow 0.3s, transform 0.3s;
}
.team-member img:hover {
  box-shadow: 0 8px 24px rgba(0,0,0,0.2), 0 1.5px 3px rgba(0,0,0,0.08);
  transform: scale(1.05);
  border-color:rgb(0, 0, 0);
}
.team-member .name {
  font-size: 1.2em;
  font-weight: bold;
  margin-bottom: 0.5em;
}
.team-member .github {
  display: block;
  color: #0366d6;
  text-decoration: none;
  margin-top: 0.5em;
}
</style>

<div class="team-list">
  {% assign members = site.data.authors %}
  {% for member in members %}
    <div class="team-member">
      <img src="{{ site.baseurl }}{{ member[1].picture }}" alt="{{ member[1].name }}">
      <div class="name">{{ member[1].name }}</div>
      <a class="github" href="{{ member[1].github }}" target="_blank">GitHub</a>
    </div>
  {% endfor %}
</div>