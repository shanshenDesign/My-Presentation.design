id: photorealistic-collage
name: Photorealistic Collage
essence: "Impossible worlds, believably rendered. Torn edges of different epochs meeting in one frame. Surreal editorial power."
mood: [maximal, surreal, editorial, culturally-electric]

palette:
  strategy: "No fixed palette — the imagery leads. UI palette is EXTRACTED from the hero collage: pick its 2 dominant + 1 accent."
  ui_base: "#F5F2EC"        # gallery off-white lets collages dominate
  ink: "#191919"
  note: "UI stays neutral and quiet. All chromatic energy lives inside the collage artwork."

typography:
  display: ["Editorial serif: Canela-style → Fraunces", "Playfair Display"]
  body: ["Inter", "Source Sans 3"]
  rules: "Magazine typography: huge display serif, drop caps allowed, captions in small italic. Type may weave BETWEEN collage layers."

texture_technique:
  - "Torn-paper and rough-cut edges on collaged photos (realistic paper fiber)"
  - "Mixed epochs in one frame: classical sculpture + botanical + modern object"
  - "Layered depth: some elements cast soft realistic shadows on others"
  - "Tape, pins, or staple marks as authentic fastening details"

layout:
  grid: "Editorial spread logic: asymmetric, overlapping, but with an invisible strong axis holding it together."
  spacing: "Dense art zone + clean text zone. Never collage behind body text."
  frames: "Torn edges are the frame. No rectangular borders on collage pieces."

motion:
  style: "Gallery subtlety: layers parallax gently (max 8px offset), pieces settle into place on load (staggered, 400ms)."
  duration: slow
  forbid: [spin, bounce, fast-slides]

imagery:
  treatment: "High-quality photorealistic cutouts: statues, hands, flowers, architecture, celestial bodies — combined impossibly but lit consistently."
  signature_prompt: "surreal photorealistic collage art, torn paper edges, classical greek statue mixed with botanical flowers and vintage architecture, moon and ocean fragments, layered mixed-media composition, consistent cinematic lighting, editorial magazine cover style, renaissance meets contemporary"

components:
  buttons: "Quiet and editorial: underlined text links, or hairline buttons. The art is loud; the UI whispers."
  cards: "Clean gallery-white panels; collage piece bleeds out of the card edge."
  captions: "Gallery-caption style: small, italic, numbered (fig. 01)."

dos:
  - "Unify the collage with ONE light direction and consistent shadow logic"
  - "Mix at least 3 different epochs/categories per hero collage"
  - "Let one collage element break the frame boundary"
donts:
  - "No collage behind text — carve a clean reading zone"
  - "No more than 7 distinct elements or it turns to noise"
  - "No flat vector shapes mixed into the photorealism"
pairs_with: [oil-painting, botanical]
