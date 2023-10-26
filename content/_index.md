---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    
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
        - name: Autonomous Driving
          tag: Autonomous Driving
        - name: Connected and Automated Vehicle
          tag: Connected and Automated Vehicle
        - name: Deep Reinforcement Learning
          tag: Deep Reinforcement Learning
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
    
  - block: collection
    id: JournalPapers
    content:
      title: Publications
      subtitle: Journal article
      filters:
        folders:
          - publication
        exclude_featured: true
      order: desc
    design:
      columns: '2'
      view: compact
  
  - block: collection
    id: featured
    content:
      title: Publications
      subtitle: Conference paper
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: compact
  - block: experience
    id: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2023
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Ph.D Student
          company: Tsinghua University
          company_url: https://www.tsinghua.edu.cn/
          company_logo: org-Tsinghua
          location: Beijing
          date_start: '2020-08-01'
          date_end: ''
          description: 'Pursuing the Ph.D. degree with the Department of Automation at Tsinghua University, Beijing, China'
        - title: Undergraduate Student
          company: Tsinghua University
          company_url: https://www.tsinghua.edu.cn/
          company_logo: org-Tsinghua
          location: Beijing
          date_start: '2016-08-01'
          date_end: '2020-07-01'
          description: 'Received the B.S. degree from Tsinghua University, Beijing, China, in 2020'
    design:
      columns: '2'

  - block: features
    id: services
    content:
      title: Services
      items:
        - name: Reviewer for Journal
          description: [IEEE Transactions on Intelligent Transportation Systems](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=6979)
          icon: newspaper
          icon_pack: fas
        - name: Reviewer for Conference
          description: IEEE ITSC-2022, IEEE ITSC-2023; CAC-2022
          icon: building-columns
          icon_pack: fas
        - name: Teaching Assistant
          description: Convex Optimization (2020, 2021)
          icon: person-chalkboard
          icon_pack: fas
    design:
      columns: '2'
      view: List
    
  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Honors & Awards'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2023
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: ''
          date_end: ''
          date_start: '2023-10-20'
          description: ''
          organization: Ministry of Education
          organization_url: http://www.moe.gov.cn/
          title: National Scholarship
          url: https://www.tsinghua.edu.cn/
        - certificate_url: http://www.baachina.cn/html/page/notice/notice2022-12.html
          date_end: ''
          date_start: '2022-12-01'
          description: ''
          organization: BEIJING ASSOCIATION OF AUTOMATION
          organization_url: http://www.baachina.cn/index.html
          title: Outstanding Ph.D Student
          url: http://www.baachina.cn/html/page/notice/notice2022-12.html
          icon: person-chalkboard
          icon_pack: fas
        - certificate_url: ''
          date_end: ''
          date_start: '2022-10-01'
          description: ''
          organization: IEEE ITSC 2022
          organization_url: https://www.ieee-itsc2022.org/#/
          organization_logo: org-Tsinghua
          title: Best Student Paper Award
          url: https://www.ieee-itsc2022.org/#/
        - certificate_url: ''
          date_end: ''
          date_start: '2022-10-01'
          description: Tsinghua-Xuancheng Scholarship
          organization: Tsinghua University
          organization_url: https://www.tsinghua.edu.cn/
          title: Excellent Comprehensive Scholarship of Tsinghua University
          url: https://www.tsinghua.edu.cn/
        - certificate_url: ''
          date_end: ''
          date_start: '2021-10-01'
          description: Tsinghua-Weihai Scholarship
          organization: Tsinghua University
          organization_url: https://www.tsinghua.edu.cn/
          title: Excellent Comprehensive Scholarship of Tsinghua University
          url: https://www.tsinghua.edu.cn/
        - certificate_url: ''
          date_end: ''
          date_start: '2020-10-01'
          description: ''
          organization: Department of Automation, Tsinghua University
          organization_url: https://www.tsinghua.edu.cn/
          title: Outstanding Graduates
          url: ''
        - certificate_url: ''
          date_end: ''
          date_start: '2019-10-01'
          description: ''
          organization: Ministry of Education
          organization_url: http://www.moe.gov.cn/
          title: National Encouragement Scholarship
          url: https://www.tsinghua.edu.cn/
        - certificate_url: ''
          date_end: ''
          date_start: '2018-10-01'
          description: ''
          organization: Ministry of Education
          organization_url: http://www.moe.gov.cn/
          title: National Encouragement Scholarship
          url: https://www.tsinghua.edu.cn/
        - certificate_url: ''
          date_end: ''
          date_start: '2017-10-01'
          description: ''
          organization: Ministry of Education
          organization_url: http://www.moe.gov.cn/
          title: National Encouragement Scholarship
          url: https://www.tsinghua.edu.cn/
        
    design:
      columns: '2'
      view: List
  
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
    
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle: Welcome to send emails to exchange.
      # Contact (add or remove contact options as necessary)
      email: zhangjw20@mails.tsinghua.edu.cn
      address:
        street: Department of Automation, Tsinghua University
        city: Beijing
        postcode: '100084'
        country: China
      office_hours:
        - 'Every day is Saturday, Saturday is a working day.'
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
