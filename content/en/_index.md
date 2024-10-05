---
# If the homepage title is empty, the site title will be used
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Select the user profile to display (folder name inside `content/authors/`)
      username: admin
      text: ""
      # Display a call-to-action button below the biography? (optional)
      button:
        text: Download Resume
        url: /uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add an image background in `assets/media/`
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: markdown
    content:
      title: '📚 My Interests 📚'
      subtitle: ''
      text: |-
        I am currently conducting research on web service design and databases.  
        Based on this, I am planning several projects and would like to collaborate to produce even better results.  
        Feel free to contact me if you're interested in collaborating! 😃
    design:
      columns: '1'

  # Slider block (using shortcode)
  - block: custom_slider1
    content:
      dir: "" 
      height: "" 
      width: "" 
      webp: 
      resize:  
      command: "" 
      option: "" 
      zoomable: 
      slides:
        - title: "Project 1"
          content: "Web service development project"
          align: "center"
          background:
            image:
              filename: "project1.png"
              filters:
                brightness: 1.0
            position: "center"
            color: "#fff"
        - title: "Project 2"
          content: "Mobile app development project"
          align: "center"
          background:
            image:
              filename: "project2.png"
              filters:
                brightness: 1.0
            position: "center"
            color: "#fff"
    design:
      slide_height: "500px"
      slide_width: "100%"
      loop: true
      interval: 5000

  - block: collection
    id: papers
    content:
      title: 📅 Future Plans 📅
      filters:
        folders:
          - planned
        featured_only: true
    design:
      view: article-grid
      columns: 3

  - block: collection
    id: talks
    content:
      title: 💫 Club Activities 💫
      filters:
        folders:
          - dongari
    design:
      view: article-grid
      columns: 4
     
  - block: collection
    id: blog
    content:
      title: 😁 My Blog 😁
      subtitle: 'I write about various interesting topics.'
      text: 'This is a space where I organize and share my thoughts on programming, web service design, and personal interests.'
      page_type: post
      count: 5
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      offset: 0
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]

  - block: cta-card
    demo: false
    content:
      title: 🚀 Check Out My Projects
      text: |-
        Interested in the various projects I've worked on?  
        From web development and design to academic projects, you can find my work in my portfolio.  
        Feel free to contact me if you'd like to know more!
      button:
        text: View Projects
        url: projects/
    design:
      card:
        css_class: ""
        css_style: ""
---
