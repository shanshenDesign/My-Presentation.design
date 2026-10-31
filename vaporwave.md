id: vaporwave
name: Vaporwave
essence: "A dream of a 1990s that never existed. Neon grids, marble busts, palm trees and infinite sunsets. Irony + beauty."
mood: [nostalgic, surreal, nocturnal, euphoric-melancholy]

palette:
  bg: "#1A0B2E"            # deep night purple
  surface: "#241040"
  primary: "#FF71CE"       # hot pink
  secondary: "#01CDFE"     # cyan
  accent: "#FFFB96"        # pale sun yellow
  extras: ["#B967FF", "#05FFA1"]
  note: "Pink + cyan duet over deep purple. Sunsets are gradients — everything else flat or chrome."

typography:
  display: ["VCR OSD Mono aesthetic", "Space Mono", "Major Mono Display"]
  latin_display_alt: ["Michroma", "Orbitron"]
  body: ["Space Grotesk", "Inter"]
  rules: "Full-width spacing vibes (V A P O R). Japanese text fragments as decoration (use real, correct Japanese or none). Mono fonts for UI chrome."

texture_technique:
  - "Perspective grid floors vanishing to a neon horizon"
  - "Gradient sun with horizontal scanline cuts"
  - "Chrome/greek-bust/palm silhouettes"
  - "VHS artifacts: scanlines, chromatic aberration (1–2px RGB split), tracking glitches"

layout:
  grid: "Centered 'album cover' compositions; hero is a framed scene like a cassette insert."
  spacing: "Atmospheric depth over density."
  frames: "Neon keylines (1px glow ≤8px blur). Windows-95 chrome frames for panels, used ironically but neatly."

motion:
  style: "Endless loop: sun drifts, grid scrolls toward viewer, slow chromatic pulse. Everything loops seamlessly."
  duration: hero
  forbid: [sudden-cuts, realistic-physics]

imagery:
  treatment: "Surreal retro-futurist collage: marble statues, dolphins, 80s tech, palm trees under a grid sky."
  signature_prompt: "vaporwave aesthetic artwork, neon pink and cyan on deep purple, perspective grid floor to horizon, gradient sunset with scanlines, greek marble bust, palm tree silhouettes, VHS glitch artifacts, 80s retro-futurism, dreamy nostalgic"

components:
  buttons: "Neon-outlined, glow on hover; label in mono caps."
  cards: "Dark purple panels, 1px neon border, subtle scanline overlay."
  windows: "Retro OS title-bar panels allowed for features/sections."

dos:
  - "Commit to the fantasy — full atmosphere, not a purple theme"
  - "Loop one ambient animation in the hero"
  - "Keep body text high-contrast despite the neon (accessibility law still applies)"
donts:
  - "No pastel corporate 'purple SaaS' look — vaporwave is night + neon"
  - "No realistic photography without treatment"
  - "No more than 2 glow colors per element"
pairs_with: [metallic-chrome, holographic]
