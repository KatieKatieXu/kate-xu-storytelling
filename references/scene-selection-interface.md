# Scene Selection Checkpoint

Use this checkpoint after reading the complete deck and scoring the scenes that could benefit from illustration. It decides which scenes receive illustrations and what each illustration must communicate.

## Use human-readable scene names

- Identify every candidate by its semantic scene name and source slide range.
- Keep serial numbers and internal IDs hidden from the user.
- Reserve `A` through `D` for the later illustration-direction choice.

Examples:

- `Coffee-shop field study · Slides 5–6`
- `Discovery barrier · Slides 9–10`
- `Founder debate and product pivot · Slides 10–13`

## Build the candidate shortlist

Show up to five of the strongest scenes. Rank additional candidates internally and omit them from the first screen. The user may add a missed scene afterward.

Every candidate must include:

- a short scene name grounded in the deck;
- the source slide number or range;
- a recognizable thumbnail from the supplied deck;
- one sentence describing what is currently hard to understand;
- one editable sentence beginning with the intended audience takeaway, such as `Help the audience understand…`.

Preselect the agent's recommended two to four scenes. Base the recommendation on spatial, relational, causal, compression, and memorability value. Avoid recommending adjacent scenes that repeat the same narrative job.

## Give the user three controls

1. **Select or deselect** each named scene.
2. **Adjust the visual focus** by editing the audience-takeaway sentence.
3. **Add a missed scene** by describing the missing story in their own words.

The focus field changes the communication goal while preserving the deck's facts. Examples:

- `Discovery barrier: emphasize the participant's hesitation before discovering the editor.`
- `Strategic fork: show the two options and the founder discussion.`
- `Add scene: illustrate the feedback loop between applications and market position.`

## Resolve a missed scene with the Scene Locator

When the user writes something in `Add a missed scene`, treat their wording as a search query across the full deck.

1. Find the slides whose text, notes, and neighboring context best match the requested scene.
2. Propose one continuous story range, including the first slide that establishes the situation and the last slide that completes the consequence or decision.
3. Show that range as a filmstrip with the selected slides highlighted and at least one neighboring slide on each side when available.
4. Let the user adjust `Start slide` and `End slide` independently.
5. Generate a concise scene name and an editable `Help the audience understand…` focus statement.
6. Confirm the result with its scene name and slide range, select it by default, and return it to the main scene list.

The live confirmation should read like: `Founder debate and product pivot · Slides 10–13`.

Prefer a continuous range of one to four slides. Allow a longer range when the deck clearly treats it as one scene. Split noncontiguous evidence into separate scenes instead of implying continuity.

When the query has more than one plausible location, show up to three candidates identified by scene name and slide range. The user chooses the meaningful chapter directly. Avoid visible range codes.

Validate that the start slide is not after the end slide. Ask one focused question when the wording cannot be located reliably. Never invent a slide range.

## Keep the interface compact

- Show candidate thumbnails and essential copy directly in the conversation.
- Use checkboxes or equivalent multi-select controls when the host supports them.
- Keep focus editing available without opening another page.
- Show a live summary using scene names, such as `3 scenes selected: Coffee-shop field study, Discovery barrier, Strategic fork`.
- Use one action to continue to the A–D illustration checkpoint.
- Keep slide images readable without requiring the user to open them.

When native controls are unavailable, ask for one compact reply:

```text
Coffee-shop field study; Discovery barrier; Strategic fork
Strategic fork: focus on the disagreement and the evidence that resolved it.
```

A selected scene with no edit accepts the proposed focus as written.

## Confirm and advance

After submission:

1. Summarize the selected scenes and any edits in one compact list.
2. Ask only for evidence that is genuinely missing from a selected scene.
3. Choose one representative selected scene for the A–D visual-direction previews.
4. Continue to the Four-Choice Illustration Checkpoint.

Do not reopen rejected scenes unless new evidence materially changes the story or the user asks to reconsider them.
