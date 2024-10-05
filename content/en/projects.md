---
title: 'Projects'
date: 2024-05-19
type: landing
design:
  # Default section spacing
  spacing: '5rem'
  background:
        color: black
sections:
  - block: collection
    content:
      title: Selected Projects
      text: 
      filters:
        folders:
          - project
    design:
      view: article-grid
      fill_image: true
      columns: 3
      css_class: dark
      background:
        color: black
        image:
          filename: projectbackground.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
---