---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: slider
    content:
      slides:
      - title: 👋 Welcome to the Jialin research website
        content: Take a look at what we're working on...
        align: center
        background:
          image:
            filename: pcb.jpg
            filters:
              brightness: 0.4
          position: right
          color: '#666'
      - title: Lunch & Learn ☕️
        content: 'Share your knowledge with the group and explore exciting new topics together!'
        align: left
        background:
          image:
            filename: contact.jpg
            filters:
              brightness: 0.7
          position: center
          color: '#555'
      - title: World-Class Semiconductor Lab
        content: 'Just opened last month!'
        align: right
        background:
          image:
            filename: welcome.jpg
            filters:
              brightness: 0.5
          position: center
          color: '#333'
        link:
          icon: graduation-cap
          icon_pack: fas
          text: Join Us
          url: ../contact/
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: ''
      is_fullscreen: true
      # Automatically transition through slides?
      loop: false
      # Duration of transition between slides (in ms)
      interval: 2000
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
    
  - block: markdown
    content:
      title: ""
      text: |-
        <div style="display:flex;justify-content:space-around;flex-wrap:wrap;background-color:#f8f9fa;padding:2rem 1rem;border-radius:0.75rem;text-align:center;">
          <div style="flex:1 1 200px;margin:1rem;">
            <div style="font-size:2rem;font-weight:700;">1M+</div>
            <div>Websites built<br>with Hugo Blox</div>
          </div>
          <div style="flex:1 1 200px;margin:1rem;">
            <div style="font-size:2rem;font-weight:700;">10k+</div>
            <div>GitHub stars<br>since 2016</div>
          </div>
          <div style="flex:1 1 200px;margin:1rem;">
            <div style="font-size:2rem;font-weight:700;">3k+</div>
            <div>Discord community<br>for support</div>
          </div>
        </div>
    design:
     background:
      image:
        filename: bg-hue.svg   # 图片放在 assets/media/bg-hue.svg
        size: cover
        position: center
        filters:
          brightness: 1.0
          contrast: 1.0
---


