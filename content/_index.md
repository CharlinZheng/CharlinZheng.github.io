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
              brightness: 0.5
          position: right
          color: '#666'
        link:
          icon: book
          icon_pack: fas
          text: Get Started
          url: ../project/
      - title: Want to know more about me? ☕️
        content: 'Please see my profile and CV!'
        align: left
        background:
          image:
            filename: robot.jpg
            filters:
              brightness: 0.7
          position: center
          color: '#555'
        link:
          icon: circle-user
          icon_pack: fas
          text: Find Me
          url: ../aboutme/
      - title: Cooperation to promote energy system upgrades
        content: 'Achieving digitization, informatization, and intelligence！'
        align: right
        background:
          image:
            filename: world.jpg
            filters:
              brightness: 0.5
          position: center
          color: '#333'
        link:
          icon: graduation-cap
          icon_pack: fas
          text: Contact me!
          url: ../contact/
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: ''
      is_fullscreen: true
      # Automatically transition through slides?
      loop: true
      # Duration of transition between slides (in ms)
      interval: 5000
---


