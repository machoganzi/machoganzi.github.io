---
title: '경력'
date: 2023-10-24
type: landing

design:
  spacing: '5rem'

# 참고: `username`은 `content/authors/` 폴더 내 사용자의 폴더 이름을 의미합니다.

# 페이지 섹션
sections:
  - block: resume-experience
    content:
      username: admin
    design:
      # Hugo 날짜 형식
      date_format: '2006년 1월'
      # 학력 또는 경력을 먼저 표시할까요?
      is_education_first: false
  - block: resume-skills
    content:
      title: 기술 및 취미 🎨
      username: admin
    design:
      show_skill_percentage: false
  - block: resume-awards
    content:
      title: 수상 내역 🏆
      username: admin
  - block: resume-languages
    content:
      title: 언어 🌍
      username: admin
---
