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
      title: "Tech Stack"
      subtitle: "Technologies I use to build things"
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
            - name: MCP (Model Context Protocol) # Shows you understand standard interfaces for AI
              icon: brands/mcp # Generic icon, or use a 'server' icon
            - name: LangChain # The industry standard for orchestration (good to know both)
              icon: brands/langchain
            - name: Ollama # Shows you know how to run 'safe/local' models (huge for Education)
              icon: brands/ollama1
            - name: Hugging Face # Shows you know how to run 'safe/local' models (huge for Education)
              icon: brands/huggingface
        - name: Languages
          items:
            - name: C#
              icon: devicon/csharp
            - name: TypeScript
              icon: devicon/typescript
            - name: Go
              icon: devicon/go
            - name: Python # Crucial to list here too for data/scripting
              icon: devicon/python
            - name: C++ # Differentiator: Shows deep technical roots (Games/Legacy)
              icon: devicon/cplusplus
        - name: Databases # MISSING FROM YOUR LIST
          items:
            - name: SQL Server
              icon: devicon/microsoftsqlserver
            - name: PostgreSQL
              icon: devicon/postgresql
            - name: Redis # Vital for the "Scale" narrative
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
            - name: Blazor # Optional: If you want to show modern .NET UI
              icon: devicon/blazor
        - name: Cloud & DevOps
          items:
            - name: Azure
              icon: devicon/azure
            - name: AWS # Listed in your CV, shows multi-cloud maturity
              icon: devicon/amazonwebservices-wordmark
            - name: Kubernetes
              icon: devicon/kubernetes
            - name: git
              icon: devicon/git
            - name: GitHub
              icon: devicon/github
            - name: Docker
              icon: devicon/docker
            - name: Terraform # Highly likely for a Director owning "Infrastructure"
              icon: devicon/terraform
        - name: Architecture # SUGGESTED CATEGORY
          items:
            - name: Kafka # Listed in your CV, key for "Event Driven"
              icon: devicon/apachekafka
            - name: Microservices
              icon: brands/microservice1
            - name: FinOps # You explicitly own this strategy
              icon: hero/currency-pound
        - name: Leadership & Culture
          items:
            - name: Technical Strategy
              icon: ♟️ # Chess pawn implies strategy/moves
            - name: Global Team Leadership
              icon: hero/globe-europe-africa
            - name: Mentoring & Coaching
              icon: 🌱 # Growth/Seedling
            - name: FinOps & Budgeting
              icon: 💸 # Money with wings (perfect for 'controlling' spend)
            - name: Stakeholder Management
              icon: 🤝 # Handshake
            - name: Public Speaking
              icon: 🎤 # Microphone
            - name: Recruitment & Hiring
              icon: brands/linkedin
            - name: Crisis Management
              icon: 🧯 # Fire extinguisher (Putting out fires)
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
      subtitle: "Let's build something amazing together"
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
