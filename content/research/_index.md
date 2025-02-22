---
title: Research
type: landing
layout: landing
sections:
  - block: showcase
    id: research-areas
    content:
      title: "Our Research Directions"
      text: "We focus on multiple cutting-edge research areas."
      items: 
        {{ range .Pages }}
        - title: "{{ .Title }}"
          description: "{{ .Params.summary }}"
          image: "{{ .RelPermalink }}featured.jpg"
          external_link: "{{ .RelPermalink }}"
        {{ end }}
    design:
      view: showcase
      columns: 2
      flip_alt_rows: true
---
