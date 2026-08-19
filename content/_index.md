---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Llama a tu perfil /content/authors/me
      username: me
      text: ''
      headings:
        about: 'Sobre mí'
        education: ''
        interests: ''
    design:
      css_class: 'quicksand-bio'
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: false

      # Name heading sizing to accommodate long or short names
      name:
        size: xs # Options: xs, sm, md, lg (default), xl
      avatar:
        size: large # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  
  - block: collection
    content:
      title: '📚 Proyectos'
      text: 'Esta es una muestra de algunos proyectos en los que he tenido la oportunidad de colaborar.'
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 2
  
  - block: collection
    id: papers
    content:
      title: Publicaciones destacadas
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  
  - block: collection
    content:
      title: Publicaciones recientes
      text: ''
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation  
---
