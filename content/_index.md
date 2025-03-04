---
# Leave the homepage title empty to use the site title
title:
date: 2025-02-06
type: landing

sections:
  - block: hero
    design:
      columns: '1'  # ✅ 确保整个 hero 模块是一个整体
    content:
      title: ""  # 避免默认标题
      custom_html: |
        <div style="display: flex; flex-direction: column; justify-content: center; align-items: center; width: 100%; max-width: 1100px; margin: 0 auto; text-align: center;">

          <div style="display: flex; justify-content: center; align-items: center; gap: 30px; flex-wrap: wrap;">
          
            <a href="https://www.sigs.tsinghua.edu.cn/" target="_blank">
              <img src="media/Tsinghua-SIGS-logo.png" alt="Tsinghua University Logo"
                   style="height: 100px; max-width: 100%; border-radius: 10px;">
            </a>

        
            <img src="media/Intro.png" alt="Intro Image"
                 style="height: 100px; max-width: 100%; border-radius: 10px;">
          </div>

          <div style="margin-top: 20px; max-width: 800px;">
            <p style="font-size: 16px; line-height: 1.6;">
              We are a research group at <strong>Institute of Data and Information, Tsinghua Shenzhen International Graduate School.</strong>
              Our team is led by <strong>Dr. Kaichen Dong</strong>. Our group focuses on research topics related to
              <strong>Temperature-adaptive Radiative Cooling, Moiré Photonics, Metamaterials/Metasurfaces, Zero-power Smart MEMS Sensors, and AI for Science</strong>.
              <br>
              <a href="{{ "/publication/" | absURL }}" style="font-weight: bold; color: #0056b3; text-decoration: none;">(see publications →)</a>
            </p>
          </div>

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
      css_class: small-text  # ✅ 让 Latest Preprints 字体变小 (14px)

  - block: markdown
    content:
      title:
      text: |
        {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
    design:
      columns: '1'
---
