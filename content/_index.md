---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: aboutme
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  - block: collection
    id: post
    content:
      title: Recent News
      count: 5
      filters:
        folders:
          - post
        exclude_featured: false
        exclude_future: false
        exclude_past: false
    design:
      view: compact
      columns: 2

  - block: collection
    id: event
    content:
      title: Recent & Upcoming Events
      filters:
        folders:
          - event
        exclude_future: false
        exclude_past: false
    design:
      view: article-grid
      columns: 2

  - block: hero
    id: research
    content:
      title: Research Goal
      image:
        # Reference an image in your `assets/media/` folder
        filename: Web_HomePage.svg
      # Add your Call-To-Action (CTA) button and optional icon
      cta:
        label: See the Publications
        url: publication
        #icon_pack: fas
        #icon: download
      # Optionally, add an alternative CTA link
      cta_alt:
        label: Detailed Experience
        url: experience
      # Optionally, add a note under the Call-To-Action          
      # Add your Hero text here
      text: |
        <br>
        My research focuses on the digital transformation of power electronics and energy systems. I aim to develop advanced control and optimization methods that enhance the efficiency, reliability, and sustainability of modern power systems.
        <br>
    design:
      # Choose an optional background color, gradient, image, or video
      background:
        gradient_angle: 180
        gradient_end: '#eaeaebff'
        gradient_start: '#ffffffff'
        text_color_light: false

  - block: portfolio
    id: project
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
        color: '#eaeaebff'
  - block: contact
    id: contact
    content:
      title: Contact
      text: |-
        Feel free to reach out for collaboration, inquiries, or feedback. Leave your name, email, and a short message—I usually reply within 2–3 business days. Your information is used solely for communication.
      email: jialinzheng@ieee.org
      phone: +1 765-767-0550
      address:
        street: 401 N Grant St
        city: West Lafayette
        region: IN
        postcode: '47907'
        country: United States
        country_code: US
      coordinates:
        latitude: '40.4294'
        longitude: '-86.9124'
      directions: Enter A. A. Potter Engineering Center and take the stairs to Office 257 on Floor 2
      office_hours:
       - 'Monday 10:00 to 13:00'
       - 'Wednesday 09:00 to 10:00'
      appointment_url: 'https://calendly.com'
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
  
---


