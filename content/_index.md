---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: 'My Research'
      subtitle: ''
      text: |-
        My work centers on three interconnected domains: **trucking infrastructure**, **port–hinterland systems**, and **traffic assignment modeling**. Within these areas, I use operations research techniques and data-driven methods to study and improve multimodal freight and logistics networks.
        
        I am particularly interested in how ports connect to their hinterlands and how bottlenecks in one component ripple across the system. My focus includes capacity measurement, anchorage and terminal queues, resilience during disruptions, re-routing, and the interaction of waterside, terminal, and landside operations. I am also drawn to questions of data quality and integration, as well as economic and policy aspects such as port pricing, demurrage, environmental costs, and the safety and sustainability of large-scale multimodal freight systems.

        **Primary Focus:** Maritime Logistics, Trucking Logistics, Traffic Assignment, Port Operations, Multimodal Freight Networks
        
        **Allied Focus:** Operations Research, Queueing Theory, Discrete Event Simulation, Stochastic User Equilibrium, Network Optimization, Data-Driven Methods

        Beyond publications, I am a strong advocate of open source research and strive to release large-scale frameworks along with documentation for community use.
        
        [**To know more, view my research page →**](https://debojjalb.github.io/research/)
        
        Please reach out to collaborate 😃
    design:
      columns: '1'
      background:
        color: '#e8f5e8'  # Light green background
      text_color_light: false
      css_style: |
        .block-markdown h2 {
          color: #2e7d2e !important;
        }
        .block-markdown strong {
          color: #2e7d2e !important;
        }
        .block-markdown a {
          color: #2e7d2e !important;
          font-weight: bold;
        }
  # - block: collection
  #   id: papers
  #   content:
  #     title: Featured Research
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #     count: 3

  #   design:
  #     view: article-grid
  #     columns: 3
  # - block: collection
  #   content:
  #     title: Recent Conferences and Publications
  #     text: ""
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 3
  - block: markdown
    id: recent-updates
    content:
      title: 'Recent Updates'
      subtitle: ''
      text: |-
        [**For more details and pictures, see my travel page →**](https://debojjalb.github.io/travel/)

        **Sep, 2025:** I will presenting our work on "A framework for measuring maritime port system capacities with limited input data" at INFORMS Annual Meeting 2025 in Atlanta (2:45-4:00 PM, TSL invited session on Network Design).

        **Sep 2025:** I have been appointed as Member of the TRB Standing Committee on Intermodal Freight and Truck Transportation for the 2025–2028 term. I aim to contrinute to the committee on multimodal port operations, capacity, and resilience. [More details here](https://www.linkedin.com/posts/debojjal-bagchi_excited-to-share-that-following-the-recent-activity-7365922069374537730-Qcfo?utm_source=share&utm_medium=member_desktop&rcm=ACoAAB-24_ABlBO97b8VIUpjxdDlIw_oB4ljeX8)
        
        **July 2025:** I presented master's thesis on Error Bounds for Stochastic User Equilibrium Traffic Assignment at TRISTAN XII in Okinawa, Japan, focusing on early termination criteria for stochastic traffic assignment problems. [More details here](https://www.linkedin.com/posts/debojjal-bagchi_presented-my-masters-thesis-link-in-comments-activity-7351498036625219584-FcWJ?utm_source=share&utm_medium=member_desktop&rcm=ACoAAB-24_ABlBO97b8VIUpjxdDlIw_oB4ljeX8)
        
        **Apr 2025:** Our paper was accepted at [DTA 2025](https://www.motusanimi.it/dta-abstracts/) in Salerno, Italy on localized queue spillback with uncertain demand.
        
        **Apr 2025:** Our manuscript on bi-criterion Steiner TSP for last-mile electric vehicle logistics to Computers & Operations Research. [A preprint is available here](https://arxiv.org/abs/2409.14848)

      columns: '1'
      spacing:
        padding: ["15px", "10px", "15px", "10px"]
      background:
        color: '#f8f9fa'
      text_color_light: false
      css_style: |
        .block-markdown {
          max-width: 100% !important;
          margin: 0 !important;
        }
        .block-markdown .container {
          max-width: 100% !important;
          padding: 0 !important;
        }
        .block-markdown h2 {
          color: #2c3e50 !important;
          font-weight: 600 !important;
          font-size: 1.5rem !important;
          margin-bottom: 0.8rem !important;
        }
        .block-markdown p {
          margin-bottom: 0.4rem !important;
          line-height: 1.4 !important;
          font-size: 0.95rem !important;
          color: #4a5568 !important;
        }
        .block-markdown strong {
          color: #2d3748 !important;
          font-weight: 600 !important;
        }
        .block-markdown a {
          color: #3182ce !important;
          text-decoration: none !important;
          font-weight: 500 !important;
        }
        .block-markdown a:hover {
          color: #2c5aa0 !important;
          text-decoration: underline !important;
        }
        .block-markdown p:first-of-type {
          margin-bottom: 0.8rem !important;
          padding-bottom: 0.5rem !important;
          border-bottom: 1px solid #e2e8f0 !important;
        }
  # - block: cta-card
  #   demo: true # Only display this section in the Hugo Blox Builder demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!
        
  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
    # design:
    #   card:
    #     # Card background color (CSS class)
    #     css_class: "bg-primary-700"
    #     css_style: ""
---
