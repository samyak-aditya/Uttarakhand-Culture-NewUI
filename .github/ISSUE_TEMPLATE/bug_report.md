---
name: Report a Bug 🐞
about: Help us improve by reporting an issue.
title: "[BUG] Brief description"
labels: ["status: awaiting triage"]
body:
  - type: checkboxes
    id: duplicates
    attributes:
      label: Is this a new issue?
      description: Please confirm you've checked that this issue hasn't been reported before.
      options:
        - label: I have searched "open" and "closed" issues, and this is not a duplicate.
          required: true

  - type: textarea
    id: description
    attributes:
      label: Bug Description
      description: Provide a clear and concise description of the issue.
    validations:
      required: true

  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to Reproduce
      description: List the steps to reproduce the issue.
    validations:
      required: true

  - type: textarea
    id: expected-behavior
    attributes:
      label: Expected Behavior
      description: Describe what you expected to happen.
    validations:
      required: true

  - type: textarea
    id: actual-behavior
    attributes:
      label: Actual Behavior
      description: Describe what actually happened.
    validations:
      required: true

  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots (if applicable)
      description: Attach screenshots to help explain your issue.
    validations:
      required: false

  - type: dropdown
    id: assignee
    attributes:
      label: Do you want to work on this issue?
      options:
        - "Yes"
        - "No"
      validations:
        required: true

  - type: markdown
    attributes:
      value: |
        Thank you for taking the time to report this bug! Please make sure to fill out all the sections to help us address the issue effectively.
---