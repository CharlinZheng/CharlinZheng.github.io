---
title: Projects
type: landing

sections:
  - block: markdown
    content:
      title: Research Projects
      subtitle: 'Browse by category:'
      text: |
        [All Projects](/project/) | [Machine Learning](/tags/machine-learning/) | [Computer Vision](/tags/computer-vision/) | [NLP](/tags/nlp/) | [Deep Learning](/tags/deep-learning/)
    design:
      columns: '1'
      css_style: |
        text-align: center;
        a {
          display: inline-block;
          margin: 0.5rem;
          padding: 0.5rem 1.5rem;
          background: #007bff;
          color: white;
          border-radius: 25px;
          text-decoration: none;
        }
        a:hover {
          background: #0056b3;
          transform: translateY(-2px);
        }
  - block: portfolio  # 如果主题支持
    content:
      title: ''
      page_type: project
      filter_button:
        - name: All
          tag: '*'
        - name: Machine Learning
          tag: ML
        - name: Computer Vision
          tag: CV
    design:
      columns: '2'
      view: showcase
  
  - block: collection
    content:
      title: ''
      page_type: project
      count: 0
      filters:
        folders:
          - project
    design:
      view: card
      columns: '2'
---