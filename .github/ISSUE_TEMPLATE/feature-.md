---
name: 'Feature'
about: Issue Template for new features
title: 'Feature:'
labels: ''
assignees: ''
body:
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: What is your name?
      placeholder: ex. Victoria Einzburg
    validations:
      required: false
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to suggest a new feature! Please fill out the template below to help us understand what you’re looking for.
  - type: dropdown
    id: request
    attributes:
      label: Type of request?
      description: Select the type of your request
      options:
        - New Feature
        - Improvment to existing feature
      default: 0
    validations:
      required: true
  - type: dropdown
    id: os
    attributes:
      label: What is the OS which you want to suggest?
      multiple: true
      options:
        - MacOS
        - Windows
        - Linux
  - type: textarea
    id: suggestion
    attributes:
      label: What are the details of your suggestion?
      description: Explain what do you want
      placeholder: Feature details
      render: shell
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our Code of Conduct.
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
---


