---
name: "OctoAcme Project Management Docs README"
description: "Create a README for OctoAcme Project Management Docs with links to all process documents and a process summary"
title: "[Process Doc Update]: Create README for OctoAcme Project Management Docs with Process Summary and Links"
labels: ["documentation", "process improvement"]
body:
  - type: markdown
    attributes:
      value: |
        ## Issue Details
        
        This issue requests the creation of a comprehensive README for the OctoAcme Project Management Documentation that serves as a central index and quick reference guide.

  - type: textarea
    id: content_summary
    attributes:
      label: "Summary of New Content"
      description: "Briefly describe the new content or update you want to add."
      value: |
        Create a new README.md file in the docs/ folder that:
        1. Provides a brief overview of OctoAcme project management processes
        2. Contains a table of contents with links to all process documents:
           - octoacme-project-management-overview.md
           - octoacme-project-initiation.md
           - octoacme-project-planning.md
           - octoacme-execution-and-tracking.md
           - octoacme-risks-and-communication.md
           - octoacme-release-and-deployment.md
           - octoacme-retrospective-and-continuous-improvement.md
           - octoacme-roles-and-personas.md
        3. Acts as a landing page for quick navigation to all process documentation
    validations:
      required: true

  - type: textarea
    id: rationale
    attributes:
      label: "Why is this update needed?"
      description: "Explain the reason for this addition."
      value: |
        The project management documentation is scattered across individual files. A centralized README will:
        - Provide new team members with a quick overview of OctoAcme processes
        - Create a single entry point for navigating all project management documentation
        - Establish context for how different processes relate to each other
        - Improve discoverability and usability of the process documentation library
    validations:
      required: true

  - type: textarea
    id: example_content
    attributes:
      label: "Suggested Content"
      description: "Paste the proposed new text, checklist, or example content."
      value: |
        # OctoAcme Project Management Documentation
        
        Welcome to the OctoAcme Project Management Documentation. This directory contains standardized processes, templates, and guidance for running projects at OctoAcme.
        
        ## Quick Start
        
        OctoAcme follows a structured project lifecycle that emphasizes iterative delivery, clear ownership, and data-informed decisions. Our approach is designed to ensure transparency, reduce risk, and maximize team productivity.
        
        ### Core Principles
        - **Customer-first**: Prioritize customer value and usability
        - **Iterative delivery**: Deliver small, testable increments
        - **Clear ownership**: Each project has named Project Manager and Product Lead
        - **Data-informed decisions**: Measure impact and iterate based on evidence
        - **Psychological safety**: Encourage feedback and learning
        
        ## Project Lifecycle Overview
        
        OctoAcme projects follow these phases:
        
        1. **Initiation** — Validate business need, align stakeholders, confirm success criteria
        2. **Planning** — Break work into shippable increments, identify dependencies, establish timeline
        3. **Execution** — Build, test, review, and iterate with regular team rhythm and quality gates
        4. **Release** — Deploy to production with verification and stakeholder communication
        5. **Close & Retrospective** — Capture learnings and feed improvements back into processes
        
        ## Documentation Index
        
        ### Overview & Roles
        - [**Project Management Overview**](./octoacme-project-management-overview.md) — High-level introduction to OctoAcme's approach, core roles, and key artifacts
        - [**Roles & Personas**](./octoacme-roles-and-personas.md) — Definitions of Project Manager, Product Manager, Developer, and QA responsibilities
        
        ### Project Phases
        - [**Project Initiation**](./octoacme-project-initiation.md) — Guidance for validating ideas, aligning stakeholders, and deciding to move forward
        - [**Project Planning**](./octoacme-project-planning.md) — How to build an actionable backlog, estimate scope, and define dependencies
        - [**Execution & Tracking**](./octoacme-execution-and-tracking.md) — Day-to-day management, team rhythm, quality standards, and progress tracking
        - [**Release & Deployment**](./octoacme-release-and-deployment.md) — Standardized approach for releasing to production and managing rollbacks
        
        ### Cross-Cutting Concerns
        - [**Risk Management & Communication**](./octoacme-risks-and-communication.md) — Identifying, tracking, and escalating risks; stakeholder communication templates
        - [**Retrospective & Continuous Improvement**](./octoacme-retrospective-and-continuous-improvement.md) — How to run retrospectives and convert learnings into actionable improvements
        
        ## How to Use These Docs
        
        - **New to OctoAcme?** Start with the [Project Management Overview](./octoacme-project-management-overview.md)
        - **Starting a new project?** Follow the sequence: Initiation → Planning → Execution → Release → Retrospective
        - **Need role-specific guidance?** Refer to [Roles & Personas](./octoacme-roles-and-personas.md)
        - **Want to improve a process?** Create an issue using the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template
        
        ## Key Artifacts Used Across Projects
        
        - **Project Charter / One-pager** — Problem, goal, success metrics, timeline
        - **Roadmap and Release Plan** — Major milestones and delivery timeline
        - **Sprint/Iteration Backlog** — Work items with acceptance criteria
        - **Risk Register** — Identified risks with impact, likelihood, and mitigation
        - **Status Reports** — Weekly updates to stakeholders on progress and blockers
        - **Retrospective Notes** — Learnings and action items for continuous improvement
        
        ## Communication & Support
        
        Questions about these processes? 
        - Review the relevant doc for your current project phase
        - Reach out to your Project Manager or Product Manager
        - Suggest improvements by creating an issue in this repository

  - type: checkboxes
    id: acceptance_criteria
    attributes:
      label: "Acceptance Criteria"
      description: "Check all that apply:"
      options:
        - label: "Content aligns with existing process docs"
          required: true
        - label: "Update improves clarity or closes a documented gap"
          required: true
        - label: "Proposed content has been reviewed with stakeholders (if needed)"
