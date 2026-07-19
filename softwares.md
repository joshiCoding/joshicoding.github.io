---
layout: default
title: Software
permalink: /software/
---

# Research Software

I develop open-source software to support research in **Quantum Computing**, **Blind Quantum Computation**, **Quantum Homomorphic Encryption**, and **Secure Delegated Quantum Computing**. My software aims to bridge the gap between theoretical cryptographic protocols and practical implementations using modern quantum programming frameworks.

---

# Featured Project

<div class="software-hero">

## BlindTranspiler

**BlindTranspiler** is an open-source Python framework that automatically converts standard quantum circuits into secure delegated quantum computation circuits.

It provides a unified interface for multiple secure delegated quantum computing protocols while integrating seamlessly with **Qiskit**.

<div class="software-buttons">

<a class="btn" href="https://github.com/joshiCoding/blind_transpiler">
GitHub Repository
</a>

<a class="btn" href="https://joshicoding.in/blind_transpiler/">
Documentation
</a>

<a class="btn" href="https://zenodo.org/doi/10.5281/zenodo.21437379">
Zenodo
</a>

</div>

</div>

---

# Features

<div class="card-grid">

<div class="card">

## Universal Blind Quantum Computation

Implements secure delegated quantum computation using recursive arbitrary rotation gates.

</div>

<div class="card">

## Quantum Homomorphic Encryption

Supports execution of quantum circuits directly on encrypted quantum data.

</div>

<div class="card">

## Qiskit Integration

Works directly with Qiskit circuits without requiring modifications to existing quantum programs.

</div>

<div class="card">

## Automatic Circuit Translation

Transforms standard quantum circuits into blind quantum circuits automatically.

</div>

<div class="card">

## Multiple Protocols

Supports UBQC, FDQC, SSDQC, and Quantum Homomorphic Encryption.

</div>

<div class="card">

## Open Source

Released under the Apache 2.0 License and available on GitHub.

</div>

</div>

---

# Installation

```bash
pip install blind-transpiler
```

or install the latest development version:

```bash
git clone https://github.com/joshiCoding/blind_transpiler.git

cd blind_transpiler

pip install -e .
```

---

# Example

```python
from blind_transpiler import BlindTranspiler

transpiler = BlindTranspiler(protocol="ubqc")

blind_circuit = transpiler.transpile(circuit)
```

---

# Software Architecture

The package consists of several major modules:

- Controllers
- Translators
- Blind Quantum Protocols
- Homomorphic Encryption
- Universal Blind Quantum Computation
- Utility Functions

The modular architecture allows researchers to easily extend the framework with new secure delegated quantum computation protocols.

---

# Applications

BlindTranspiler can be used in research involving:

- Blind Quantum Computation
- Secure Delegated Quantum Computing
- Quantum Homomorphic Encryption
- Quantum Searchable Encryption
- Quantum Cloud Computing
- Resource Estimation
- Quantum Compiler Research
- Quantum Cryptography

---

# Publications

The following publications describe the theory behind BlindTranspiler.

{% assign featured = site.data.publications | where:"featured",true %}

{% for paper in featured %}

<div class="publication-card">

### {{ paper.title }}

{{ paper.journal }}

({{ paper.year }})

<div class="paper-links">

{% if paper.pdf != "" %}
<a class="btn-small" href="{{ paper.pdf }}">
PDF
</a>
{% endif %}

{% if paper.doi != "" %}
<a class="btn-small" href="{{ paper.doi }}">
DOI
</a>
{% endif %}

</div>

</div>

{% endfor %}

---

# Development Roadmap

- Python Package (Completed)

- GitHub Repository (Completed)

- Documentation Website (Completed)

- Zenodo Archive (Completed)

- PyPI Release

- Benchmark Suite

- Verification Module

- IBM Quantum Runtime Integration

- PennyLane Backend

- Cirq Backend

---

# Contributing

Contributions from researchers, students, and developers are welcome.

If you are interested in extending BlindTranspiler or implementing new secure delegated quantum computation protocols, please feel free to open an issue or submit a pull request on GitHub.

---

# Citation

If you use BlindTranspiler in your research, please cite the associated journal publication.

<div style="text-align:center;margin-top:40px;">

<a class="btn" href="/publications/">

View Publications

</a>

</div>