---
title: "Letters"
permalink: /letters/
layout: splash
header:
  overlay_image: /assets/images/background.jpg
  overlay_color: "#000"
  overlay_filter: "0.4"

---

<h2 class="text-center" style="font-family: serif; font-style: italic; color: #888;">from our executive team</h2>

<hr>

<div class="letter-container">
  {% for person in site.data.letters %}
    <div class="letter-column">
      <div class="letter-header">
        <img src="{{ person.image_path }}" alt="{{ person.name }}" class="profile-image">
        <div class="person-details">
          <h3 class="person-name">{{ person.name }}</h3>
          <p class="person-title">{{ person.title }}</p>
        </div>
      </div>
      <div class="letter-body">
        {{ person.letter_html | markdownify }}
      </div>
    </div>
  {% endfor %}
</div>
