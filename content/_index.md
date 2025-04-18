---
# Leave the homepage title empty to use the site title
title: ''
date: 2023-12-29
type: landing

sections:
  - block: hero
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: Hugo Academic Theme
      image:
        filename: hero-academic.png
      cta:
        label: '**Get Started**'
        url: https://hugoblox.com/templates/
      cta_alt:
        label: Ask a question
        url: https://discord.gg/z8wNYzb
      cta_note:
        label: >-
          <div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star Hugo Blox Builder</a></div><div style="text-shadow: none;"><a class="github-button" href="https://github.com/HugoBlox/theme-academic-cv" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star">Star the Academic template</a></div>
      text: |-
        **Generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 500,000+ sites.**

        **Easily build anything with blocks - no-code required!**

        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.

        <!--Custom spacing-->
        <div class="mb-3"></div>
        <!--GitHub Button JS-->
        <script async defer src="https://buttons.github.io/buttons.js"></script>
    design:
      background:
        gradient_end: '#1976d2'
        gradient_start: '#004ba0'
        text_color_light: true
  - block: about.biography
    id: about
    content:
      title: Welcome
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin   

  - block: collection
    id: featured
    content:
      title: Current work
      filters:
        folders:
          - publication
        featured_only: false # this means displaying the full abstract and everything on the website (when true)
        publication_type: '3' # originally: 3
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Publications
      text: #|-
       # {{% callout note %}}
       # Quickly discover relevant content by [filtering publications](./publication/).
       # {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
        publication_type: '2' # originally: 2
    design:
      columns: '2'
      view: citation
#  - block: collection
#    content:
#      title: Work in progress
#      text: #|-
#       # {{% callout note %}}
#       # Quickly discover relevant content by [filtering publications](./publication/).
#       # {{% /callout %}}
#      filters:
#        folders:
#          - publication
#        exclude_featured: true
#        publication_type: '0'
#    design:
#      columns: '2'
#      view: citation
  - block: collection
    id: policy
    content:
      title: Policy reports
      text: #|-
       # {{% callout note %}}
       # Quickly discover relevant content by [filtering publications](./publication/).
       # {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
        publication_type: '4' # originally: 4
    design:
      columns: '2'
      view: citation
#  - block: collection
#    #id: featured
#    content:
#      title: Work in progress
#      filters:
#        folders:
#          - publication
#       #exclude_featured: true
#        publication_type: '4'
#    design:
#      columns: '2'
#      view: citation
  - block: markdown
    id: teaching
    content:
      title: Teaching
      #subtitle: My subtitle
      text: |- 
        ## Free University Berlin 
        <span style="line-height: 2;"> 

        - Winter 2022/2023 Behavioral Macroeconomics, Seminar (B.Sc.), _Teaching Assistant_
        - Summer 2022 Fundamentals of Macroeconomics (B.Sc.), _Teaching Assistant_
        - Winter 2021/2022 Behavioral Macroeconomics, Seminar (B.Sc.), _Teaching Assistant_
    design:
      columns: '2'
        #view: compact
#      text: Add any **markdown** formatted content here - text, images, videos, galleries - and even HTML code!
#  - block: collection
#    id: teaching
#    content:
#      title: Teaching 
#        items:
#          - title: Behavioral Macroeconomics - Seminar (B.Sc.) 
            #company: GenCoin
            #company_url: ''
            #company_logo: org-gc
            #location: California
            #date_start: '2021-01-01'
            #date_end: ''
#            description: |2-
#                Teaching Assistant
#    design:
#      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: 
      # Contact (add or remove contact options as necessary)
      email: frederik.kurcz@gmail.com
      #phone: 888 888 88 88
      #appointment_url: 'https://calendly.com'
      address:
        street: Mohrenstraße 58
        city: Berlin
        #region: CA
        postcode: '10117'
        country: Germany
        #country_code: US
      #directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      #office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      #coordinates:
      #  latitude: '37.4275'
      #  longitude: '-122.1697'  
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/FrederikKurcz'
        - icon: hero/chevron-right
          icon_pack: hero
          name: Link to my DIW website
          link: 'https://www.diw.de/sixcms/detail.php?id=diw_01.c.840943.en'
      #  - icon: skype
      #    icon_pack: fab
      #    name: Skype Me
      #    link: 'skype:echo123?call'
      #  - icon: video
      #    icon_pack: fas
      #    name: Zoom Me
      #    link: 'https://zoom.com'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      #form:
      #  provider: netlify
      #  formspree:
      #    id:
      #  netlify:
      #    # Enable CAPTCHA challenge to reduce spam?
      #    captcha: false
    design:
      columns: '2'
---