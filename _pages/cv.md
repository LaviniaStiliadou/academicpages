---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
hide_avatar: true
redirect_from:
  - /resume
---

{% include base_path %}

<!--
TODO: Add your education and work experience here, e.g.

Education
======
* M.Sc. in ..., University of ..., 20XX

Work experience
======
* 20XX – present: Research Associate, Institute of Architecture of Application Systems (IAAS), University of Stuttgart
-->

Research interests
======
* Quantum software engineering
* Low-code development of quantum applications
* Patterns for quantum computing and quantum machine learning
* Variational quantum algorithms and hybrid quantum-classical workflows

Skills
======
* Cloud computing: hybrid and multi-cloud environments, orchestration of quantum workflows across cloud providers
* Low-code platform development (Qonstruct)
* Pattern-based software design

Awards
======
* Best Paper Award, IQSOFT 2025: *Fundamental Patterns for Composing Quantum Algorithms*
* Best Paper Award, PATTERNS 2025: *Patterns for Quantum Machine Learning*

Publications
======
{% for group in site.publication_authorship %}
  {% assign pubs = site.publications | where: "authorship", group[0] | reverse %}
  {% if pubs.size > 0 %}
### {{ group[1].title }}

  <ul>{% for post in pubs %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  {% endif %}
{% endfor %}

Education packages
======
  <ul>{% for post in site.education %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
