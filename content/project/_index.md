---
title: Projects
type: landing

sections:
  - block: markdown
    content:
      title: Our Research Projects
      subtitle: ''
      text: ''
    design:
      columns: '1'
      
  - block: collection
    id: projects
    content:
      title: ''
      subtitle: ''
      text: ''
      # 选择要显示的页面类型
      page_type: project
      # 显示数量（0 = 全部）
      count: 0
      # 过滤器
      filters:
        folders:
          - project
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # 排序
      order: desc
      # 归档页面
      archive:
        enable: false
    design:
      # 选择视图类型
      # 可选: list, compact, card, citation, showcase
      view: card
      # 列数
      columns: '2'
---