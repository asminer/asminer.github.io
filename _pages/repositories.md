---
layout: page
permalink: /repositories/
title: Software
description: Summary of software tools that I manage
nav: true
nav_order: 3
---

----
## SMART

SMART, or *Stochastic Model-checking Analyzer for Reliability and Timing*,
is an open-source software package for analyzing discrete-state models.
Models may be specified either directly at a low level
(e.g., as a finite state machine or Markov chain),
or using a high-level formalism (e.g., as a Petri net).
Analysis engines include CTL model checking and
computation of performance measures.

----
## MEDDLY

MEDDLY, or *Multi-terminal and Edge-valued Decision Diagram LibrarY*,
is an open-source software library for decision diagrams.
It is written in C++ and has been integrated into several tools,
including the new version of SMART.
It supports binary and multi-valued decision diagrams,
and edge-valued decision diagrams.


{% if site.data.repositories.github_repos %}

----
## GitHub Repositories

<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.liquid repository=repo %}
  {% endfor %}
</div>
{% endif %}
