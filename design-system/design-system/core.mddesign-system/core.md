# Core Design Rules

## Purpose

Produce usable, coherent, premium interfaces rather than collections
of unrelated visual effects.

## Existing projects

- Reuse existing components and design tokens.
- Follow the current framework and repository conventions.
- Avoid new dependencies unless necessary.
- Preserve working behavior during visual changes.

## Hierarchy

- Make the primary action easy to identify.
- Use clear headings and logical reading order.
- Give related content consistent grouping.
- Keep decorative elements subordinate to useful content.

## Layout

- Use a consistent spacing scale.
- Support small screens without hiding essential content.
- Avoid fixed heights for text-heavy content.
- Use content-driven breakpoints.
- Keep body-text line lengths comfortable.

## Typography

- Use no more than two font families by default.
- Keep essential text readable.
- Reserve experimental typography for short, nonessential accents.
- Use available fonts or appropriate fallbacks.
- Do not assume permission to download commercial fonts.

## Color and surfaces

- Use semantic tokens for colors, spacing, radii, and elevation.
- Keep interactive states distinguishable.
- Do not use visual effects to compensate for unclear hierarchy.

## Content

- Prefer clear labels over clever but ambiguous wording.
- Use realistic sample content without inventing customer claims,
  testimonials, certifications, or performance statistics.
- Do not use manipulative interface patterns.

## Motion

- Use motion only to communicate state, continuity, or feedback.
- Respect reduced-motion preferences.
- Never require animation to understand essential information.

## Delivery

- Explain the selected visual direction briefly.
- Describe important implementation changes.
- Report tests actually run and checks not completed.
- Never claim full accessibility compliance from a visual inspection.
