id: japanese-ink
name: Japanese Ink (Sumi-e)
essence: "The beauty of what is left out. One brush, black ink, and ma (間) — purposeful emptiness."
mood: [meditative, refined, poetic, disciplined]

palette:
  bg: "#F5F2EA"            # washi paper
  ink: "#1C1B18"
  grays: ["#4A4843", "#8A867C", "#C9C4B4"]  # ink dilutions
  accent: "#A63D2F"        # vermillion — ONLY for the hanko seal moment, 1 per view
  note: "Ink density creates the entire value scale. Vermillion is sacred: one seal, that's all."

typography:
  display: ["Shippori Mincho", "Noto Serif JP", "Cormorant"]
  body: ["Shippori Mincho", "Source Serif 4"]
  rules: "Vertical text (writing-mode: vertical-rl) allowed for hero accents. Extreme restraint in sizes — often just two."

texture_technique:
  - "Expressive brushstrokes: dry-brush (kasure) edges, wet bleeds"
  - "Enso circles, bamboo, mountain silhouettes at 10–30% ink density"
  - "Washi paper grain overlay 4%"
  - "One red hanko-style seal stamp as signature element"

layout:
  grid: "Radical asymmetry with vast emptiness (ma). Content occupies ≤40% of the view."
  spacing: "Enormous margins; sections separated by emptiness, not lines."
  frames: "None. Occasionally a single 1px sumi line."

motion:
  style: "Ink flows: brushstrokes paint themselves in real-time (stroke draw, 1.2s). Then stillness."
  duration: slow
  forbid: [constant-motion, parallax, bounce]

imagery:
  treatment: "Sumi-e painting only. No photography unless reduced to near-ink monochrome."
  signature_prompt: "minimalist japanese sumi-e ink wash painting, expressive black brushstrokes on washi paper, vast negative space, dry brush texture, single vermillion seal stamp, zen aesthetic, mountains or bamboo subject"

components:
  buttons: "Ink-underlined text, or a single brushstroke rectangle outline. Hover: ink deepens."
  cards: "Borderless; separated by space. A faint 8% ink wash may ground them."
  seal: "Square vermillion stamp with initials/mark — the brand signature, used once."

dos:
  - "Cut content until it hurts, then cut once more"
  - "Let a single brushstroke carry an entire section"
  - "Use ink dilution (grays) instead of borders and boxes"
donts:
  - "No fills of solid color, no gradients, no shadows"
  - "No more than one accent seal per view"
  - "No clutter — every element must earn its existence"
pairs_with: [minimal-line-art, watercolor]
