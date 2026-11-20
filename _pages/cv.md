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
- **Quantum programming:** Python, OpenQASM 3, quantum circuit design and transformation
- **Quantum algorithms:** variational quantum algorithms, quantum neural networks, quantum machine learning, warm-starting
- **Quantum software engineering:** low-code platforms, model-to-code transformation, patterns, hybrid quantum-classical workflows
- **Cloud and workflows:** orchestration and observability of quantum workflows across hybrid and multi-cloud environments
- **Platforms:** Qonstruct, QHAna
<!-- TODO: please verify and complete: SDKs (Qiskit, PennyLane, ...), quantum hardware/providers used (IBM Quantum, AWS Braket, IonQ, ...), languages/frameworks (TypeScript, React, Flask, Docker, Kubernetes, BPMN/Camunda, ...) -->

Leadership
======
- Supervised **26 theses and student projects**: 6 Master's theses, 6 Bachelor's theses, and 14 research and development projects, 11 of them team projects with up to 7 students (see [Teaching](/teaching/)).
- Co-developing the low-code platform Qonstruct together with colleagues and student teams.
<!-- TODO: add project leadership (e.g. "Technical lead of Qonstruct") and funded projects (name, funder, your role) if applicable -->

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
