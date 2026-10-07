---
layout: default
title: Lessons Learned Building a 250k-Line Roblox Game with AI
date: 2026-10-07
---

# Lessons Learned Building a 250k-Line Roblox Game with AI

Developing a large-scale project in Roblox Luau involves balancing network architecture, client-server security, modular framework design, and game state management. When a project scales up to roughly 250,000 lines of code, managing complexity becomes the single biggest challenge. 

By leveraging AI as a coding assistant and architecture sounding board, I was able to rapidly prototype systems, draft complex algorithms, and refactor existing frameworks. Here is a breakdown of the core skills and engineering practices I developed throughout this process.

---

## 1. Modular Architecture & System Design
At 250,000 lines of code, a monolithic script structure quickly becomes unmaintainable. 

* **Component-Based Frameworks:** I relied heavily on modular architectures (such as ModuleScripts paired with frameworks like Knit or custom OOP structures) to decouple game logic.
* **Separation of Concerns:** Splitting data handling, UI logic, server replication, and physics controllers into distinct, self-contained modules ensured that updating one system wouldn't break another.
* **AI Integration:** AI excel at generating clean boilerplate for new modules, allowing me to focus on high-level system interactions rather than repetitive setup code.

---

## 2. Advanced Prompt Engineering & Code Auditing
Working with AI on a large codebase requires moving past simple prompts to structured engineering workflows.

* **Context Window Management:** Because AI models have context limits, I learned to extract and feed only the relevant interface definitions, types, and module.
* **Reiteration For Quality** You need to be rather specific with some of the prompts needed to create with the use of AI. An example would be a visual effect prompt such as: Make an arcane tarot skill fitting out game art. A deck of ornate cards appears floating in front of the player's chest and fans out into a wide arc, each card spinning in place with a faint glint along its edge. Three cards slide out of the fan one at a time and flip face-up with a sharp flash, each showing a different glowing arcane symbol, while the rest of the deck dissolves into sparks. After a short beat, the three cards launch toward a target point about 45 studs away, spinning edge-first like blades and curving in on slightly different paths. They land one after another, each one stabbing upright into the ground and projecting its symbol as a ring of light beneath it, and once all three are planted, lines of light connect them into a triangle that collapses inward and detonates in a sharp burst of runes and shredded card fragments. It should feel mysterious, elegant and precise, with a deep violet, midnight black and burnished gold palette with sharp white highlights on the symbols and card edges, not soft or whimsical. Draw custom textures in Blender (the card back, three card faces with distinct symbols, the edge-glint trails, the symbol rings, and the burst fragments) and preview them in an Artifact before uploading anything; only upload the final set.
