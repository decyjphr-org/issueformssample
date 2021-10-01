name: MSFT Co-Sell
description: Co-sell opportunities
title: "<CUSTOMER>-<TEAM>:<DATE>"
labels: [msft, needs-triage]
assignees:
  - rohitnb

body:
  - type: input
    id: msx-id
    attributes:
      label: MSX ID
    validations:
      required: true
  - type: input
    id: customer-name
    attributes:
      label: Customer Name
    validations:
      required: true
  - type: input
    id: team-name
    attributes:
      label: Team Name
    validations:
      required: true
  - type: input
    id: opp-size
    attributes:
      label: Opportunity Size
      description: How many developers does this team have? How many seats of GitHub are they looking for?
    validations:
      required: true
  - type: textarea
    id: key-stakeholders
    attributes:
      label: Key Stakeholders
      description: Who are the key decision makers and what are their emails?
    validations:
      required: true
  - type: dropdown
    id: scm
    attributes:
      label: Current Source Control Management solution?
      description: What system do they have in place currently?
      options:
        - GitLab
        - GitHub self-serve plans
        - Azure DevOps Git
        - Azure DevOps TFVC or TFS
        - BitBucket
        - Other
    validations:
      required: true
  - type: textarea
    id: devops-stack
    attributes:
      label: DevOps Tools
      description: What additional DevOps Tools do they have?
      placeholder: "CI/CD, Security, Issue Trackers etc.."
      value: |
        CI/CD: 
        Issue Tracker: 
        Application Security tools: 
        Operating/Deployment Targets: OnPrem/Cloud/Hybrid?
        Languages they write code in: 
    validations:
      required: true
  - type: textarea
    id: opp-context-1
    attributes:
      label: What is the customers primary need which is driving their interest in GitHub?
    validations:
      required: true
  - type: textarea
    id: opp-context-2
    attributes:
      label: Any specific capabilities that is driving the customers interest in GitHub?
    validations:
      required: true
  - type: textarea
    id: opp-context-3
    attributes:
      label: Additional Details
      placeholder: Any other details not captured above. Stuff like Timelines, history with customer etc.
    validations:
      required: true
