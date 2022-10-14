---
widget: slider
weight: 1
active: true
headless: true

design:
  # Slide height is automatic unless you force a specific height (e.g. '400px')
  slide_height: ''
  is_fullscreen: true
  # Automatically transition through slides?
  loop: false
  # Duration of transition between slides (in ms)
  interval: 2000

content:
  slides:
    # - title: 👋 Welcome to MAGIC
    #   content: Multi-Agent Graph Intelligence Crew 🪄
    #   align: center
    #   background:
    #     position: right
    #     color: '#666'
    #     brightness: 0.7
    #     media: graph.jpg
    - title: '<font>Welcome to<br> Multi-Agent Graph Intelligence Crew<br> (MAGIC)</font>'
      content: ''
      align: center
      background:
        position: center
        color: '#555'
        brightness: 0.4
        media: bevpic.jpg
    - title: About MAGIC
      content: 'Multi-Agent Graph Intelligence Crew at Shanghai Jiao Tong University is dedicated to the research of graph-based interaction modeling and collaboration strategy learning.'
      align: right
      background:
        position: center
        color: '#333'
        brightness: 0.5
        media: bevpic2.jpg
      link:
        icon: github
        icon_pack: fab
        text: Follow us
        url: 'https://github.com/SJTU-MAGIC'
---
