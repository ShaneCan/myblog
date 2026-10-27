---
date: "2022-10-24"
sections:
- block: about.biography
  content:
    title: About
    username: admin
  design:
    spacing:
      padding: ["48px", "0", "32px", "0"]
  id: about

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
    archive:
      enable: true
      link: https://scholar.google.com/citations?view_op=list_works&authuser=1&user=q6B8jmYAAAAJ&authuser=1
      text: See all on Google Scholar
  design:
    columns: "1"
    view: compact
    spacing:
      padding: ["40px", "0", "40px", "0"]
  id: publications

- block: portfolio
  content:
    buttons:
    - name: All
      tag: '*'
    default_button_index: 0
    filters:
      folders:
      - project
    title: Demonstrations
  design:
    columns: "1"
    flip_alt_rows: false
    view: showcase
    spacing:
      padding: ["40px", "0", "40px", "0"]
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
      padding: ["40px", "0", "40px", "0"]
  id: posts

- block: contact
  content:
    address:
      city: Dresden
      country: Germany
      country_code: DE
      postcode: "01069"
      region: Germany
      street: Andreas-Pfitzmann-Bau (APB), Nöthnitzer Strasse 46
    autolink: true
    email: tianxiong.zhang[at]tu-dresden.de
    subtitle: I am happy to supervise Bachelor's and Master's theses on topics related to AI, computer vision, and robotics applications in air transportation. Feel free to reach out.
    title: Contact
  design:
    columns: "1"
    spacing:
      padding: ["40px", "0", "40px", "0"]
  id: contact

- block: lab-gallery
  content:
    title: Drone experiments
    images:
    - filename: albums/Holybro_field_test.png
      alt: Holybro quadrotors.
    - filename: albums/Crazyflies-2.png
      alt: Crazyflie quadrotors.
    - filename: albums/Crazyflies-3.png
      alt: Crazyflie quadrotors.
    - filename: albums/Crazyflies in Robolab.png
      alt: Crazyflie quadrotors.
  id: lab-gallery

title: null
type: landing
---
