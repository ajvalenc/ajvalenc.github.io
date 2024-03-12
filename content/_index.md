---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: collection
    id: posts
    content:
      title: Recent News
      subtitle: ''
      text: |-
        - **Jun 5, 2023:** New [paper](publication/rouhafzay-2023/) accepted at [SAS2023](https://2023.sensorapps.org/).
        - **Apr 17, 2023:** New [paper](publication/valencia-2023/) accepted at [CRV2023](https://www.computerrobotvision.org/2023/).
        - **Nov 23, 2020:** New [paper](publication/valencia-2020-a/) accepted in [Frontiers in Robotics and AI](https://www.frontiersin.org/journals/robotics-and-ai).
        - **Sep 17, 2020:** Two new [papers](publication/nadon-2020/) accepted at the [IROS](https://www.iros2020.org/) workshop on [RObotic MAnipulation of Deformable Objects](https://commandia.unizar.es/irosworkshop2020/).
        - **Jun 5, 2020:** [MASc Thesis](publication/valencia-2020/) approved with minor revisions.
        - **Aug 10, 2019**: New [paper](publication/valencia-2019/) accepted at [SENSORS2019](https://2019.ieee-sensorsconference.org/index.html).
        - **Nov 14, 2018**: New [paper](publication/nadon-2018/) accepted in [Robotics](https://www.mdpi.com/journal/robotics).
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: collection
    id: featured
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
      # Contact (add or remove contact options as necessary)
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
