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
          <img src="media/Tsinghua-SIGS-logo.png" alt="Tsinghua University Logo" height="50">
        </a>
      image:
        filename: Intro.png
      text: |
        <br>
        
        We are a research group at **Institute of Data and Information, Tsinghua Shenzhen International Graduate School.** Our team is led by **Dr. Kaichen Dong**. Our group focuses on research topics related to **Temperature-adaptive Radiative Cooling, Moiré Photonics, Metamaterials/Metasurfaces, Zero-power Smart MEMS Sensors, and AI for Science** (see publications).
    
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
      view: compact  # ✅ 改用 compact 视图，以便去除超链接
      columns: '1'
      css_class: small-news-text  # ✅ 设定 CSS 类，便于调整字体和图片大小

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
