---
# Leave the homepage title empty to use the site title
title: Research
date: 2022-10-24
type: landing

sections:

  - block: hero
    content:
      title: Research Goal
      image:
        # Reference an image in your `assets/media/` folder
        filename: Web_HomePage.svg
      # Add your Call-To-Action (CTA) button and optional icon
      cta:
        label: Get Started
        url: ../project/
        #icon_pack: fas
        #icon: download
      # Optionally, add an alternative CTA link
      cta_alt:
        label: See the Publications
        url: ../publication/
      # Optionally, add a note under the Call-To-Action          
      # Add your Hero text here
      text: |
        <br>
        My research focuses on the **digital transformation** of power electronics and energy systems. I aim to develop advanced control and optimization methods that enhance the efficiency, reliability, and sustainability of modern power systems.
    
    design:
      # Choose an optional background color, gradient, image, or video
      background:
        gradient_angle: 180
        gradient_end: '#e1e5faff'
        gradient_start: '#ffffffff'
        text_color_light: false
  - block: tag_cloud
    content:
      title: Research Tags
      subtitle: ''
      text: Please select tags of interest to view related publications!
      # Choose a taxonomy from the `taxonomies` list in `config.yaml` to display (e.g. tags, categories, authors)
      taxonomy: tags
      # Choose how many tags you would like to display (0 = all tags)
      count: 30
    design:
      # Minimum and maximum font sizes (1.0 = 100%).
      font_size_min: 0.7
      font_size_max: 2.0
      background:
        color: '#e1e5faff'



---