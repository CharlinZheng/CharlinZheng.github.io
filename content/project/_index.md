---
title: Projects
view: showcase

# Optional header image (relative to `assets/media/` folder)
banner:
  caption: ''
  image: ''

# Showcase
sections:
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # 默认过滤器按钮
      default_button_index: 0
      # 过滤器按钮
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # 选择展示多少列（1-3）
      columns: '3'
      # 切换不同的视图模式
      view: showcase
      # 对于展示视图，在鼠标悬停时翻转卡片？
      flip_alt_rows: false
---