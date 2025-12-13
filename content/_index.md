---
date: "2022-10-24"
sections:
- block: about.biography
  content:
    title: Biography
    username: admin
  design:
    spacing:
      padding: ["20px", "0", "20px", "0"]
  id: about
# - block: experience
#   content:
#     date_format: Jan 2006
#     items:
#     - company: Civil Aviation Flight University of China
#       company_logo: org-gc
#       company_url: ""
#       date_end: ""
#       date_start: "2021-09-01"
#       description: |2-
#           Department of Transportation
#           
#           College of Air Traffic Management
#           
#           Supervisor: Prof. Xinping Zhu
# 
#       location: Sichuan Province, China
#       title: Master's degree student
#     - company: Inner Mongolia University of Technology
#       company_logo: org-x
#       company_url: ""
#       date_end: "2021-07-01"
#       date_start: "2017-09-01"
#       description: |2-
#           Department of Transportation
#           
#           College of Aviation
#       
#       location: Inner Mongolia, China
#       title: Bachelor
#     title: Experience
#   design:
#     columns: "2"
#   id: experience
# - block: features
#   content:
#     items:
#     - name: Python
#     - name: Deep Learning
#     - name: Computer Vision
#     - name:
#     - name: 
#     - name: 
#     - name:
#     - name: 
#     - name: 
#     - name: ROS
#     - name: Linux
#     - name: R
#     title: Skills
#   id: Skills
# - block: collection
#   content:
#     # filters:
#     #   exclude_featured: true
#     #   folders:
#     #   - publication
#     # text: |-
#     #   {{% callout note %}}
#     #   Quickly discover relevant content by [filtering publications](./publication/).
#     #   {{% /callout %}}
#     title: Selected Publications
#   design:
#     columns: "2"
#     view: citation
#   id: publications
# - block: accomplishments
#   content:
#     date_format: Jan 2006
#     items:
#     - certificate_url: https://www.coursera.org
#       date_end: ""
#       date_start: "2021-01-25"
#       description: ""
#       organization: Coursera
#       organization_url: https://www.coursera.org
#       title: Neural Networks and Deep Learning
#       url: ""
#     - certificate_url: https://www.edx.org
#       date_end: ""
#       date_start: "2021-01-01"
#       description: Formulated informed blockchain models, hypotheses, and use cases.
#       organization: edX
#       organization_url: https://www.edx.org
#       title: Blockchain Fundamentals
#       url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
#     - certificate_url: https://www.datacamp.com
#       date_end: "2020-12-21"
#       date_start: "2020-07-01"
#       description: ""
#       organization: DataCamp
#       organization_url: https://www.datacamp.com
#       title: Object-Oriented Programming in R
#       url: ""
#     subtitle: null
#     title: Accomplish&shy;ments
#   design:
#     columns: "2"
- block: collection
  content:
    count: 6
    filters:
      author: ""
      category: ""
      exclude_featured: false
      exclude_future: false
      exclude_past: false
      folders:
      - publication
      publication_type: ""
      tag: ""
    offset: 0
    order: desc
    subtitle: ""
    text: ""
    title: Selected Publications
  design:
    columns: "1"
    view: compact
    spacing:
      padding: ["20px", "0", "20px", "0"]
  id: publications
- block: portfolio
  content:
    buttons:
    - name: All
      tag: '*'
#    - name: Deep Learning
#      tag: Deep Learning
#    - name: Other
#      tag: Demo
    default_button_index: 0
    filters:
      folders:
      - project
    title: Projects
  design:
    columns: "1"
    flip_alt_rows: false
    view: showcase
    spacing:
      padding: ["20px", "0", "20px", "0"]
  id: projects
- block: collection
  content:
    count: 5
    filters:
      author: ""
      category: ""
      exclude_featured: false
      exclude_future: false
      exclude_past: false
      folders:
      - post
      publication_type: ""
      tag: ""
    offset: 0
    order: desc
    subtitle: ""
    text: ""
    title: News
  design:
    columns: "1"
    view: compact
    spacing:
      padding: ["20px", "0", "20px", "0"]
  id: posts
# - block: collection
#   content:
#     filters:
#       featured_only: true
#       folders:
#       - publication
#     title: Featured Publications
#   design:
#     columns: "2"
#     view: card
#   id: featured
- block: markdown
  content:
    subtitle: ""
    text: '{{< gallery album="demo" >}}'
    title: Gallery
  design:
    columns: "1"
    spacing:
      padding: ["20px", "0", "20px", "0"]
    id: gallery
# - block: collection
#   content:
#     filters:
#       folders:
#       - event
#     title: Recent & Upcoming Talks
#   design:
#     columns: "2"
#     view: compact
#   id: talks
# - block: tag_cloud
#   content:
#     title: Popular Topics
#   design:
#     columns: "2"
- block: contact
  content:
    address:
      city: Dresden
      country: Germany
      country_code: DE
      postcode: "01069"
      region: Germany
      street: 2081, Andreas-Pfitzmann-Bau (APB), Nöthnitzer Strasse 46
    # appointment_url: https://calendly.com
    autolink: true
    contact_links:
    # - icon: twitter
    #   icon_pack: fab
    #   link: https://twitter.com/Twitter
    #   name: DM Me
    # - icon: skype
    #   icon_pack: fab
    #   link: skype:echo123?call
    #   name: Skype Me
    # - icon: video
    #   icon_pack: fas
    #   link: https://zoom.com
    #   name: Zoom Me
    # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
    email: tianxiong.zhang[at]tu-dresden.de
    # form:
    #   formspree:
    #     id: null
    #   netlify:
    #     captcha: false
    #   provider: netlify
    # office_hours:
    # - Monday 10:00 to 13:00
    # - Wednesday 09:00 to 10:00
    # phone: +86 15934146183
    subtitle: null
    # text: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis
    #   ut magna et, vehicula efficitur enim.
    title: Contact
  design:
    columns: "1"
    spacing:
      padding: ["20px", "0", "20px", "0"]
  id: contact
title: null
type: landing
---
