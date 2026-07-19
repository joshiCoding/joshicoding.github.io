---
layout: default
title: Research
permalink: /research/
---

# Research

My research lies at the intersection of **Quantum Computing**, **Cryptography**, and **Secure Delegated Computing**. My primary goal is to develop practical and resource-efficient protocols that enable secure quantum computation on remote quantum computers while preserving the privacy of users' data, algorithms, and computation.

---

# Research Interests

<div class="card-grid">

<div class="card">

## Blind Quantum Computation

Design and analysis of information-theoretically secure protocols that allow a client with limited quantum capabilities to delegate computations to a remote quantum server without revealing the computation or data.

</div>

<div class="card">

## Quantum Cryptography

Development of secure quantum communication protocols, quantum key distribution, delegated quantum computation, and privacy-preserving quantum protocols.

</div>

<div class="card">

## Quantum Homomorphic Encryption

Construction of encryption techniques that enable computation directly on encrypted quantum data while maintaining confidentiality throughout the computation.

</div>

<div class="card">

## Quantum Algorithms

Design and optimization of quantum algorithms with emphasis on Grover's Search Algorithm, Quantum Fourier Transform, and algorithms for practical quantum applications.

</div>

<div class="card">

## Quantum Searchable Encryption

Application of blind quantum computation techniques to searchable encryption, enabling secure cloud-based data retrieval with quantum speedup.

</div>

<div class="card">

## NISQ Computing

Performance analysis of quantum algorithms under realistic hardware constraints including noise models, connectivity limitations, and resource estimation.

</div>

</div>

---

# Current Research

## Secure Delegated Quantum Computing

My doctoral research focuses on designing universal protocols for secure delegated quantum computation using arbitrary rotation gates. The objective is to reduce computational and communication overhead while maintaining information-theoretic security.

Current directions include:

- Universal Blind Quantum Computation
- Recursive Arbitrary Rotation Gates
- Quantum Homomorphic Encryption
- Secure Delegated Quantum Computing
- Resource Optimization
- Blind Quantum Circuit Compilation

---

# Research Contributions

### Universal Blind Quantum Computation

Development of recursive techniques for implementing arbitrary rotation gates in blind quantum computation with significantly improved resource efficiency.

---

### BlindTranspiler

Development of **BlindTranspiler**, an open-source software framework for converting standard Qiskit quantum circuits into blind quantum circuits supporting multiple secure delegated quantum computation protocols.

<div style="margin-top:20px;">

<a class="btn" href="https://github.com/joshiCoding/blind_transpiler">

GitHub Repository

</a>

<a class="btn" href="https://joshicoding.in/blind_transpiler/">

Documentation

</a>

</div>

---

# Research Timeline

| Year | Milestone |
|------|-----------|
| 2022 | Started Ph.D. at Banaras Hindu University |
| 2022 | First publication on Blind Quantum Computation |
| 2024 | Quantum Searchable Encryption and NISQ resource estimation |
| 2025 | Research on arbitrary rotation gates and encrypted quantum computation |
| 2026 | Universal Blind Quantum Computation and BlindTranspiler software |

---

# Research Collaborations

I am interested in collaborations in the following areas:

- Blind Quantum Computation
- Quantum Cryptography
- Quantum Software Engineering
- Secure Delegated Quantum Computing
- Quantum Algorithms
- Quantum Machine Learning
- Quantum Networks

Researchers and students interested in collaboration are welcome to contact me.

---

# Research Vision

Future fault-tolerant quantum computers will likely be accessed through cloud services. My long-term research vision is to make cloud quantum computing **private, secure, and practical** by developing efficient cryptographic protocols that protect users' computations without sacrificing performance.

The combination of Blind Quantum Computation, Quantum Homomorphic Encryption, and Quantum Cryptography has the potential to become the foundation of secure quantum cloud computing.

---

# Selected Publications

{% assign featured = site.data.publications | where:"featured",true %}

{% for paper in featured %}

<div class="publication-card">

### {{ paper.title }}

**{{ paper.journal }} ({{ paper.year }})**

{{ paper.authors }}

<div class="paper-links">

{% if paper.pdf != "" %}
<a class="btn-small" href="{{ paper.pdf }}">PDF</a>
{% endif %}

{% if paper.doi != "" %}
<a class="btn-small" href="{{ paper.doi }}">DOI</a>
{% endif %}

</div>

</div>

{% endfor %}

<div style="text-align:center;margin-top:40px;">

<a class="btn" href="/publications/">

View Complete Publication List

</a>

</div>