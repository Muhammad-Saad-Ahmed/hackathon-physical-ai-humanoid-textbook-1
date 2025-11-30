---
id: 1764528673
title: Update Book Constitution
stage: constitution
date: 2025-11-30
surface: agent
model: claude-sonnet-4-5-20250929
feature: none
branch: master
user: user
command: /sp.constitution You are an expert AI system for creating a complete Spec-Driven Book using Spec-Kit Plus and Claude Code. Generate a high-level constitution for a book titled: "Physical AI {{COMMAND}} Humanoid Robotics — From Digital Intelligence to Embodied Intelligence" The constitution must describe only high-level rules, boundaries, and goals for the book. No chapters, no tasks, no detailed content — only the governing framework. The constitution must include: 1. Mission - Define that the book teaches Physical AI, Humanoid Robotics, ROS 2, Gazebo, Unity, NVIDIA Isaac, and Vision-Language-Action systems. - Focus on connecting AI agents with real/simulated humanoid robots. 2. Writing Style - Clear, structured, beginner-friendly, technical accuracy, step-by-step, no fluff. 3. High-Level Modules (just names + 1-line descriptions) - ROS 2 - Gazebo {{COMMAND}} Unity - NVIDIA Isaac - Vision-Language-Action (VLA) 4. Required Integrations (high-level only) - RAG Chatbot (OpenAI Agents/ChatKit, Qdrant, FastAPI, Neon Postgres) - BetterAuth signup/signin - Per-chapter personalization button - Urdu translation button 5. Reusable Intelligence Requirements - Claude Code Subagents + Skills (high-level, modular) 6. Output Requirements - Must produce /sp.constitution, /sp.specify, /sp.tasks, /sp.deploy - Must deploy the final book using Docusaurus + GitHub Pages. 7. Quality Standards - Technical correctness, clarity, automation-friendly, aligned with the humanoid capstone project. 8. Key Insights Section - Physical AI concept - Importance of ROS 2 - Simulation necessity - Strength of NVIDIA Isaac - Vision-Language-Action as future robotics - Personalization + RAG + Urdu accessibility benefits Make the constitution concise, high-level, and suitable for iterative refinement. Do NOT write the actual book. Just write the governing constitution rules.
labels: [[]]
links:
  spec: {{LINKS_SPEC}}
  ticket: {{LINKS_TICKET}}
  adr: {{LINKS_ADR}}
  pr: {{LINKS_PR}}
files:
- .specify/memory/constitution.md
tests:
[]
---

## Prompt

You are an expert AI system for creating a complete Spec-Driven Book using Spec-Kit Plus and Claude Code. 
Generate a high-level constitution for a book titled:

"Physical AI {{PROMPT_TEXT}} Humanoid Robotics — From Digital Intelligence to Embodied Intelligence"

The constitution must describe only high-level rules, boundaries, and goals for the book. 
No chapters, no tasks, no detailed content — only the governing framework.

The constitution must include:

1. Mission  
   - Define that the book teaches Physical AI, Humanoid Robotics, ROS 2, Gazebo, Unity, NVIDIA Isaac, and Vision-Language-Action systems.  
   - Focus on connecting AI agents with real/simulated humanoid robots.

2. Writing Style  
   - Clear, structured, beginner-friendly, technical accuracy, step-by-step, no fluff.

3. High-Level Modules (just names + 1-line descriptions)  
   - ROS 2  
   - Gazebo {{PROMPT_TEXT}} Unity  
   - NVIDIA Isaac  
   - Vision-Language-Action (VLA)  

4. Required Integrations (high-level only)  
   - RAG Chatbot (OpenAI Agents/ChatKit, Qdrant, FastAPI, Neon Postgres)  
   - BetterAuth signup/signin  
   - Per-chapter personalization button  
   - Urdu translation button  

5. Reusable Intelligence Requirements  
   - Claude Code Subagents + Skills (high-level, modular)

6. Output Requirements  
   - Must produce /sp.constitution, /sp.specify, /sp.tasks, /sp.deploy  
   - Must deploy the final book using Docusaurus + GitHub Pages.

7. Quality Standards  
   - Technical correctness, clarity, automation-friendly, aligned with the humanoid capstone project.

8. Key Insights Section  
   - Physical AI concept  
   - Importance of ROS 2  
   - Simulation necessity  
   - Strength of NVIDIA Isaac  
   - Vision-Language-Action as future robotics  
   - Personalization + RAG + Urdu accessibility benefits

Make the constitution concise, high-level, and suitable for iterative refinement. 
Do NOT write the actual book. 
Just write the governing constitution rules.

## Response snapshot

The constitution has been updated to version 1.1.0. This is a minor version bump due to the addition of new principles and content. Files flagged for manual follow-up: .specify/templates/plan-template.md, .specify/templates/spec-template.md, .specify/templates/tasks-template.md, .claude/commands/*.md. Suggested commit message: docs: amend constitution to v1.1.0 (principle additions + governance update)

## Outcome

- ✅ Impact: {{OUTCOME_IMPACT}}
- 🧪 Tests: {{TESTS_SUMMARY}}
- 📁 Files: {{FILES_SUMMARY}}
- 🔁 Next prompts: {{NEXT_PROMPTS}}
- 🧠 Reflection: {{REFLECTION_NOTE}}

## Evaluation notes (flywheel)

- Failure modes observed: {{FAILURE_MODES}}
- Graders run and results (PASS/FAIL): {{GRADER_RESULTS}}
- Prompt variant (if applicable): {{PROMPT_VARIANT_ID}}
- Next experiment (smallest change to try): {{NEXT_EXPERIMENT}}
