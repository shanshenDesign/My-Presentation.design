id: holographic
name: Holographic / Iridescent
essence: "Color that depends on where you stand. Shifting spectrum foils, oil-slick sheens, future-prism energy."
mood: [futuristic, playful-premium, magical, kinetic]

palette:
  base: "#0E0E14"          # dark lets holo shine, OR "#F4F4FA" pearl-white base
  spectrum: "linear-gradient(120deg, #A8C0FF, #C77DFF, #7DFFD4, #FFF07D, #FF9EC6, #A8C0FF)"
  ink_on_dark: "#F2F2FA"
  ink_on_light: "#2A2A35"
  note: "The holo spectrum is an ACCENT material (≤15% of surface). The base stays quiet so the shift reads."

typography:
  display: ["Clash Display", "Space Grotesk", "Unbounded"]
  body: ["Inter", "Space Grotesk"]
  rules: "Bold geometric display; one hero word may carry the holo gradient (background-clip: text). Rest stays solid."

texture_technique:
  - "Iridescent gradient that shifts hue on scroll/pointer (rotate gradient angle ±30°)"
  - "Foil-card effect: conic-gradient sheen following cursor"
  - "Fine prismatic edge-light on cards (1px gradient border)"
  - "Subtle dispersion: 1px RGB split on hero edges only"

layout:
  grid: "Clean modern product grid — the holo is the material, not the layout."
  spacing: "Contemporary and confident."
  frames: "Gradient borders; glass panels with spectral edges."

motion:
  style: "The gradient IS the motion: continuous slow hue rotation (12s loop), pointer-tracked foil on cards."
  duration: hero
  forbid: [nothing-else-moves: keep other motion minimal so holo leads]

imagery:
  treatment: "Iridescent 3D shapes, foil textures, prismatic light leaks, bubble/chromatic glass renders."
  signature_prompt: "holographic iridescent 3d render, shifting rainbow spectrum foil material, oil-slick sheen on smooth curved shapes, prismatic light dispersion, dark background, futuristic y2k-luxury aesthetic, chromatic glass, studio product render"

components:
  buttons: "Solid base with holo gradient border; hover makes the border flow."
  cards: "Glass panels; on hover, a foil sheen sweeps across following the cursor."
  badges: "Small holo chips for 'new/premium' markers."

dos:
  - "Tie the spectrum shift to user movement (cursor/scroll)"
  - "Keep 85% of the surface quiet base color"
  - "Use dark base for drama or pearl base for softness — never mid-gray"
donts:
  - "No holo behind body text (contrast law)"
  - "No rainbow on every element — it stops being special"
  - "No static rainbow: holographic must SHIFT"
pairs_with: [metallic-chrome, dreamy-pastel]
