---
# Leave the homepage title empty to use the site title
title: ''
summary: 'Robotics, computer vision, and learning-based control work by Joost Leliveld.'
date: 2026-05-22
type: landing

sections:
  # Hero
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      show_status: true
      show_scroll_indicator: false
      typewriter:
        enable: false
      cta_buttons:
        - text: Robotics Work
          url: "#projects"
          icon: arrow-down
        - text: Contact
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      spacing:
        padding: ["3rem", "0", "2rem", "0"]

  # Projects
  - block: portfolio
    id: projects
    content:
      title: "Robotics Projects"
      subtitle: "External perception, autonomous navigation, and learning-based control"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
      default_button_index: 0
    design:
      columns: 3
      spacing:
        padding: ["3rem", "0", "3rem", "0"]

  # Publications and reports
  - block: collection
    id: publications
    content:
      title: Research & Reports
      subtitle: 'Theses, reports, and technical writeups'
      text: ''
      filters:
        folders:
          - publications
      count: 0
      order: desc
    design:
      view: citation
      columns: 1
      spacing:
        padding: ["3rem", "0", "3rem", "0"]

  # Blog
  - block: collection
    id: blog
    content:
      title: Notes
      subtitle: 'Short writeups from robotics, perception, and experiments'
      text: ''
      filters:
        folders:
          - blog
        exclude_featured: false
      count: 3
      order: desc
    design:
      view: card
      columns: 3
      spacing:
        padding: ["3rem", "0", "3rem", "0"]

  # Contact
  - block: contact-info
    id: contact
    content:
      title: Get In Touch
      subtitle: ""
      text: |-
        Reach out if you want to talk about robotics, computer vision, sensor fusion, or graduation-project work.
      email: j.j.p.leliveld@student.tue.nl
      autolink: true
    design:
      columns: '1'
      spacing:
        padding: ["3rem", "0", "4rem", "0"]
---
