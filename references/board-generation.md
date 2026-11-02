# Board generation

Use this reference for the final presentation board or a board revision.

## Visual grammar

Default to a horizontal 3:2 board unless the user specifies another format.

- **Top 45–55%:** title, short problem/solution, product hero, and one dominant human use scene.
- **Lower 35–45%:** three to five numbered steps, components, state comparison, maintenance or service loop.
- **Bottom 5–8%:** four-column information strip: Category, Concept, Target, Status.
- White or warm-white field, one primary accent, one warning/secondary accent, charcoal text.
- Large title and scenario first; process second; components third; values last.
- Use leader lines only for information that changes understanding.

## Board copy budget

- Title: 1–3 words.
- Subtitle: 5–10 words.
- Problem: 25–45 words.
- Solution: 25–50 words.
- Steps: 3–5, each with a one-word verb and 6–14 words.
- Components: 4–6 short labels.
- Values: exactly three, each with a title and one line.
- Footer: Category / Concept / Target / Status.

Prefer mechanism, maintenance, and system ownership over inspiration statements. Do not describe visible aesthetics in the body copy.

## Input-image roles

Explicitly label every image in the generation prompt:

- **Product master:** exact geometry and CMF to preserve.
- **Layout reference:** hierarchy and density only; never copy product or identity.
- **Supporting reference:** material, environment, or technical detail only.

If no product master exists, define the product system with enough physical specificity that every view can remain coherent.

## Direct board prompt template

```text
Use case: infographic-diagram
Asset type: complete horizontal 3:2 iF-style student design award board
Primary request: Design and present <NAME>, <one-line proposition>.

Input images:
- Image 1... are layout references only. Learn white field, dominant scenario,
  product hero, concise steps, callouts and footer. Do not copy products,
  logos, people, watermarks or exact compositions.

Product-service system:
- <physical component, geometry, CMF, material>
- <second component>
- <service/maintenance element>
- <privacy/safety boundary>

Interaction:
<before -> key action -> feedback -> after -> return/maintenance>

Layout:
- <palette and top/bottom bands>
- upper-left title and concise statement
- center-left faithful product hero
- upper-right dominant realistic use scene
- lower section numbered steps, components, service loop and three values
- bottom four-column information strip

Style:
premium industrial/product/service design award board, photorealistic
editorial scenario, precise render, Swiss grid, generous white space

Exact English text:
"<TITLE>"
"<SUBTITLE>"
"<PROBLEM>"
"<SOLUTION>"
"HOW IT WORKS"
"01 <VERB>"
"<step copy>"
...
"SYSTEM COMPONENTS"
...
"<VALUE 1>"
"<value copy>"
...
"Category  <category>"
"Concept  <name>"
"Target  <audience>"
"Status  Design concept"

Constraints:
same product identity in every view; <safety and ethical boundaries>;
no iF logo or award claim; no fake entrant details, QR code, email,
watermark or unsupported statistics; readable concise text

Avoid:
<topic-specific failure modes>, distorted hands, duplicated components,
dense illegible microtext
```

## Two-stage generation rule

Generate a product master first when the concept has:

- multiple views of a complex mechanism;
- components that must remain identical across states;
- a distinctive form likely to drift;
- a board that depends on an exploded view.

Generate the board directly when the system is architecturally simple and the prompt can define all components unambiguously. If the first board shows inconsistent geometry, do not keep rewording the whole prompt: generate a master and use it as the exact product reference.

## Saving

Use a project folder such as:

```text
<workspace>/<concept-slug>/output/
  <concept-slug>_product_concept_v1.png
  <concept-slug>_competition_board_v1.png
```

Never overwrite a prior version unless the user explicitly requests replacement.

