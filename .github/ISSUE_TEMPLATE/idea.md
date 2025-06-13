---
name: Idea
about: Idea para el repositorio
title: "Idea: "
labels: ["idea"]
assignees:
  - midudev
---
body:
  - type: markdown
    attributes:
      value: 
        Gracias por hacer tu idea!!!
  
    validations:
      required: true
  - type: dropdown
    id: type-idea
    attributes:
      label: ¿Que version de Node.js estás usando?
      multiple: false
      options:
        - Visual
        - Codigo
        - Otro
    validations:
  - type: textarea
    id: descr
    attributes:
      label: Di tu idea
      description: Describe tu idea para el repo
      placeholder: Idea
      value: "Idea: "