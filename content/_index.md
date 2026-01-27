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
        - name: Languages
          items:
            - name: C#
              icon: devicon/csharp
            - name: TypeScript
              icon: devicon/typescript
            - name: Go
              icon: devicon/go
            - name: PowerShell
              icon: devicon/powershell
        - name: .NET
          items:
            - name: .NET Core
              icon: devicon/dotnetcore
            - name: ASP.NET
              icon: devicon/dot-net
            - name: Entity Framework
              icon: devicon/dotnetcore
        - name: DevOps
          items:
            - name: Docker
              icon: devicon/docker
            - name: Kubernetes
              icon: devicon/kubernetes
            - name: Azure
              icon: devicon/azure
            - name: GitHub Actions
              icon: brands/github
        - name: Tools
          items:
            - name: Git
              icon: devicon/git
            - name: Azure DevOps
              icon: devicon/azure
            - name: Prometheus
              icon: devicon/prometheus
            - name: Linux
              icon: devicon/linux
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
