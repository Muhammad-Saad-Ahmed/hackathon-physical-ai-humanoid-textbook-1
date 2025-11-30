# Spec-Driven Development (SDD) Agent Framework

## Overview
This repository contains a framework designed to facilitate Spec-Driven Development (SDD) through an AI assistant. It provides a structured approach to software development, ensuring that user intent is strictly followed, and development artifacts like Prompt History Records (PHRs) and Architectural Decision Records (ADRs) are automatically managed. The AI agent acts as an expert architect, guiding users and executing tasks efficiently based on a defined set of tools and principles.

## Features
The framework is built around a set of specialized slash commands that streamline the SDD process:

*   **/sp.tasks**: Generate an actionable, dependency-ordered `tasks.md` for the feature based on available design artifacts.
*   **/sp.specify**: Create or update the feature specification (`spec.md`) from a natural language feature description.
*   **/sp.plan**: Execute the implementation planning workflow using the plan template to generate design artifacts (`plan.md`).
*   **/sp.phr**: Record an AI exchange as a Prompt History Record (PHR) for learning and traceability.
*   **/sp.implement**: Execute the implementation plan by processing and executing all tasks defined in `tasks.md`.
*   **/sp.git.commit_pr**: An autonomous Git agent that intelligently executes Git workflows to commit work and create Pull Requests.
*   **/sp.constitution**: Create or update the project constitution (`constitution.md`) from interactive or provided principle inputs, ensuring all dependent templates stay in sync.
*   **/sp.clarify**: Identify underspecified areas in the current feature spec by asking targeted clarification questions and encoding answers back into the spec.
*   **/sp.checklist**: Generate a custom checklist for the current feature based on user requirements.
*   **/sp.analyze**: Perform a non-destructive cross-artifact consistency and quality analysis across `spec.md`, `plan.md`, and `tasks.md` after task generation.
*   **/sp.adr**: Review planning artifacts for architecturally significant decisions and create ADRs.

## Project Structure

*   `.claude/commands/`: Contains the markdown files defining the custom slash commands (e.g., `/sp.adr`, `/sp.plan`).
*   `.specify/`: Holds various templates and scripts essential for the SDD workflow:
    *   `memory/constitution.md`: Project principles and guidelines.
    *   `scripts/`: PowerShell scripts for various operations (e.g., checking prerequisites, setting up plans).
    *   `templates/`: Markdown templates for ADRs, checklists, PHRs, plans, specs, and tasks.
*   `history/prompts/`: Stores Prompt History Records, organized by constitution, feature-name, or general prompts.
*   `history/adr/`: Stores Architectural Decision Records.
*   `CLAUDE.md`: The main configuration file for the Claude Code agent, outlining its rules and operational guidelines.

## Getting Started
To begin using this SDD Agent Framework:
1.  **Clone the repository.**
2.  **Ensure you have Git configured** (as demonstrated in previous steps: `git config --global user.email "your@example.com"` and `git config --global user.name "Your Name"`).
3.  **Interact with the AI assistant** using the provided slash commands to drive your development process. Refer to the specific command documentation (within `.claude/commands/`) for detailed usage.

## Contributing
Contributions are welcome! Please refer to the `CLAUDE.md` and the project's principles for guidelines on how to contribute effectively to this Spec-Driven Development Agent Framework.

---

🤖 Generated with [Claude Code](https://claude.com/claude-code)
