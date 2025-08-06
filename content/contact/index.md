---
title: Contact
date: 2022-10-24

type: landing

sections:
  - block: contact
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
        latitude: '40.2631'
        longitude: '86.5445'
      directions: Enter Potter Center and take the stairs to Office 257 on Floor 2
      #office_hours:
      # - 'Monday 10:00 to 13:00'
      # - 'Wednesday 09:00 to 10:00'
      #appointment_url: 'https://calendly.com'
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
      columns: '1'

  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: contact.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen
---
