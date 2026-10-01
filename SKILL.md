---
name: kate-xu-storytelling
description: Add selective narrative infographics to an existing presentation deck. Use when a user supplies a finished or substantially complete PPT, PDF export, or viewable slide deck and wants hard-to-explain research, location, debate, decision, or system scenes turned into illustrations that match the deck. Do not use to create an entire case study or presentation from an oral story alone.
---

# Kate Xu Storytelling

Improve an existing presentation by turning a few hard-to-explain scenes into concise narrative illustrations. The deck already owns the story, sequence, typography, and visual identity. This skill identifies where illustration adds clarity, lets the user choose one illustration direction, and integrates that direction into the existing deck.

## Product boundary

The required input is an existing presentation: preferably a PPTX, or a readable PDF export, Figma Slides link, Google Slides link, or equivalent deck source. It must already contain a meaningful story and an established visual language.

If no deck is available, ask the user to provide it and stop this workflow. This skill does not:

- turn an oral project story into a complete presentation;
- interview the user to author every slide;
- choose a presentation template;
- create a new deck-wide visual language;
- illustrate every page;
- replace another slide-authoring skill.

Preserve the deck's structure and strengthen only the scenes where illustration materially improves comprehension.

## Workflow

### 1. Read the complete deck

Inspect every slide, its visible text, speaker notes when available, and the visual relationship between adjacent slides. Build a compact internal inventory:

| Slide | Narrative job | Key claim | Evidence | Current communication issue |
|---|---|---|---|---|

Understand the causal sequence before selecting any page for illustration. Do not infer a claim from a single slide when the surrounding slides change its meaning.

### 2. Extract the deck's visual language

Treat the supplied presentation as the only visual source of truth. Identify:

- heading, body, and label fonts and weights;
- dominant background, text, accent, and supporting colors;
- shape, corner, stroke, shadow, icon, image, and spacing language;
- illustration or diagram conventions already present;
- slide aspect ratio and the available insertion area on each candidate slide.

Verify fonts and colors from the source file or inspectable design properties when possible.

For every infographic, select four or fewer colors from the existing deck, including the background and primary ink color. Preserve their established roles. Do not ask the user to choose a new palette and do not introduce an unrelated color system.

### 3. Find the scenes that earn illustration

An illustration earns its place when it compresses a relationship, setting, argument, or causal sequence that currently takes too much effort to understand.

Strong candidates include:

- research or interviews followed by synthesis;
- a physical or social setting that affected the work;
- a disagreement, strategic fork, or tradeoff;
- a discovery barrier or hidden-value scene;
- evidence becoming a pattern and then a decision;
- a feedback loop or many-to-one transformation;
- a system whose actors and relationships are difficult to explain with prose alone.

Score each candidate from 0–2 on spatial value, relational value, causal value, compression value, and memorability. A total of 6 or higher is a strong default threshold.

Select only a few scenes. For most decks, two to four infographic interventions are enough. Avoid three consecutive infographic-heavy slides. Preserve screenshots, product evidence, data, and whitespace between illustrated peaks.

### 4. Let the user choose and adjust the scenes

Read [references/scene-selection-interface.md](references/scene-selection-interface.md) before presenting candidate scenes.

Present up to five strong candidates using their semantic scene names and source slide ranges. Do not expose serial numbers or internal IDs. Each candidate must show a recognizable slide thumbnail, one direct sentence describing what is currently hard to understand, and one proposed visual focus. Preselect the agent's recommended two to four scenes while keeping every candidate editable.

The user decides two things in this checkpoint:

1. which scenes should become illustrations;
2. what each selected illustration should help the audience understand.

Allow the user to select or deselect candidates, edit the proposed visual focus, and add a missed scene in their own words. When a missed scene is entered, search the deck and open the Scene Locator defined in the reference: propose the most likely continuous slide range, let the user adjust its start and end, confirm the scene name and visual focus, then return the named scene to the selection list. In a plain chat fallback, accept scene names such as `Coffee-shop field study` and `Strategic fork`, followed by any focus edits.

Treat the confirmed scene set as the intervention plan. Use only facts already supported by the deck and supplied artifacts. Ask a focused question when a selected scene depends on missing or ambiguous evidence. Never invent metrics, quotes, participants, causality, or outcomes.

### 5. Let the user choose the illustration direction

Read [references/agent-choice-interface.md](references/agent-choice-interface.md) before presenting choices.

Choose one representative scene from the confirmed scene set. Generate exactly four 4:3 previews that use:

- the same scene and verified facts;
- the same content density;
- the same deck-derived typography;
- the same deck-derived palette of four or fewer colors;
- different illustration or composition treatments appropriate to that scene.

Present the previews at a directly readable size in a wide 2×2 grid. Put only the plain black letters A, B, C, and D beneath them. End with the localized equivalent of: `Reply A, B, C, or D to continue.`

The user's single-letter response is the complete style selection. Confirm the choice in one sentence and continue production without another approval loop.

### 6. Produce and integrate the selected illustrations

Apply the chosen visual direction only to the approved infographic scenes. Adapt each final asset to the target slide's actual insertion area while preserving the selected style.

Keep canonical claims, nuanced explanations, and accessibility-critical wording as editable slide text whenever possible. Use the illustration to communicate people, place, relationships, movement, hierarchy, or causality. Keep text inside raster artwork short.

Preserve unaffected slides, slide order, and existing brand decisions. Make broader deck changes only when the user explicitly asks for them.

## Illustration rules

### Human detail

- Use no people when data, a system, or a feedback loop carries the story.
- Use facial expressions for one or two people when emotion or dialogue is central.
- Use simplified faces for three or four people only when individual roles matter.
- Remove facial detail in groups larger than four. Show diversity and dynamics through silhouette, hair, clothing, posture, gesture, spacing, and environment.
- Isolate an important pair when one relationship matters inside a larger crowd.

### Evidence and judgment

Distinguish what happened from what the team concluded. When useful, visualize the chain:

`raw evidence → pattern questions → assisted synthesis → human judgment → decision`

Represent AI according to its actual role. Preserve the human decision that accepted, rejected, or reframed its output.

### Page integration

- Match the deck's font family, weight, palette, and spacing.
- Use page-colored or transparent backgrounds unless the deck clearly uses framed artwork.
- Avoid repeating the slide title inside the illustration.
- Give every arrow, box, person, and object a narrative purpose.
- Keep labels short and preserve enough whitespace for immediate grouping.
- Use motion only when it reveals sequence or causality and preserve reduced-motion behavior in HTML-based decks.

## Final quality gate

Verify that:

- the source deck was supplied and remains the narrative foundation;
- only the strongest hard-to-explain scenes were illustrated;
- the user selected scenes by semantic name and slide range and could adjust each visual focus;
- every user-added scene has a confirmed slide range, scene name, and visual focus;
- the selected direction came from a clear A/B/C/D choice;
- each infographic uses four or fewer colors sampled from the deck;
- typography and shape language remain consistent with the deck;
- every illustration clarifies a relationship, setting, argument, or causal sequence;
- all claims remain factual and confidential material stays protected;
- unaffected slides and settled design decisions remain unchanged;
- the reader can understand the improved scene without opening or zooming the preview.
