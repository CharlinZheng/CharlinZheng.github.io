---
title: Home
type: landing
sections:
  - block: portfolio
    id: projects
    content:
      title: Projects
      subtitle: Check out my projects below.
      text: 
      filters:
        folders: 
         - project
        tags: []             # 只显示哪些 tag（留空表示不过滤）
        exclude_tags: []     # 排除哪些 tag
        kinds: 
         - page       # 保持默认即可
      sort_by: 'Date'
      sort_ascending: false
      default_button_index: 0
      buttons:
        - name: All
          tag: '*'
        - name: Machine Learning
          tag: ML
        - name: Cyber-Physical Systems
          tag: CPS
        - name: Hybrid Dynamics Modeling
          tag: Modeling
          tag: Sim
        - name: High Frequency Control
          tag: Control
        - name: Edge Computing
          tag: Edge
        - name: Other
          tag: Demo
    design:
      columns: '1'
      view: masonry
      flip_alt_rows: true
      background: {color: '#d4d9dfff', image_parallax: true}
      spacing: {padding: [0, 2, 0, 2]}
  
---
