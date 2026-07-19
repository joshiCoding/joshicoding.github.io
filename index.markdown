---
layout: default
title: Home
permalink: /
---

<section class="hero">

<div class="hero-container">

<div class="hero-image">
    <img src="{{ '/assets/images/profile.jpg' | relative_url }}" alt="Mohit Joshi">
</div>

<div class="hero-content">

<h1>Mohit Joshi</h1>

<h2>Ph.D. Research Scholar</h2>

<p class="hero-university">
Department of Computer Science<br>
Banaras Hindu University, Varanasi, India
</p>

<p class="hero-tags">

<span>Quantum Computing</span>

<span>Blind Quantum Computation</span>

<span>Quantum Cryptography</span>

<span>Secure Delegated Computing</span>

<span>Quantum Algorithms</span>

</p>

<p class="hero-description">

My research focuses on developing practical and resource-efficient
protocols for <strong>Blind Quantum Computation</strong>,
<strong>Quantum Homomorphic Encryption</strong>,
and <strong>Secure Delegated Quantum Computing</strong>.
I also develop open-source software for quantum computing research.

</p>

<div class="hero-buttons">

<a href="/cv/Mohit_Joshi_CV.pdf" class="btn">CV</a>

<a href="https://scholar.google.com/" class="btn" target="_blank">Scholar</a>

<a href="https://github.com/joshiCoding" class="btn" target="_blank">GitHub</a>

<a href="mailto:joshi.mohit1221@gmail.com" class="btn">Email</a>

</div>

</div>

</div>

</section>

<hr>

# Research Interests

<div class="card-grid">

<div class="card">

## Blind Quantum Computation

Design of secure delegated quantum computation
protocols with information-theoretic privacy.

</div>

<div class="card">

## Quantum Cryptography

Quantum key distribution, secure delegated
computation, quantum homomorphic encryption.

</div>

<div class="card">

## Quantum Algorithms

Grover's algorithm, quantum search,
resource estimation and optimization.

</div>

<div class="card">

## NISQ Computing

Noise analysis and hardware-aware optimization
for near-term quantum devices.

</div>

<div class="card">

## Quantum Searchable Encryption

Application of blind quantum computation
to secure cloud search.

</div>

<div class="card">

## Quantum Software

Development of open-source quantum computing
libraries and tools.

</div>

</div>

---

# Featured Publications

{% assign featured = site.data.publications | where: "featured", true %}

{% for paper in featured %}

<div class="publication-card">

### {{ paper.title }}

**{{ paper.journal }}** ({{ paper.year }})

{{ paper.authors }}

{% if paper.quartile %}
**{{ paper.quartile }}**
{% endif %}

{% if paper.impact_factor %}
Impact Factor: {{ paper.impact_factor }}
{% endif %}

<div class="paper-buttons">

{% if paper.pdf != "" %}
<a href="{{ paper.pdf }}" class="btn-small">
PDF
</a>
{% endif %}

{% if paper.doi != "" %}
<a href="{{ paper.doi }}" target="_blank" class="btn-small">
DOI
</a>
{% endif %}

</div>

</div>

{% endfor %}

<p align="center">

<a href="/publications/" class="btn">
View All Publications
</a>

</p>

---

# Software

<div class="software-card">

# BlindTranspiler

An open-source Python framework for

- Blind Quantum Computation

- Quantum Homomorphic Encryption

- Secure Delegated Quantum Computing

<div class="paper-buttons">

<a href="https://github.com/joshiCoding/blind_transpiler" class="btn-small">

GitHub

</a>

<a href="https://joshicoding.in/blind_transpiler/" class="btn-small">

Documentation

</a>

</div>

</div>

---

# Invited Talks

{% for talk in site.data.talks limit:4 %}

<div class="talk-card">

## {{ talk.title }}

**{{ talk.organization }}**

{{ talk.event }}

{{ talk.date }}

</div>

{% endfor %}

<p align="center">

<a href="/talks/" class="btn">

View All Talks

</a>

</p>

---

# Awards & Achievements

<ul class="awards">

<li>🏅 UGC-NET Junior Research Fellowship</li>

<li>🥇 Gold Medal – M.Sc. Information Technology</li>

<li>🏆 GATE Computer Science (2024)</li>

<li>🏆 GATE Data Science & Artificial Intelligence (2024)</li>

</ul>

---

# Latest News

<div class="timeline">

<div class="timeline-item">

### 2026

Publication in *Quantum Information Processing*

</div>

<div class="timeline-item">

### 2026

Invited Talk at RNS Institute of Technology

</div>

<div class="timeline-item">

### 2026

BlindTranspiler released as an open-source project

</div>

<div class="timeline-item">

### 2026

Publication in *Physica Scripta*

</div>

</div>

---

# Contact

**Email**

joshi.mohit1221@gmail.com

**GitHub**

https://github.com/joshiCoding

**Website**

https://joshicoding.in

**Location**

Department of Computer Science

Banaras Hindu University

Varanasi, India
