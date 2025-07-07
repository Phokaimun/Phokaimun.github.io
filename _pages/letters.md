---
title: "Letters"
permalink: /letters/
layout: splash
header:
  overlay_image: /assets/images/background.jpg
  overlay_color: "#000"
  overlay_filter: "0.4"

persons:
  - name: "Duru Söylemezoğlu"
    title: "Secretary General"
    image_path: /assets/images/duru.jpeg
    letter_html: |
      <p>Dear Delegates, Organization Team, and Academic Team Candidates,</p>
      <p>It is my biggest pleasure to welcome you all to PHOKAIMUN'25.</p>
      <p>As the Secretary General of the First Official Session of PHOKAIMUN'25.</p>
      <p>With my dearest exec members we have worked so hard nearly a year. I'm really excited to announce this prestigious conference.</p>
      <p>Our aim was to achieve something that we would be proud when we looked back. What I want from this conference is to give the best memories to our dear academic team and our esteemed delegates.</p>
      <p>I'm looking forward to see you all in PHOKAIMUN'25.</p>
      <p>Yours sincerely,<br><strong>Duru Söylemezoğlu</strong><br><em>Secretary General</em></p>

  - name: "Ece Ertaş"
    title: "Director General"
    image_path: /assets/images/ece.jpeg
    letter_html: |
      <p>Welcome you to PHOKAIMUN'25.</p>
      <p>Over the past months, our team has worked tirelessly to bring this conference to life. Countless hours of planning, drafting, and organizing have gone into every detail to ensure that your experience here is not only educational, but also meaningful, inspiring, and enjoyable.</p>
      <p>We truly hope you feel the dedication behind this event, and that you leave with new friendships, valuable memories, and a deeper understanding of the world around you. It has been our honor to prepare this platform for passionate, thoughtful debate. And now, it’s your turn to bring it to life.</p>
      <p>Yours sincerely,<br><strong>Ece Ertaş</strong><br><em>Director General</em></p>
---

<div class="letter-container">
  {% for person in page.persons %}
    <div class="letter-column">
      <div class="letter-header">
        <img src="{{ person.image_path | relative_url }}" alt="{{ person.name }}" class="profile-image">
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
