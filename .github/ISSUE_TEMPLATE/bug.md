---
name: 🐞 Bug report
description: File a bug report
labels:
  - bug
body:
  - type: markdown
    attributes:
      value: |
        Before opening a bug report, please search for the behaviour in the existing issues. 
        
        ---
        
        Thank you for taking the time to file a bug report. To address this bug as fast as possible, we need some information.
  - type: input
    id: tenant
    attributes:
      label: Tenant
      description: "Is this bug related to or for a specific tenant on Developer Studio?"
      placeholder: "Commerce Hub, Banking Hub, etc."
    validations:
      required: false
  - type: input
    id: page
    attributes:
      label: Page
      description: "On which page do you see the bug?"
      placeholder: "Account -> Data & Privacy"
    validations:
      required: true
  - type: textarea
    id: desc
    attributes:
      label: Description
      description: "Please describe the bug and how to reproduce it. Attach screenshots if applicable."
    validations:
      required: true
  - type: textarea
    id: expected
    attributes:
      label: Expected Behaviour
      description: "What is the expected behaviour?"
    validations:
      required: true
  - type: input
    id: os
    attributes:
      label: Operating system
      description: "Which operating system do you use? Please provide the version as well."
      placeholder: "macOS Big Sur 11.5.2"
    validations:
      required: true
  - type: input
    id: browser
    attributes:
      label: Browser
      description: "Which browser do you use? Please provide the version as well."
      placeholder: "Google Chrome 113.0.5672.92"
    validations:
      required: true

---