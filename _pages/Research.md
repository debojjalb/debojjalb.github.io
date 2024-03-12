---
layout: archive
title: "Ongoing Research"
permalink: /research/
author_profile: true
---

<style>
    body {
        font-family: "Times New Roman", Times, serif;
        font-size: 14px;
        color: #000;
    }
    a {
        color: #014552; /* Dark blue color for links */
    }
    h1, h2, h3, h4, h5, h6 {
        margin-top: 24px;
        margin-bottom: 16px;
        font-weight: 600;
        line-height: 1.25;
    }
    ul, ol {
        margin-bottom: 10px; /* Adjust the bottom margin of lists */
    }
    li {
        margin-bottom: 5px; /* Adjust the bottom margin of list items */
    }
</style>

## Multi-Criterion Steiner Travelling Salesman Problem:
Bi-criterion tours which visit a set of terminals while minimizing distance and turns are ideal for logistics companies. These routes are fuel-efficient, environment-friendly, and safer since they avoid stopping at junctions. We proposed a new local search heuristic and compared its performance against an Integer Programming formulation. Current work includes developing a more sophisticated heuristic for the problem.

## Reverse Logistic Network Design for Circular Economy:
The research aims to find the optimal location and state (open / closed / whether expansion is needed) for wood waste recycling centres. The aim is to minimize the cost of the whole recycle process following several environmental, logistical, and demand constraints. A scenario-based Mixed Integer Linear Program was developed based on earlier studies. Further, an Adaptive Large Neighborhood Search based heuristic was proposed for the problem. Current work includes testing on real data from CRD industries in Quebec, Canada, and improving the neighborhoods.

<!-- {% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.research reversed %}
  {% include archive-single.html %}
{% endfor %} -->