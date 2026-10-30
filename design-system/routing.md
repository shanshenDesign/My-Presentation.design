# Style Routing Protocol

## Objective

Select exactly one primary visual style and zero or one supporting
style for a design brief.

Make the decision explainable, repeatable, and accessible.

## Scope

Use this process for visual interface design and substantial
visual redesigns.

Do not reroute for minor bug fixes unless the visual direction changes.

## Rule precedence

Within this design system, resolve conflicts in this order:

1. accessibility.yaml
2. Explicit project constraints and existing brand requirements
3. core.md
4. quality-bar.md
5. Primary style
6. Supporting style

Style selection never authorizes violating a higher-priority rule.

If project requirements conflict with accessibility rules, identify
the conflict and propose an accessible alternative.

## Required files

Read:

- design-system/accessibility.yaml
- design-system/core.md
- design-system/style-index.yaml
- design-system/quality-bar.md
- design-system/tokens.yaml

After routing, read:

- design-system/styles/{primary}.yaml
- design-system/styles/{supporting}.yaml, if supporting is not null
- design-system/styles/ultimate-presentation.yaml, when the task
  is a presentation deck or high-impact visual narrative

Read routing metadata for all seven styles, but do not load all
seven detailed style files.

If a required file is missing or unreadable:

- Set status to "blocked".
- Report the exact path.
- Do not invent replacement content or continue implementation.

## Extract signals

Extract the following from the brief:

- topic: Short description of the requested experience.
- industry: Free-text domain, or "unknown".
- audience: Free-text audience, or "unknown".
- audience_age_min: Minimum intended age, or null if unspecified.
- emotion: Up to two values from:
  calm, focus, premium, expressive, playful, raw, rebel,
  technical, friendly.
- density: One of:
  minimal, balanced, data-heavy, explain-a-system, unknown.
- formality: Integer 0–10, or null if unspecified.
- context: Zero or more of:
  data, ai, dashboard, editorial, commerce, education,
  marketing, product, presentation.
- preferred_style: One of the supported style IDs, or null.

Use explicit information before inference.
Record inferred signals in assumptions.
Do not infer audience age from a visual aesthetic.

If formality must be inferred, use:

- 0–3: Casual, informal, or irreverent.
- 4–7: Professional and approachable.
- 8–10: Ceremonial, prestige-oriented, or highly formal.

Do not treat a regulated industry alone as proof of high formality.

If the brief names conflicting preferred styles without ranking them,
ask one clarification question before proceeding.

## Missing information

If the brief contains a usable topic, proceed with unknown values
and record assumptions.

If neither the topic nor intended experience is understandable,
ask one concise clarification question.

Unknown signals receive a neutral rating of 5.
Do not turn unknown information into invented requirements.

## Score every style

Score all seven styles against five dimensions:

- industry
- audience
- emotion
- density
- formality

Allowed dimension ratings:

- 0: Direct contradiction.
- 2: Weak fit; substantial adaptation required.
- 5: Neutral, unknown, or mixed evidence.
- 8: Strong fit.
- 10: Explicitly aligned with the style profile.

Use style-index.yaml as the comparison reference.
These profiles express preferences, not bans on particular industries.

Apply weights:

- industry: 1
- audience: 2
- emotion: 3
- density: 2
- formality: 2

Calculate:

score = (
  industry_rating
  + 2 * audience_rating
  + 3 * emotion_rating
  + 2 * density_rating
  + 2 * formality_rating
) / 10

Round to one decimal place.
Final scores must be between 0 and 10.

Record dimension ratings as well as final scores.

Ratings are judgments. Use the same interpretation across all styles.

## Select primary

If the brief explicitly requests one supported style, select it
as primary and record selection_method as "explicit".

Otherwise:

1. Find the highest final score.
2. Collect styles with that score after rounding.
3. If only one remains, select it.
4. If multiple remain, apply the tie-breakers below.

Tie-breakers only choose among tied candidates.
They do not override a higher-scoring style.

Apply in this order:

1. audience_age_min < 13: kawaii.
2. density = explain-a-system: isometric.
3. formality >= 8: luxury.
4. emotion includes raw or rebel:
   streetwear, then deconstructivism.
5. emotion includes calm or focus: japandi.
6. context includes data, ai, or dashboard: futuristic.

For each rule, select the first listed style that is a tied candidate.
If none matches, continue to the next rule.

If a tie remains, use this fixed order:

japandi, futuristic, isometric, luxury, kawaii,
streetwear, deconstructivism.

This final order is a repeatability fallback, not a quality ranking.

## Select supporting

A supporting style is optional.

A candidate must:

- Not be the primary style.
- Score at least 6.0.
- Share at least one exact core-value label with the primary.
- Have a useful, specific contribution that does not conflict
  with the primary, accessibility rules, or project requirements.

Filter candidates for eligibility before ranking them.

Select the eligible candidate with the highest score.
Resolve equal scores using the same fixed fallback order.

If no eligible candidate exists, set supporting to null.

If the brief requests a single style, set supporting to null.

Never select two supporting styles.

Record the shared values and the supporting style's permitted
contribution. If no useful contribution can be named, use null.

## Compose the design

The primary controls:

- Overall layout language
- Typography hierarchy
- Main palette direction
- Component geometry
- Visual tone

The supporting style may influence only one named area:

- Illustrations
- Accent colors
- Surface treatment
- Decorative typography
- Nonessential motion

Do not mix two competing layout systems.

Existing brand requirements take precedence over style defaults.
Do not replace an established logo or brand palette without permission.

## Presentation decks

For a presentation deck, product launch, pitch, conference talk,
or portfolio presentation:

1. Read ultimate-presentation.yaml.
2. Use the narrative sequence:
   cover, thesis, context, insight, solution, evidence, impact,
   and call to action.
3. Give each slide one dominant message.
4. Use premium editorial typography and an intentional grid.
5. Use restrained futuristic atmosphere when appropriate:
   gradients, grid texture, layered surfaces, controlled glow,
   and purposeful motion.
6. Do not let effects reduce readability, contrast, or clarity.
7. Ensure the deck works without animation.
8. Respect prefers-reduced-motion.
9. Do not invent metrics, customers, testimonials, certifications,
   awards, or performance claims.

Use a user-provided example deck only as a reference for desired
energy, density, hierarchy, and motion.

Do not copy it exactly unless explicitly instructed.

## Output contract

Include one JSON decision object in the response.

Required fields:

- status: "ready" or "blocked"
- topic
- signals
- assumptions
- dimension_ratings
- scores
- primary
- supporting
- selection_method
- shared_values
- supporting_scope
- why
- files_read
- warnings
- presentation_review

The exact JSON structure is defined in AGENTS.md.

Do not present invented file reads or verification results.

Return the log in the response by default.
Persist it to a repository file only when requested.

## Verification

Before delivery, verify:

- All seven styles were scored.
- The score formula was applied correctly.
- Exactly one primary and at most one supporting were selected.
- Supporting eligibility was checked before ranking.
- Accessibility rules were not weakened by style choices.
- Existing project constraints were preserved.
- The decision object matches the selected implementation.
- The result meets all applicable quality-bar requirements.

Report which checks were performed and which remain unverified.
