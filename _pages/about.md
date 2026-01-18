---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a first-year PhD student at the research group for [Machine Learning and Security](https://mlsec.org/) under the supervison of [Konrad Rieck](https://mlsec.org/team/rieck/) within the [Berlin Institute for the Foundations of Learning and Data](https://www.bifold.berlin/). 
Previously, I completed a double master's degree in Computer Science and Cybersecurity at the Technical University of Munich and the Institut Polytechnique de Paris.
I hold a B.Sc. in Computer Science from LMU Munich.

---

## Publications

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

<!-- New style rendering if publication categories are defined -->
{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign has_publications = false %}
    {% for post in site.publications reversed %}
      {% if post.category == category[0] %}
        {% assign has_publications = true %}
        {% break %}
      {% endif %}
    {% endfor %}
    {% if has_publications %}
      <h2>{{ category[1].title }}</h2><hr />
      {% for post in site.publications reversed %}
        {% if post.category == category[0] %}
          {% include archive-single.html %}
        {% endif %}
      {% endfor %}
    {% endif %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

