id: watercolor
name: Watercolor
essence: "Pigment blooming in water. Soft edges, translucent washes, and happy accidents. Romance in pigment form."
mood: [romantic, gentle, artisanal, alive]

palette:
  bg: "#FBF9F4"            # cotton paper
  ink: "#3B3A36"
  washes: ["#A8C5D6", "#E8B4B8", "#C9D6B8", "#F2D5A0", "#B8A9C9"]
  note: "Colors are always translucent (think 30–60% opacity layers). Saturated accents only in tiny pigment dots."

typography:
  display: ["Cormorant Garamond", "Playfair Display", "EB Garamond"]
  accent_script: ["Caveat", "Kalam"]  # sparingly, for signatures/labels only
  body: ["Source Serif 4", "Lora"]
  rules: "Serif throughout. Script allowed for ≤5 words per page. Never all-caps body."

texture_technique:
  - "Organic wash blobs with irregular water edges behind key content"
  - "Visible pigment pooling (darker at edges of a wash)"
  - "Paper tooth texture at 4% opacity"
  - "Occasional paint splatter (≤3 specks per section)"

layout:
  grid: "Soft grid; elements may drift slightly off-axis (2–6px) for hand-placed feel."
  spacing: "Airy. Washes need breathing room to feel wet."
  frames: "Deckle-edge panels or none."

motion:
  style: "Washes bloom in (scale 0.96→1 + opacity, 600ms, soft). Brush strokes draw on."
  duration: slow
  forbid: [hard-cuts, glitch, mechanical-snap]

imagery:
  treatment: "Watercolor illustration; photography only if painted-over/soft-focus."
  signature_prompt: "delicate watercolor painting, translucent pigment washes blooming on cotton paper, soft bleeding edges, visible paper texture, loose expressive brushwork, light airy palette, botanical or landscape subject, fine art style"

components:
  buttons: "Ink-outline buttons with a faint wash on hover that 'bleeds' to the edges."
  cards: "Paper panels with one corner wash; hairline optional."
  dividers: "A single loose brush stroke."

dos:
  - "Let one wash anchor each section"
  - "Keep edges organic — no perfect rectangles of color"
  - "Pair with generous serif typography"
donts:
  - "No neon, no hard geometry, no heavy borders"
  - "No crisp vector shapes pretending to be washes"
  - "No script font for paragraphs"
pairs_with: [botanical, dreamy-pastel]
