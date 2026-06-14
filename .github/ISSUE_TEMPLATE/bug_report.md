---
name: Bug report
description: Report a reproducible problem with the mod menu
title: "[Bug]: "
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for reporting a bug. Please include enough detail to reproduce the issue.
  - type: input
    id: mod-version
    attributes:
      label: Mod version
      description: Which version are you using?
      placeholder: "Example: 1.0.0"
    validations:
      required: true
  - type: input
    id: game-version
    attributes:
      label: Game version
      description: Which Neon Abyss build/version are you running?
      placeholder: "Example: Steam build"
    validations:
      required: true
  - type: textarea
    id: problem
    attributes:
      label: What happened?
      description: Describe the issue clearly.
    validations:
      required: true
  - type: textarea
    id: steps
    attributes:
      label: Steps to reproduce
      description: List the exact steps that trigger the issue.
      placeholder: |
        1. Launch the game
        2. Open the menu
        3. Click ...
        4. See error
    validations:
      required: true
  - type: textarea
    id: logs
    attributes:
      label: Logs or screenshots
      description: Paste relevant logs, error messages, or screenshots.
      render: text
  - type: checkboxes
    id: checks
    attributes:
      label: Checklist
      options:
        - label: I am using the latest release from this repository.
          required: true
        - label: I tested this in offline single-player.
          required: true
        - label: I backed up my save before testing.
          required: false
