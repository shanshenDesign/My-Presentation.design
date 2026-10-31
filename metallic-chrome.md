id: metallic-chrome
name: Metallic Chrome
essence: "Liquid metal. Mirror reflections, Y2K attitude, and surfaces polished to vanity. Premium industrial seduction."
mood: [sleek, luxurious, cold-precise, futuristic-retro]

palette:
  bg: "#0C0C0E"            # near-black
  surface: "#16161A"
  ink: "#F2F2F5"
  metal: "linear-gradient(135deg, #D7D7DD 0%, #8E8E99 25%, #F5F5FA 50%, #77777F 75%, #C9C9D2 100%)"
  accent: "#9BA4FF"        # one cold accent, optional
  note: "Chrome is a GRADIENT SYSTEM, not a color. Everything metal reflects a horizon: light top, dark middle, light bottom."

typography:
  display: ["Space Grotesk", "Clash Display", "Sora"]
  body: ["Inter", "Space Grotesk"]
  rules: "Display may use chrome gradient fill on huge type (background-clip: text) — hero words only, never body. Tight tracking (-0.02em)."

texture_technique:
  - "Chrome text/objects: multi-stop silver gradient + subtle environment reflection stripes"
  - "Brushed-metal surfaces: fine horizontal lines at 2–3% opacity"
  - "Specular highlights: small hard white glints on edges"
  - "Dark reflective floors under hero objects (mirror fade)"

layout:
  grid: "Showroom layout: one hero object center-stage on a dark reflective plane."
  spacing: "Premium emptiness around the hero; dense spec-sheets below in clean grids."
  frames: "Hairline silver borders (1px, 30% white)."

motion:
  style: "Slow product-turntable rotation; light sweeps across chrome on scroll. Reflections respond subtly to pointer."
  duration: slow
  forbid: [bounce, paper-texture, warm-glow]

imagery:
  treatment: "3D chrome objects, liquid metal blobs, polished product renders on black."
  signature_prompt: "liquid chrome 3d render, mirror-polished metallic surface with reflections, y2k aesthetic, silver liquid metal blob floating on black background, specular highlights, brushed metal texture, premium industrial design photography, dramatic studio lighting"

components:
  buttons: "Dark glass-metal with chrome edge highlight; hover = light sweep across."
  cards: "Gunmetal panels, hairline silver border, soft reflection at top edge."
  type_hero: "Chrome gradient text on black — one line maximum."

dos:
  - "Make chrome EARN reflections: always imply an environment (stripes, horizon)"
  - "Reserve chrome for hero moments; UI stays matte dark"
  - "Keep everything else monochrome so metal can shine"
donts:
  - "No chrome body text (unreadable + fails contrast law)"
  - "No warm colors except in reflections"
  - "No matte flat gray pretending to be metal"
pairs_with: [vaporwave, art-deco]
