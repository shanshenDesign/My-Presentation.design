id: minimal-line-art
name: Minimal Line Art
essence: "One continuous stroke. Maximum meaning, minimum ink. Silence as luxury."
mood: [calm, refined, intelligent, serene]

palette:
  bg: "#FAFAF7"            # warm off-white
  ink: "#1A1A1A"
  muted: "#9B9B93"
  accent: "#B08968"        # optional warm taupe, used <5%
  note: "Essentially monochrome. Color, if any, is a whisper."

typography:
  display: ["Cormorant Garamond", "Fraunces", "EB Garamond"]
  body: ["Inter", "Source Sans 3", "Karla"]
  rules: "Light weights, generous letter-spacing on labels (0.12em uppercase). Serif display + quiet sans body. Small sizes, huge whitespace."

texture_technique:
  - "Single-weight line illustrations (1–1.5px), continuous-line style"
  - "Hairline dividers (1px, 12–16% black)"
  - "No fills, no shadows, no texture"

layout:
  grid: "Vast negative space (60–75% empty). Content in a narrow centered measure."
  spacing: "Double the default section gaps (128px+)."
  frames: "None. Space itself separates."

motion:
  style: "Lines draw themselves on scroll (stroke-dashoffset). Everything else: slow, 400–600ms fades."
  duration: slow
  forbid: [parallax-layers, bouncy, scale-pops]

imagery:
  treatment: "Line drawings only, or photography reduced to near-monochrome with heavy whites."
  signature_prompt: "minimalist continuous line art illustration, single black line on warm white background, elegant one-line drawing, extreme simplicity, generous negative space, gallery aesthetic"

components:
  buttons: "Hairline-bordered ghost buttons; hover fills with 4% ink tint."
  cards: "No card chrome at all — space and a hairline do the work."
  nav: "Bare words, wide tracking, hairline underline on hover."

dos:
  - "Remove an element; if nothing breaks, remove another"
  - "Let one line drawing carry the entire hero"
  - "Keep contrast accessible despite the whisper palette (ink on bg must pass 4.5:1)"
donts:
  - "No color blocks, no heavy weights, no drop shadows"
  - "No more than one illustration per viewport"
  - "Never fill the whitespace because it 'looks empty'"
pairs_with: [japanese-ink, botanical]
