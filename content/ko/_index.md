---
# 홈페이지 제목을 비워두면 사이트 제목을 사용
title: ""
date: 2022-10-24
type: landing

design:
  # 기본 섹션 간격 설정
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # 표시할 사용자 프로필 선택 ( `content/authors/` 내 폴더 이름)
      username: admin
      text: ""
      # 바이오그래피 아래에 콜투액션 버튼을 표시할까요? (선택 사항)
      button:
        text: 이력서 다운로드
        url: /uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # `assets/media/`에 이미지 배경 추가
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  - block: markdown
    content:
      title: '📚 나의 관심사 📚'
      subtitle: ''
      text: |-
        저는 웹 서비스 디자인과 데이터베이스에 대한 연구를 진행하고 있습니다 현재 집중하고 있습니다.  
        이를 바탕으로 여러 가지 프로젝트를 기획하고 있으며, 협업을 통해 더 나은 결과물을 만들어내고 싶습니다.  
        협업에 관심이 있으시다면 언제든지 연락 주세요! 😃
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
        - title: "프로젝트 1"
          content: "웹 서비스 개발 프로젝트"
          align: "center"
          background:
            image:
              filename: "project1.png"
              filters:
                brightness: 1.0
            position: "center"
            color: "#fff"
        - title: "프로젝트 2"
          content: "모바일 앱 개발 프로젝트"
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
      title: 📅 향후 계획 📅
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
      title: 💫 동아리 활동 💫
      filters:
        folders:
          - dongari
    design:
      view: article-grid
      columns: 4
     
  - block: collection
    id: blog
    content:
      title: 😁 나의 블로그 😁
      subtitle: '여러 가지 흥미로운 주제에 대한 글을 작성합니다.'
      text: '프로그래밍, 웹 서비스 디자인, 그리고 개인적인 관심사에 대해 정리하고 공유하는 공간입니다.'
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
      title: 🚀 나의 프로젝트를 확인해 보세요
      text: |-
        지금까지 제가 작업한 다양한 프로젝트에 관심이 있으신가요?  
        웹 개발, 디자인, 학문적 프로젝트 등 여러 분야에서의 작업물을 포트폴리오에서 확인하실 수 있습니다.  
        더 알고 싶다면 언제든지 저에게 연락해 주세요!
      button:
        text: 프로젝트 보기
        url: projects/
    design:
      card:
        css_class: ""
        css_style: ""
---
