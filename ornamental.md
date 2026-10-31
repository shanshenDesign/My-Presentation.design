id: ornamental
name: Ornamental / Classical
essence: "The art of the frame. Filigree, cartouches, engraved flourishes — ceremony and heritage in every corner."
mood: [ceremonial, prestigious, heritage, meticulous]

palette:
  bg: "#F8F4E9"            # parchment
  bg_alt: "#17130E"        # for dark certificates
  ink: "#2B2118"
  primary: "#9A7B2D"       # antique gold
  accent: "#6B1F2A"        # oxblood
  note: "Parchment + ink + gold + one deep ceremonial color. Everything aged, nothing neon."

typography:
  display: ["Cinzel Decorative", "Playfair Display SC", "Cormorant SC"]
  body: ["EB Garamond", "Cormorant Garamond"]
  flourish_fonts: ["Great Vibes"]  # ≤3 words per artifact
  rules: "Small caps everywhere. Drop caps for opening paragraphs. Centered composition for headings."

texture_technique:
  - "Corner filigree ornaments on every major panel"
  - "Engraved cartouches around titles and seals"
  - "Fine guilloché / lathe patterns as security-print style backgrounds (very subtle)"
  - "Letterpress deboss effect: 1px highlight below, 1px shadow above"

layout:
  grid: "Perfectly centered, symmetric, certificate logic. The frame is the layout."
  spacing: "Formal and measured; generous padding inside borders."
  frames: "Double frames: outer thin + inner thick, ornamental corners joining them."

motion:
  style: "Almost none. A seal may stamp once (scale 1.2→1, 300ms). Ornaments may draw on very slowly."
  duration: slow
  forbid: [slides, bounces, parallax]

imagery:
  treatment: "Engraved portraits, crests, wax seals, laurel wreaths."
  signature_prompt: "ornate victorian ornamental design, intricate filigree corner flourishes, engraved cartouche frame, antique gold on parchment, guilloche pattern, classical certificate style, letterpress texture, symmetrical heraldic composition"

components:
  buttons: "Framed rectangles with corner ornaments, small-caps label; hover = gold brightens."
  cards: "Certificate panels: double border + corner flourishes."
  dividers: "Ornamental fleurons (❦-style) between sections."

dos:
  - "Invest all detail budget in frames and corners"
  - "Keep interiors calm so ornament can breathe"
  - "Use one engraved seal/crest as the signature"
donts:
  - "No sans-serif anywhere visible"
  - "No flat modern icons — use engraved-style glyphs"
  - "No asymmetric layouts"
pairs_with: [vintage-engraving, art-deco]
