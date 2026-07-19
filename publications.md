---
layout: default
title: Publications
permalink: /publications/
---

# Publications

My research focuses on **Blind Quantum Computation**, **Quantum Cryptography**, **Quantum Algorithms**, **Secure Delegated Quantum Computing**, and **Quantum Searchable Encryption**.

---

{% assign journals = site.data.publications | where: "type", "Journal" %}
{% assign conferences = site.data.publications | where: "type", "Conference" %}
{% assign books = site.data.publications | where: "type", "Book Chapter" %}

# Journal Articles

{% for paper in journals %}

<div class="publication-card">

<h2>{{ paper.title }}</h2>

<p>

<strong>Authors:</strong>

{{ paper.authors }}

</p>

<p>

<strong>Journal:</strong>

<i>{{ paper.journal }}</i>

({{ paper.year }})

</p>

{% if paper.volume %}
<p>

<strong>Volume:</strong>

{{ paper.volume }}

{% if paper.pages %}

&nbsp;&nbsp;

<strong>Pages:</strong>

{{ paper.pages }}

{% endif %}

</p>
{% endif %}

<p>

{% if paper.quartile %}
<span class="badge badge-blue">{{ paper.quartile }}</span>
{% endif %}

{% if paper.impact_factor %}
<span class="badge badge-green">
IF {{ paper.impact_factor }}
</span>
{% endif %}

</p>

<div class="paper-links">

{% if paper.pdf != "" %}
<a class="btn-small" href="{{ paper.pdf }}">
📄 PDF
</a>
{% endif %}

{% if paper.doi != "" %}
<a class="btn-small" target="_blank"
href="{{ paper.doi }}">
🔗 DOI
</a>
{% endif %}

</div>

</div>

{% endfor %}

---

# Conference Papers

{% for paper in conferences %}

<div class="publication-card">

<h2>{{ paper.title }}</h2>

<p>

<strong>Authors:</strong>

{{ paper.authors }}

</p>

<p>

<strong>Conference:</strong>

{{ paper.conference }}

({{ paper.year }})

</p>

{% if paper.publisher %}
<p>

<strong>Publisher:</strong>

{{ paper.publisher }}

</p>
{% endif %}

<div class="paper-links">

{% if paper.pdf != "" %}
<a class="btn-small" href="{{ paper.pdf }}">
📄 PDF
</a>
{% endif %}

{% if paper.doi != "" %}
<a class="btn-small"
href="{{ paper.doi }}">
🔗 DOI
</a>
{% endif %}

</div>

</div>

{% endfor %}

---

# Book Chapters

{% for paper in books %}

<div class="publication-card">

<h2>{{ paper.title }}</h2>

<p>

<strong>Authors:</strong>

{{ paper.authors }}

</p>

<p>

<strong>Book:</strong>

<i>{{ paper.book }}</i>

({{ paper.year }})

</p>

{% if paper.publisher %}
<p>

<strong>Publisher:</strong>

{{ paper.publisher }}

</p>
{% endif %}

{% if paper.pages %}
<p>

<strong>Pages:</strong>

{{ paper.pages }}

</p>
{% endif %}

<div class="paper-links">

{% if paper.pdf != "" %}
<a class="btn-small" href="{{ paper.pdf }}">
📄 PDF
</a>
{% endif %}

{% if paper.doi != "" %}
<a class="btn-small"
href="{{ paper.doi }}">
🔗 DOI
</a>
{% endif %}

</div>

</div>

{% endfor %}