---
layout: default
title: Invited Talks
permalink: /talks/
---

# Invited Talks & Workshops

I actively deliver invited lectures, workshops, and faculty development programs on **Quantum Computing**, **Quantum Cryptography**, **Blind Quantum Computation**, and related areas. My talks are aimed at introducing researchers, faculty members, and students to modern developments in quantum technologies while emphasizing practical implementation using Qiskit and current quantum hardware.

---

# Research Seminar Topics

<div class="card-grid">

<div class="card">

## Quantum Computing

Introduction to Quantum Computing, Quantum Gates, Quantum Circuits, Quantum Programming using Qiskit.

</div>

<div class="card">

## Blind Quantum Computation

Secure delegated quantum computation, information-theoretic security, client-server quantum protocols.

</div>

<div class="card">

## Quantum Cryptography

Quantum Key Distribution, Quantum Homomorphic Encryption, Secure Quantum Cloud Computing.

</div>

<div class="card">

## Quantum Algorithms

Grover's Algorithm, Quantum Fourier Transform, Shor's Algorithm, NISQ Computing.

</div>

</div>

---

# Invited Talks

{% assign sorted = site.data.talks | sort: "date" | reverse %}

{% for talk in sorted %}

<div class="publication-card">

<h2>{{ talk.title }}</h2>

<p>

<strong>Organization</strong><br>

{{ talk.organization }}

</p>

{% if talk.event != "" %}

<p>

<strong>Event</strong><br>

{{ talk.event }}

</p>

{% endif %}

<p>

<strong>Location</strong><br>

{{ talk.location }}

</p>

<p>

<strong>Date</strong><br>

{{ talk.date }}

{% if talk.end_date %}
– {{ talk.end_date }}
{% endif %}

</p>

<div class="paper-links">

{% if talk.slides != "" %}
<a class="btn-small" href="{{ talk.slides }}">
📑 Slides
</a>
{% endif %}

{% if talk.video != "" %}
<a class="btn-small" href="{{ talk.video }}">
🎥 Video
</a>
{% endif %}

</div>

</div>

{% endfor %}

---

# Areas of Expertise

I am available to deliver invited talks and workshops in the following areas:

- Quantum Computing
- Blind Quantum Computation
- Quantum Cryptography
- Quantum Algorithms
- Quantum Programming using Qiskit
- Secure Delegated Quantum Computing
- Quantum Homomorphic Encryption
- Quantum Searchable Encryption
- NISQ Computing

---

# Workshop Experience

My lectures generally include:

- Interactive presentations
- Mathematical foundations
- Live coding using Python & Qiskit
- IBM Quantum demonstrations
- Hands-on laboratory sessions
- Research paper discussions
- Open-source software demonstrations

---

# Previous Invited Institutions

- Banaras Hindu University
- RNS Institute of Technology
- Bapatla Engineering College
- QNepal Initiative
- SASTRA Deemed University

---

# Invitation

If your university, department, research group, or organization is interested in an invited lecture, workshop, faculty development program, or seminar on Quantum Computing or Quantum Cryptography, please feel free to contact me.

<div style="text-align:center;margin-top:40px;">

<a class="btn" href="/contact/">

Contact Me

</a>

</div>