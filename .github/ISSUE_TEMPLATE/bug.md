name: Bug Report. 
description: Create a report to help us improve
default_title: "[Bug]: "
labels: bug
inputs:
- dropdown:
    label: "**What type of feedback are you reporting?**"
    choices:
      - value: Incorrect/Unexpected Behavior
      - value: Application Crash
      - value: Application Slow/Unresponsive
      - value: Battery Life
      - value: Something Else
- input:
    id: version
    label: "**Which version are you using?**"
    required: true
    placeholder: 1.7.5
- textarea:
    label: "**Describe the bug**"
    description: A clear and concise description of the problem.
    required: true
- checkboxes:
    label: "**Debugging steps**"
    choices:
      - value: I can reproduce the problem with `--debug=true`
- textarea:
    label: "**To Reproduce**"
    description: Steps to reproduce the behaviour.
    required: true
    value: |
      1. Go to '...'
      2. Click on '....'
      3. Scroll down to '....'
      4. See error
- textarea:
    id: additional-context
    label: "**Additional context**"
    description: Add any other context about the problem here.
issue_body: false
