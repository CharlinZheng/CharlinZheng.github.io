---
title: Home
type: landing
sections:
  - block: portfolio
    id: projects
    content:
      title: Projects
      subtitle: My subtitle
      text: Add any **markdown** content here.
      filters:
        folders: [project]   # 从哪个内容类型读取，通常是 content/project/*
        tags: []             # 只显示哪些 tag（留空表示不过滤）
        exclude_tags: []     # 排除哪些 tag
        kinds: [page]        # 保持默认即可
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
      view: showcase         # masonry / showcase / compact / list 等
      flip_alt_rows: true   # showcase 视图下可交替反转布局
---
