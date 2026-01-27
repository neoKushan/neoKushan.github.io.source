---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

design:
  # Default section spacing
  spacing: '0'

sections:
  # Developer Hero - Gradient background with name, role, social, and CTAs
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      show_status: true
      show_scroll_indicator: true
      typewriter:
        enable: true
        prefix: "I build"
        strings:
          - "enterprise software"
          - "seamless pipelines"
          - "scalable platforms"
          - "world class teams"
          - "high-performing cultures"
          - "future leaders"
          - "engineering excellence"
          - "technical strategy"
          - "cloud-native solutions"
          - "operational efficiency"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: What I do
          url: "#experience"
          icon: arrow-down
        - text: Get In Touch
          url: "#contact"
          icon: envelope
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["6rem", "0", "4rem", "0"]
  
  # Visual Tech Stack - Icons organized by category
  - block: tech-stack
    id: skills
    content:
      title: "The Stack"
      subtitle: "How I do what I do"
      categories:
        - name: AI & Emerging Tech
          items:
            - name: OpenAI / ChatGPT
              icon: brands/openai
            - name: Anthropic Claude
              icon: brands/claude
            - name: Google Gemini
              icon: brands/gemini
            - name: Microsoft Copilot
              icon: brands/copilot
            - name: MCP (Model Context Protocol) AI
              icon: brands/mcp 
            - name: LangChain 
              icon: brands/langchain
            - name: Ollama 
              icon: brands/ollama1
            - name: Hugging Face
              icon: icons/huggingface
        - name: Languages
          items:
            - name: C#
              icon: devicon/csharp
            - name: Visual Basic
              icon: devicon/visualbasic
            - name: TypeScript
              icon: devicon/typescript
            - name: Go
              icon: devicon/go
            - name: Python 
              icon: devicon/python
            - name: C++ # 
              icon: devicon/cplusplus
        - name: Databases 
          items:
            - name: SQL Server
              icon: devicon/microsoftsqlserver
            - name: PostgreSQL
              icon: devicon/postgresql
            - name: Redis 
              icon: devicon/redis
            - name: MongoDB
              icon: devicon/mongodb
            - name: MariaDB
              icon: devicon/mariadb
            - name: MySQL
              icon: devicon/mysql
        - name: .NET
          items:
            - name: Modern .NET
              icon: devicon/dotnetcore
            - name: ASP.NET Core
              icon: devicon/dot-net
            - name: Entity Framework
              icon: devicon/dotnetcore
            - name: Blazor 
              icon: devicon/blazor
        - name: Cloud & DevOps
          items:
            - name: Azure
              icon: devicon/azure
            - name: AWS 
              icon: devicon/amazonwebservices-wordmark
            - name: Kubernetes
              icon: devicon/kubernetes
            - name: git
              icon: devicon/git
            - name: GitHub
              icon: devicon/github
            - name: Docker
              icon: devicon/docker
            - name: Terraform 
              icon: devicon/terraform
        - name: Architecture 
          items:
            - name: Kafka 
              icon: devicon/apachekafka
            - name: Microservices
              icon: brands/microservice1
            - name: FinOps 
              icon: hero/currency-pound
        - name: Leadership & Culture
          items:
            - name: Technical Strategy
              icon: icons/pawn 
            - name: Global Team Leadership
              icon: hero/globe-europe-africa
            - name: Mentoring & Coaching
              icon: icons/seed 
            - name: Budgeting
              icon: icons/money 
            - name: Stakeholder Management
              icon: icons/handshake 
            - name: Public Speaking
              icon: icons/mic 
            - name: Recruitment
              icon: brands/linkedin
            - name: Crisis Management
              icon: icons/fire-ext 
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      username: me
      title: "Experience"
      subtitle: "My professional journey"
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Filterable Portfolio - Alpine.js powered project filtering
  - block: portfolio
    id: projects
    content:
      title: "Featured Projects"
      subtitle: "A selection of my work"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: Open Source
          tag: Open Source
        - name: .NET
          tag: .NET
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]

  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: Get In Touch
      subtitle: "Need a world class leader?"
      text: |-
        I'm always interested in hearing about new projects and opportunities.
        Whether you're looking to hire, collaborate, or just want to say hi, feel free to reach out!
      email: donaghy.steve@googlemail.com
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
---
