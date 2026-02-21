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

  - block: markdown
    id: post
    content:
      title: News
      text: |

        ### 2026

        - **Mar-23-2026**，Invited talk at Cornell AI for Sustainability (AI4S) Seminar Series: [*“Empowering the Grid Edge: Real-Time Embedded AI on Power Electronics Converters”*](https://sustainability.ai.cornell.edu/seminars/).
        - **18-Feb-2026**，Our paper "[Discovering Unknown Inverter Governing Equations via Physics-Informed Sparse Machine Learning](https://arxiv.org/abs/2602.16166)" is subbmitted to  *arxiv*.

        ### 2025

        - **04-Jun-2024**，Our paper "[FPGA-based Real-Time X-in-the-loop Simulation Testbench for Dynamic Wireless Power Transfer System with Stochastic and Nonlinear Inductance](https://ieeexplore.ieee.org/abstract/document/11077776)" is accepted by *IEEE Transactions on Industrial Electronics*.
      
        
        ### 2024
        - **04-Jun-2024**，Our paper "[FPGA-based Real-Time X-in-the-loop Simulation Testbench for Dynamic Wireless Power Transfer System with Stochastic and Nonlinear Inductance](https://ieeexplore.ieee.org/abstract/document/10551289)" is accepted by *IEEE Transactions on Transportation Electrification*.
        

      design:
       column: 2

  - block: collection
    id: event
    content:
      title: Recent and Upcoming Events
      filters:
        folders:
          - event
        exclude_future: false
        exclude_past: false
    design:
      view: card

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
        My research focuses on AI-enabled design and control of intelligent circuits and complex networked systems, bridging integrated microwave communication and large-scale power conversion through advanced digital methodologies.
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

  - block: features
    id: affiliations
    content:
      title: Affiliations
      items:
        - name: Princeton University
          image:
            filename: princeton.svg
          link: https://www.princeton.edu

        - name: Purdue University
          image:
            filename: purdue.svg
          link: https://www.purdue.edu

        - name: Tsinghua University
          image:
            filename: tsinghua.svg
          link: https://www.tsinghua.edu.cn

        - name: Cornell University
          image:
            filename: cornell.svg
          link: https://www.cornell.edu
    design:
      columns: 4
      background:
        color: '#ffffff'

  - block: contact
    id: contact
    content:
      title: Contact
      text: |-
        Feel free to reach out for collaboration, inquiries, or feedback. Leave your name, email, and a short message—I usually reply within 2–3 business days. Your information is used solely for communication.
      email: jialinzheng@ieee.org
      phone: +1 765-767-0550
      address:
        street: B 216, Engineering Quadrangle
        city: Princeton
        region: NJ 
        postcode: '08540'
        country: United States
        country_code: US
      coordinates:
        latitude: '40.35'
        longitude: '-74.65'
      directions: B 217/219, Engineering Quadrangle, Princeton, NJ 08540
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


