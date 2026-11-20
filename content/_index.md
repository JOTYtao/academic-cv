---
title: ''
type: landing
sections:
  - block: resume-biography-3
    content:
      username: me
      button:
        text: Academic CV
        url: experience/
      headings:
        about: About me
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
  - block: markdown
    id: research-focus
    content:
      title: Research
      text: |
        I study how cloud evolution affects solar irradiance and how forecast uncertainty can inform power system operation. My work spans satellite-based intraday forecasting, probabilistic downscaling of weather predictions, and renewable generation scenarios for economic dispatch.

        [Research projects](research/)
  - block: collection
    id: papers
    content:
      title: Selected Research
      filters:
        folders: [publications]
        featured_only: true
    design:
      view: research-card
      columns: 2
  - block: collection
    id: other-papers
    content:
      title: More Publications
      filters:
        folders: [publications]
        exclude_featured: true
      count: 4
      text: '[Full publication list](publications/)'
    design:
      view: citation
---
