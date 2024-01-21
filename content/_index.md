---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: 个人简介
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    
  - block: portfolio
    id: projects
    content:
      title: 科研项目
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
        - name: 自动驾驶汽车
          tag: 自动驾驶
        - name: 智能网联汽车
          tag: 智能网联汽车
        - name: 智能驾驶仿真测试
          tag: 自动驾驶仿真
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
    
  - block: collection
    id: JournalPapers
    content:
      title: 科研成果
      subtitle: 期刊论文
      filters:
        folders:
          - publication
        exclude_featured: true
      order: desc
    design:
      columns: '1'
      view: compact
  
  - block: collection
    id: featured
    content:
      title: 科研成果
      subtitle: 会议论文
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '1'
      view: compact
    
  - block: experience
    id: experience
    content:
      title: 教育背景
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2023
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: 博士研究生
          company: 清华大学
          company_url: https://www.tsinghua.edu.cn/
          company_logo: org-Tsinghua
          location: 中国北京
          date_start: '2020-08-01'
          date_end: ''
          description: '自动化系 控制科学与工程专业 预计毕业时间2025年6月'
        - title: 工学学士
          company: 清华大学
          company_url: https://www.tsinghua.edu.cn/
          company_logo: org-Tsinghua
          location: 中国北京
          date_start: '2016-08-01'
          date_end: '2020-07-01'
          description: '自动化系 自动化专业 优秀毕业生'
    design:
      columns: '2'

  - block: features
    id: services
    content:
      title: 学术服务
      items:
        - name: 高水平期刊审稿人
          description: IEEE Transactions on Intelligent Transportation Systems, Transportation Research Part C-Emerging Technologies, IEEE Transactions on Intelligent Vehicles, IEEE Transactions on Automation Science and Engineering, IEEE Antennas and Wireless Propagation Letters, International Journal of Human-Computer Interaction, 自动化学报, 交通运输工程与信息学报
          icon: newspaper
          icon_pack: fas
        - name: 旗舰会议审稿人
          description: IEEE International Conference on Intelligent Transportation Systems-2022, IEEE International Conference on Intelligent Transportation Systems-2023; China Automation Conference-2022; China Automation Conference-2023
          icon: building-columns
          icon_pack: fas
        - name: 清华大学助教
          description: 3次担任清华大学研究生专业基础课《凸优化》课程助教 (2020, 2021; 2023)
          icon: person-chalkboard
          icon_pack: fas
    design:
      columns: '2'
      view: List
    
  - block: accomplishments
    id: awards
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: '荣誉获奖'
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
          date_start: ''
          description: ''
          organization: 中华人民共和国教育部
          organization_url: http://www.moe.gov.cn/
          title: 国家奖学金
          url: http://www.moe.gov.cn/
        
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
