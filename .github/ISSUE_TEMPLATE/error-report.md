---
name: Error
description: Error en el proyecto
title: "Error: "
labels: ["error"]
assignees:
  - midudev
---
body:
  - type: markdown
    attributes:
      value: 
        Gracias por hacer el reporte del error!!!
  
    validations:
      required: true
  - type: dropdown
    id: v-node
    attributes:
      label: ¿Que version de Node.js estás usando?
      multiple: false
      options:
        - 12
        - 13
        - 14
        - 15
        - 16
        - 17
        - 18
        - 19
        - 20
        - 21
        - 22
        - 23
        - 24
        - Otra
    validations:
  - type: dropdown
    id: browsers
    attributes:
      label: ¿Es un error en la web?
      multiple: false
      options:
        - Si
        - No
  - type: textarea
    id: console-log
    attributes:
      label: ¿Que error a ocurrido si a sido de consola
      description: Pasa el error que te a salido en consola
      placeholder: ¿Que sera?
      value: "log:"