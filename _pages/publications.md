---
layout: archive
title: "Publications"
excerpt: "Here you can find a mostly up-to-date list of my publications. By clicking on >>Read more<<, you should typically be able to access the abstract of the respective work, my own copy of the pdf, slides (if there was a talk and if I was the one giving it), and a link to the source code/artifacts of the project that produced the respective publication."
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
