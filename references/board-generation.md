# Board generation

Use this reference for the final presentation board or a board revision.

## Visual grammar

Default to a horizontal 3:2 board unless the user specifies another format. Select one layout family from [layout-pattern-library.md](layout-pattern-library.md) before writing the prompt.

Across layout families:

- Reserve 60–75% of the board for visual explanation and 25–40% for text.
- Give one hero image or use scene 35–55% of the active canvas; do not distribute emphasis evenly.
- Use two to four secondary modules: mechanism, sequence, components, evidence, maintenance, or material loop.
- Keep the bottom 5–8% as a quiet information strip: Category, Concept, Target, Status.
- Use a white or warm-white field and one main accent. A full-width red band is optional legacy styling, not an iF requirement.
- Make the reading order visible at thumbnail size: title and proposition first, hero/action second, proof third, details last.
- Use line drawings for secondary explanation and photorealistic rendering for the hero. Mixing modes is useful when hierarchy is clear.
- Use leader lines only where they explain mechanism, assembly, or state change.

## Board copy budget

- Title: 1–3 words.
- Subtitle: 5–10 words.
- Problem: 25–45 words.
- Solution: 25–50 words.
- Steps: 3–5, each with a one-word verb and 6–14 words.
- Components: 4–6 short labels.
- Values: exactly three, each with a title and one line.
- Footer: Category / Concept / Target / Status.

Target 70–140 English words outside labels and footer. A board that needs long paragraphs probably lacks visual proof or has not selected its core claim.

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
- Image 1... are labout references only. Learn white field, dominant scenario,
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
- layout family: <Hero + mechanism / Scenario + intervention /
  Product-service system / Material + lifecycle / Wearable + validation>
- one dominant proof image: <hero, use scene, material family, or wearing view>
- two or three supporting modules chosen from mechanism, sequence,
  components, evidence/validation plan, maintenance, and lifecycle
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

## Evidence rule

Use evidence modules only when the project has evidence. Prototype photos, user quotes, charts, test results, and clinical or environmental claims must come from supplied or completed research. Otherwise label the module `VALIDATION PLAN`, show what will be tested, and avoid fabricated numbers or photographs that imply a completed study.

## Saving

Use a project folder such as:

```text
<workspace>/<concept-slug>/output/
  <concept-slug>_product_concept_v1.png
  <concept-slug>_competition_board_v1.png
```

Never overwrite a prior version unless the user explicitly requests replacement.
