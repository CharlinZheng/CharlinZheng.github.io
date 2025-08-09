---
# Leave the homepage title empty to use the site title
title: Research
date: 2022-10-24
type: landing

sections:
  - block: hero
    content:
      title: |
        Research Goal
      image:
        filename: Web_HomePage.svg
      text: |
        <br>
        
        The **Wowchemy Research Group** has been a center of excellence for Artificial Intelligence research, teaching, and practice since its founding in 2016.
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
      text: |-
        The transition is powered by the synergy of **Machine Learning**, **Computational Engineering**, and **Electrical Engineering**. Key technologies include neural networks, physics-informed models, reinforcement learning, numerical and parallel computing, embedded computing, and real-time operating systems. Applications span high-frequency power converters, inverter control, and power system stability enhancement.
    design:
      # Choose an optional background color, gradient, image, or video
      background:
        gradient_end: '#f7f7f7'
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



---