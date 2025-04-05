---
title: "Error bounds for stochastic user equilibrium traffic assignment"

# Authors
authors:
  - admin
  - Stephen Boyles

# Author notes (optional)
# author_notes:
#   - 'Equal contribution'
#   - 'Equal contribution'

date: '2025-06-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2025-04-04T00:00:00Z'

# Publication type.
publication_types: ['working-paper']

# Publication name and optional abbreviated publication name.
publication: This work is a part of my MS theis and have been presented in the following conferences:<br> 1) *12th Triennial Symposium on Transportation Analysis (TRISTAN XII), Okinawa, Japan.*<br> 2) *INFORMS Annual Meeting 2024 (TSL invited session), Indianapolis, USA*
# publication_short: In *TRISTAN XII*

abstract: In stochastic user equilibrium traffic assignment, we develop bounds on the distance between a given feasible solution and the equilibrium solution in terms of a gap function.  The intent is to provide guidance on termination criteria to reduce run times, which is important because this assignment problem is often a subproblem to a more complex bilevel optimization.  These mathematical bounds complement existing rules-of-thumb drawn empirically from numerical case studies.  Our approach is based on Taylor's theorem, as applied to the fixed-point formulation of the stochastic user equilibrium assignment, and provides upper bounds on differences in both aggregate metrics (total travel time, distance traveled) and disaggregate metrics (link flows, path flows).  We demonstrate that these bounds are tight and cannot be further improved without additional restrictions on the network topology or problem instance.


# Summary. An optional shortened abstract.
# summary: 


tags:
  - Traffic Assignment

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: 'https://github.com/debojjalb/SUE_Bounds'
#url_dataset: 'https://github.com/HugoBlox/hugo-blox-builder'
#url_poster: ''
#url_project: ''
#url_slides: ''
#url_source: 'https://github.com/HugoBlox/hugo-blox-builder'
#url_video: 'https://youtube.com'

# Featured image
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
# projects:
#   - example

# Slides (optional).
# slides: example
---

{{% callout note %}}
The codebase and conference extended abstract is available on the buttons above article.
{{% /callout %}}

In stochastic user equilibrium traffic assignment, we derive bounds on the distance between a given feasible solution and the equilibrium solution. The intent is to provide guidance on termination criteria to reduce runtimes, which is important because the traffic assignment problem is often a subproblem of a more complex bilevel optimization.  These mathematical bounds complement existing rules of thumb drawn empirically from numerical case studies.  

Our approach is based on Taylor's theorem, applied to the fixed-point formulation of the stochastic user equilibrium assignment, and provides upper bounds on differences in both aggregate metrics (average link travel cost, total system travel time) and disaggregate metrics (link flows, path flows). We demonstrate that the proposed path flow, link flow, and travel cost bounds are tight and cannot be further improved without additional restrictions on the network topology or problem instance.

Results on city-level networks indicate that the bounds on path flows are reasonably tight, with the absolute difference between the derived bound and actual value often in the order of $10^{-1}$. We study the tradeoff between the distance from equilibrium—where the bound becomes applicable—and its tightness. Detailed results guide the choice of a parameter that yields the tightest possible bound for a given distance from equilibrium. Empirical evidence shows that the bound on the distance between any feasible path flow and the equilibrium flow exhibits a near-linear rate of convergence close to equilibrium. This convergence rate is found to be close to $0.9$, consistent across all tested networks.

Finally, we demonstrate the practical utility of the derived bounds in a simple network design problem to find optimal link closures. By enumerating the complete feasible set, we show a 36\% improvement in computation time on the Sioux Falls network when using the derived bounds, compared to not using them.

{{% callout note %}}
Click the _Cite_ button above to cite this article.
{{% /callout %}}

