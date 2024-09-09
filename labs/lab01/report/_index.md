---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Навыки
      items:
        - name: Python
          description: 60%
          icon: python
          icon_pack: fab
        - name: Рисование
          description: 120%
          icon: paint-brush
          icon_pack: fas
        - name: Английский
          description: 20%
          icon: language
          icon_pack: fas
        - name: Обучение других
          description: 10%
          icon: mortar-board
          icon_pack: fas
  - block: experience
    content:
      title: Опыт
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Проджект-менеджер
          company: brainz CROC
          company_url: 'https://www.croc.ru/'
          company_logo: White_Logo
          location: Москва
          date_start: '2022-10-01'
          date_end: '2022-12-25'
          description: |2-
              Полученные навыки:

              * Customer-development
              * Дизайн-мышление
              * Наставничество
        - title: Репетитор
          company: Мой дом))
          company_url: 'https://www.croc.ru/'
          company_logo: teacher
          location: Москва
          date_start: '2023-01-27'
          date_end: ''
          description: Обучаю детей математике
        - title: Разработчик
          company: brainz CROC
          company_url: 'https://www.croc.ru/'
          company_logo: Green_Logo
          location: Москва
          date_start: '2020-01-11'
          date_end: '2021-03-31'
          description: Научилась создавать сайты и работать в команде
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Достижения'
      subtitle: мои достижения
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: [https://stepik.org/catalog](https://stepik.org/cert/2081530)
          date_end: ''
          date_start: '2022-10-25'
          description: ''
          organization: Stepik
          organization_url: https://stepik.org/catalog
          title: Введение "Операционные системы"
          url: ''
        - certificate_url: https://2127.mskobr.ru/proekty/nashi-proekty/profilnyiy-tsentr-mtm---moskovskiy-tehnologicheskiy-marafon
          date_end: '2022-03-20'
          date_start: '2021-10-20'
          description: Решение CTF
          organization: Министерство образования
          organization_url: https://2127.mskobr.ru/proekty/nashi-proekty/profilnyiy-tsentr-mtm---moskovskiy-tehnologicheskiy-marafon
          title: Кибертон
        - certificate_url: https://im.mcko.ru/potential.php
          date_end: '2022-02-14'
          date_start: '2022-04-03'
          description: ''
          organization: МЦКО
          organization_url: https://im.mcko.ru/
          title: Конкурс "Мегаполис потенциал"
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      email: test@example.org
      phone: 888 888 88 88
      appointment_url: 'https://calendly.com'
      address:
        street: 450 Serra Mall
        city: Stanford
        region: CA
        postcode: '94305'
        country: United States
        country_code: US
      directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      office_hours:
        - 'Monday 10:00 to 13:00'
        - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/Twitter'
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: 'skype:echo123?call'
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: 'https://zoom.com'
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
