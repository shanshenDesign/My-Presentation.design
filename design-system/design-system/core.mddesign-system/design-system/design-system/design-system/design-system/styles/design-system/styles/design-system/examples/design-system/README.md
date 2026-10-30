# AI Design Routing System

A repository-local system for choosing and applying a coherent,
premium visual direction.

## Usage

Give the AI a brief describing:

- What is being built
- Who will use it
- Desired emotional tone
- Content density
- Formality
- Existing brand constraints
- Whether it is a presentation deck or product interface

Ask it to follow `AGENTS.md` and `design-system/routing.md`.

Example:

"Create a premium futuristic product-launch presentation for [topic].
Use a confident narrative, restrained visual effects, readable data,
and purposeful motion. Follow the repository's design routing system."

## Architecture

- `routing.md`: Decision process and output contract.
- `style-index.yaml`: Metadata for comparing all styles.
- `core.md`: Shared interface rules.
- `accessibility.yaml`: Mandatory accessibility requirements.
- `quality-bar.md`: Presentation-quality requirements.
- `tokens.yaml`: Starter semantic design tokens.
- `styles/`: Detailed visual profiles.
- `examples/briefs.yaml`: Manual routing checks.

## Presentation standard

A high-level presentation is not simply a visually busy screen.

It must communicate its purpose quickly, use a controlled hierarchy,
respect the brand, work without animation, meet accessibility
requirements, and use realistic content without invented claims.

## Limitations

Scoring depends on interpretation and is not guaranteed to be
identical across models.

Style profiles are starting points, not substitutes for research,
brand strategy, usability testing, or accessibility verification.

File-loading behavior depends on the AI tool and its permissions.

## Maintenance

When changing a style:

1. Update its detailed YAML.
2. Update its index entry if routing characteristics changed.
3. Review the example briefs.
4. Check for conflicts with core, quality-bar, and accessibility rules.

Do not edit accessibility requirements merely to accommodate
a visual effect.
