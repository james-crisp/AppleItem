layout: page
title: "Stores"
permalink: /stores/

Content

<ul>
{% for org_hash in site.data %}
{% assign org = org_hash[1] %}
  <li>
    <a href="https://github.com/{{ org.username }}">
      {{ org.name }}
    </a>
    ({{ org.members | size }} members)
  </li>
{% endfor %}
</ul>
