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
        - text: Projects
          url: "#projects"
          icon: arrow-down
        - text: Experience
          url: "#experience"
          icon: briefcase
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
      title: "Projects and Experiments"
      subtitle: "Robotics, perception, control, and data-driven systems work I have built and learned from"
      count: 0
      filters:
        folders:
          - projects
      sort_by: Weight
      sort_ascending: true
      buttons:
        - name: Featured
          tag: featured
        - name: Robotics
          tag: robotics
        - name: Computer Vision
          tag: computer-vision
        - name: Machine Learning
          tag: machine-learning
        - name: All
          tag: '*'
      default_button_index: 0
    design:
      columns: 3
      spacing:
        padding: ["3rem", "0", "3rem", "0"]

  # Experience
  - block: job-experience
    id: experience
    content:
      username: me
      title: "Experience"
      subtitle: "Selected engineering work behind the robotics, data, and learning systems projects."
    design:
      spacing:
        padding: ["2rem", "0", "3rem", "0"]

  # Publications and reports
  - block: collection
    id: publications
    content:
      title: Research & Reports
      subtitle: 'Thesis material, reports, and technical notes'
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


  # Contact
  - block: contact-info
    id: contact
    content:
      title: Get In Touch
      subtitle: ""
      text: |-
        Reach out if you want to talk about anything you found interesting on this page.
      email: joost@leliveld.us
      autolink: true
    design:
      columns: '1'
      spacing:
        padding: ["3rem", "0", "4rem", "0"]
---
