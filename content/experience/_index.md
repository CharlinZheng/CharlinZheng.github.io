---
title: My page
type: landing

sections:
  

  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many experience `items` below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Postdoctoral Fellow
          company: Purdue University
          company_url: 'https://www.purdue.edu/'
          company_logo: purdue
          location: Indiana, USA
          date_start: '2024-09-01'
          date_end: ''
          description: |2-
              Participate in Project:
              * Digital Twin Addressing Multi-Scale Operational Needs of IBR-rich Grids (DIAMOND)(funded by Department of Energy with  $80,000.00)
              * Universal interoperability for grid-forming inverters (UNIFI) https://unificonsortium.org/
        - title: Teaching Assistant
          company: Tsinghua University
          company_url: 'https://www.tsinghua.edu.cn/en/'
          company_logo: tsinghua
          location: Beijing, China
          date_start: '2024-06-30'
          date_end: '2024-07-18'
          description: |2-
              The course: “Modeling and Control of Power Converters” with Prof. [Dushan Boroyevich](https://cpes.vt.edu/people/faculty/89) and Prof. [Kai Sun](https://www.eea.tsinghua.edu.cn/en/faculties/sunkai.htm).
        - title: Teaching Assistant
          company: Tsinghua University
          company_url: 'https://www.tsinghua.edu.cn/en/'
          company_logo: tsinghua
          location: Beijing, China
          date_start: '2020-09-02'
          date_end: '2021-01-21'
          description: |2-
              Design and Analysis of Electrical Machine Systems (40220682) with Prof. Zhengming Zhao.
        - title: Research Scientist
          company: Delta Electronics, Inc.
          company_url: 'https://deltaww.com/'
          company_logo: delta
          location: Shanghai, China
          date_start: '2021-06-15'
          date_end: '2021-08-14'
          description: |2-
              Research on Artificial Intelligence in Power Electronic Systems
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'

  - block: experience
    content:
      title: Education
      
      date_format: Jan 2006
      items:
        - title: PhD Electronic Engineering
          company: Tsinghua University
          company_url: 'https://www.tsinghua.edu.cn/en/'
          company_logo: tsinghua
          location: Beijing, China
          date_start: '2019-09-01'
          date_end: '2024-08-31'
          description: |2-
              * Thesis on **Real-time simulation of power electronics**. Supervised by Prof Zhengming Zhao. 
              * The relevant research results have been published in more than 20 IEEE Top journals. 
              * The thesis was awarded the title of Outstanding Doctoral Thesis at Tsinghua University.
        - title: BEng Electronic Engineering
          company: Beijing Jiaotong University
          company_url: 'http://en.njtu.edu.cn/'
          company_logo: bjtu
          location: Beijing, China
          date_start: '2015-09-01'
          date_end: '2019-08-31'
          description: |2-
              * Overall GPA: 4.42/5.00
              * Ranking 2/308
              * Outstanding Graduate.
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'

  - block: accomplishments
    content:
      title: Awards
      subtitle: ''
      text: ''
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `items` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Neural Networks and Deep Learning
          certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2021-01-25'
          description: ''
          icon: coursera
          organization: Coursera
          organization_url: https://www.coursera.org
          url: ''
        - title: Blockchain Fundamentals
          certificate_url: https://www.edx.org
          date_end: ''
          date_start: '2021-01-01'
          description: Formulated informed blockchain models, hypotheses, and use cases.
          icon: edx
          organization: edX
          organization_url: https://www.edx.org
          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
        - title: 'Object-Oriented Programming in R'
          certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          icon: datacamp
          organization: DataCamp
          organization_url: https://www.datacamp.com
          url: ''
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
  - block: features
    content:
      title: Services
      subtitle: Section subtitle
      text: Section text
      items:
        - name: R
          description: 90%
          icon: r-project
          icon_pack: fab
        - name: Statistics
          description: 100%
          icon: chart-line
          icon_pack: fas
        - name: Photography
          description: 10%
          icon: camera-retro
          icon_pack: fas
---
