---
title: Projects
type: landing

sections:
  - block: markdown
    content:
      title: Our Projects
      subtitle: 'Filter by category:'
      text: |
        <div class="btn-toolbar filter-toolbar" role="toolbar" aria-label="Filter toolbar">
          <div class="btn-group flex-wrap" role="group" aria-label="Filter buttons">
            <a href="#projects" class="btn btn-primary active">All</a>
            <a href="/tags/ml/" class="btn btn-primary">Machine Learning</a>
            <a href="/tags/cv/" class="btn btn-primary">Computer Vision</a>
            <a href="/tags/nlp/" class="btn btn-primary">NLP</a>
          </div>
        </div>
    design:
      columns: '1'
      
  - block: collection
    id: projects
    content:
      title: ''
      subtitle: ''
      text: ''
      count: 0
      filters:
        folders:
          - project
        exclude_featured: false
      archive:
        enable: false
    design:
      view: card
      columns: '2'
---