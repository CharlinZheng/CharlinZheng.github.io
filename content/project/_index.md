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
        - name: Other
          tag: Demo
    design:
      columns: '1'
      view: masonry
      flip_alt_rows: true
      background: {color: '#d4d9dfff', image_parallax: true}
      spacing: {padding: [0, 2, 0, 2]}
  - block: tag_cloud
    content:
      title: Research Tags
      subtitle: ''
      text: Please select tags of interest to view related publications!
      # Choose a taxonomy from the `taxonomies` list in `config.yaml` to display (e.g. tags, categories, authors)
      taxonomy: tags
      # Choose how many tags you would like to display (0 = all tags)
      count: 20
    design:
      # Minimum and maximum font sizes (1.0 = 100%).
      font_size_min: 0.7
      font_size_max: 2.0
---
