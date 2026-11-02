---
name: if-student-concept-board
description: Research current iF Design Student Award patterns, develop distinctive SDG-aligned product or service concepts, and generate polished horizontal competition boards with ImageGen. Use when a user asks for iF competition topics, wants to develop a concept like TACTILE CITY, requests an iF-style board, or wants to iterate a student design-award entry.
metadata:
  short-description: Build researched iF student concepts and boards
---

# iF Student Concept Board

Turn a social, cultural, environmental, or everyday-life issue into a credible student design concept and a presentation board that can be understood without a live pitch.

## Required outcome

Produce the smallest complete set appropriate to the request:

- a current award-pattern summary when topic selection is still open;
- a concept brief with problem, user, intervention, system boundary, and feasibility;
- a coherent product/service family and interaction sequence;
- concise English board copy;
- one or more horizontal 3:2 board images generated with the available image-generation workflow;
- saved workspace paths and a short Chinese explanation.

Do not stop at a slogan, isolated object, or attractive rendering. The concept must explain who uses it, what changes, how it works, and what happens before and after the key interaction.

## Workflow

1. **Read the user's references and history.** Separate layout references from instructions. Preserve explicit topic, audience, palette, and deliverable choices.
2. **Research before ideating when the user asks for current winning patterns.** Use official iF sources first and read [research-and-concept.md](references/research-and-concept.md).
3. **Frame several directions before rendering.** Avoid repeatedly returning to medical devices, emergency products, sensor-plus-app concepts, or cute child products unless the brief calls for them.
4. **Score the promising directions.** Use problem-solving, ethics/positive experience, solidarity, design relevance, and economic feasibility. Reject concepts whose main value depends on unsupported technical claims.
5. **Build a system, not feature stacking.** Define the physical product, service actors, consumables or replaceable parts, maintenance, privacy/safety boundary, and end-of-life path.
6. **Lock visual identity before generation.** Specify geometry, CMF, materials, key controls, component count, and state changes. For complex products, generate a product master before the board; for well-bounded systems, a direct board generation is acceptable.
7. **Write the board in English.** Keep the title, one-sentence problem, one-sentence solution, three to five steps, components, three value statements, and footer. The official application does not accept Chinese descriptions.
8. **Generate with ImageGen.** Read the `imagegen` skill before image work. Label every input image as product master, layout reference, or supporting reference. Never ask the model to copy a reference product or award logo.
9. **Save every final board into the workspace.** Use versioned descriptive names and keep generated project assets out of temporary-only locations.
10. **Review before delivery.** Read [quality-checklist.md](references/quality-checklist.md), fix material inconsistencies or misleading claims, and report limitations that require prototyping.

## Board construction

Read [board-generation.md](references/board-generation.md) whenever generating or revising a board. It contains the layout grammar, copy limits, and prompt template.

For the reasoning path that produced TACTILE CITY, read [tactile-city-case-study.md](references/tactile-city-case-study.md). Use it as a method example, not as a subject constraint.

## Non-negotiable constraints

- Do not place an iF winner logo or claim an award before the project wins.
- Do not invent designers, universities, entry numbers, email addresses, QR codes, test results, patents, certifications, or impact statistics.
- Do not describe a concept as medically diagnostic, absolutely safe, waterproof, fraud-proof, or environmentally restorative without evidence.
- Do not use a phone app as the default answer when a physical or service interaction is central.
- Do not copy the product, people, logo, title, or exact composition from a reference board.
- Keep the board legible at one-screen scale. Remove text before shrinking it into unreadable microcopy.
- State what the product does **not** prove or replace when that boundary affects safety or ethics.

## Reusable assets

The `assets/` folder contains the finished TACTILE CITY board as a case-study reference. Treat it only as a visual hierarchy and workflow reference. Product content must always be newly designed. When users provide their own layout references, label them as layout references and never copy their products, logos, people, or exact compositions.
