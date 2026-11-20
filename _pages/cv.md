---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
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
* 20XX – present: Research Associate, University of Stuttgart
-->

Research interests
======
* Quantum software engineering
* Low-code development of quantum applications
* Patterns for quantum computing and quantum machine learning
* Variational quantum algorithms and hybrid quantum-classical workflows

Awards
======
* Best Paper Award, IQSOFT 2025: *Fundamental Patterns for Composing Quantum Algorithms*
* Best Paper Award, PATTERNS 2025: *Patterns for Quantum Machine Learning*

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Education packages
======
  <ul>{% for post in site.education %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
