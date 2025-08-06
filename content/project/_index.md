---
title: Home
type: landing
sections:
  - block: portfolio
    id: project
    content:
      title: Projects
      subtitle: My subtitle
      text: Add any **markdown** content here.
      filters:
        folders: 
         -project
        tags: []             # 只显示哪些 tag（留空表示不过滤）
        exclude_tags: []     # 排除哪些 tag
        kinds: 
         -page       # 保持默认即可
      sort_by: 'Date'
      sort_ascending: false
      default_button_index: 0
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      columns: '1'           # '1' 或 '2'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
---
