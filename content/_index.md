---
# Leave the homepage title empty to use the site title
title:
date: 2025-02-06
type: landing

sections:
  - block: hero
    design:
      columns: '1'  # ✅ 让整个 hero 部分居中
    content:
      title: ""  # 避免默认标题
      text: |
        <div style="display: flex; flex-direction: column; align-items: center; text-align: center; width: 100%;">

          <!-- Logo -->
          <a href="https://www.sigs.tsinghua.edu.cn/" target="_blank">
            <img src="media/Tsinghua-SIGS-logo.png" alt="Tsinghua University Logo"
                 style="height: 120px; max-width: 100%; margin-bottom: 10px;">
          </a>

          <!-- 介绍文本 -->
          <p style="font-size: 14px; line-height: 1.5; max-width: 800px;">
            We are a research group at <strong>Institute of Data and Information, Tsinghua Shenzhen International Graduate School.</strong>
            Our team is led by <strong>Dr. Kaichen Dong</strong>. Our group focuses on research topics related to
            <strong>Temperature-adaptive Radiative Cooling, Moiré Photonics, Metamaterials/Metasurfaces, Zero-power Smart MEMS Sensors, and AI for Science</strong>
          </p>

          <!-- Intro 图片 -->
          <img src="media/Intro.png" alt="Intro Image"
               style="max-height: 200px; max-width: 100%; border-radius: 10px; margin-top: 10px;">
        </div>

  - block: collection
    content:
      title: Latest News
      count: 5
      filters:
        category: ''
        exclude_featured: false
        publication_type: ''
        tag: ''
      order: desc
      page_type: post
    design:
      view: compact  # ✅ 改用 compact 视图，去除超链接
      columns: '1'
      css_class: small-news-text  # ✅ 设定 CSS 类，便于调整字体和图片大小

  - block: collection
    content:
      title: Latest Preprints
      count: 5
      filters:
        folders:
          - publication
        publication_type: 'article'
    design:
      view: citation
      columns: '1'
      css_class: small-text

  - block: markdown
    content:
      title:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
