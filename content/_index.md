---
# Leave the homepage title empty to use the site title
title:
date: 2025-02-06
type: landing

sections:
  - block: hero
    content:
      title: |
        <a href="https://www.sigs.tsinghua.edu.cn/" target="_blank">
          <img src="media/Tsinghua-SIGS-logo.png" alt="Tsinghua University Logo" height="5">
        </a>
      image:
        filename: Intro.png
      text: |
        <br>
        
        We are a research group at **Institute of Data and Information, Tsinghua Shenzhen International Graduate School**.
    
  - block: collection
    content:
      title: Latest News
      subtitle:
      text:
      count: 5
      filters:
        author: ''
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      offset: 0
      order: desc
      page_type: post
    design:
      view: card
      columns: '1'
      css_class: small-news-text  # ✅ 添加自定义 CSS 类

  - block: collection
    content:
      title: Latest Preprints
      text: ""
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article'
    design:
      view: citation
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---

