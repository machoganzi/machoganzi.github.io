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
      title: '📚 My Research'
      subtitle: ''
      text: |-
        
        I am researching and studying web service design and database.

        We are planning various projects using this.

        Please contact me for a collaboration 😃
        
    design:
      columns: '1'

  # 슬라이더 블록 (shortcode 사용)
  - block: custom_slider
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
        - title: ""
          content: ""
          align: ""
          background:
            image:
              filename: ""
              filters:
                brightness: 
            position: ""
            color: ""
    design:
      slide_height: ""
      slide_width: ""
      loop: 
      interval: 

  - block: collection
    id: papers
    content:
      title: 📅 Planned Move 📅
      filters:
        folders:
          - planned
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    id: talks
    content:
      title: 💫 동아리 💫
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 4
     
  - block: collection
    id: blog
    content:
      title: 😁 My Blog 😁
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
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
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]

  - block: cta-card
    demo: false # 데모 모드가 아닌 실제 사이트에 표시
    content:
      title: 🚀 Explore My Projects
      text: |-
        Interested in seeing the projects I have worked on over the years? Feel free to check out my portfolio of various web development, design, and academic projects.

        If you'd like to know more, don't hesitate to reach out to me!

      button:
        text: View Projects
        url: projects/  # 프로젝트 목록 페이지로 링크
    design:
      card:
        css_class: ""
        css_style: ""  # 카드 배경 및 텍스트 스타일 설정

---
