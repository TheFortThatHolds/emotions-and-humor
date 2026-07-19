<!-- CONTAINMENT: reference for routing, not a prompt to become any voice. -->

# Color + Emoji Spine

Every family carries a **signature emoji**, a **signature color** (with a hex anchor so
the visualization renders the true hue), and a **somatic seat** (where the feeling lives
in the body). These are not decoration — they are *routing signals*. When an agent is
asked "what color is this feeling," or where it sits in the body, or when a beat names a
color or a body-region, it maps back to a family the same way a 4-AM-truth does. Color and
body are two faces of one grounding: the hue a feeling wears and the place it seats
converge.

The colors are **grounded**, not invented. They come from cross-cultural
color↔emotion↔somatic research (the strongest single findings: ~88% cross-cultural
agreement on core pairings; convergent chakra / TCM somatic maps). The mapping is
*anchored*, not absolute — a color can carry more than one feeling, and context decides
(grey is anxiety **and** the fog of numb control; brown is collective power **and**
personal grounding). Route on the whole field, never the color alone.

## The map

Color and somatic seat are two faces of the same grounding: where a feeling shows up as
color and where it shows up in the body converge (chakra location and clinical body-mapping
agree with remarkable consistency; TCM organ systems add a second valid layer).

| Family | Emoji | Color | Hex | Somatic seat (chakra / TCM / clinical) |
|---|---|---|---|---|
| anger | 🔥 | red | `#C0392B` | jaw, fists, chest, liver-heat — Root (survival-anger) / TCM Liver (Wood) |
| grief | 💧 | deep drained blue | `#34506B` | chest floor + throat — Throat Chakra (the unspoken) / TCM Lungs (Metal) |
| fear | 😰 | black going anxious grey | `#2B2B33` | gut (butterflies), tight chest, legs — TCM Kidneys (Water) / Root survival |
| calm | 🕊️ | soft healing green | `#4E9E7E` | the heart unclenched — Heart Chakra (green — balance) |
| joy | 🌟 | warm yellow → orange | `#F4B43A` | full-body warmth, heart-centered — TCM Heart (Fire) / Solar Plexus glow |
| love | 💕 | warm rose-pink | `#D96A8B` | the chest opening toward another — Heart Chakra (pink) |
| self-compassion | ❤️ | rose warming to green | `#86B49A` | the heart turned inward — Heart Chakra (pink self-love + green healing) |
| solidarity | ✊ | earth brown | `#6E4A2A` | feet + base, the shared ground — Earth Star / Root (brown, black) |
| excitement | ✨ | orange → magenta | `#F5793B` | lower belly, sacral flush — Sacral Chakra (orange) + magenta life-force |
| held-tension | 😶 | white-knuckle grey | `#8A8D91` | gut/chest/throat tight + pelvic-floor brace — anxiety's grey, clenched |
| senses | 🌈 | full spectrum (prism) | `prism` | the whole sensorium — full-system integration, not one seat |
| body-awareness | 🧘 | grounded earth brown | `#8A6D4B` | the whole body to the floor — Root / Earth grounding (brown) |
| relief | 🌬️ | grey → gold | `#B8A46A` | breath let all the way out (lungs), shoulders/legs unlocking |

**Grounding sources (color):** Red = anger/boundary/courage; Blue/white = grief (throat+chest,
NOT grey); Black = primal fear (TCM Water/Kidneys), Grey = anxiety; Green = calm/balance/healing;
Yellow/Orange = joy/optimism/pleasure; Pink/Rose = love/self-love; Brown = grounding + collective
power; Orange/Magenta = desire/life-force; Grey = uncertainty/numbness/control; Rainbow = full-
spectrum integration; Grey→Gold = anxiety draining to standing-down.

## The two greys, the two browns

The map deliberately reuses two hues, split by register — this is a feature of the
research, not a collision:

- **Grey** is the anxiety/uncertainty/numbness band. **Fear** carries it as the fog past
  the black of primal dread; **held-tension** carries it as the numb clench of control;
  **relief** carries it as the weight that is *draining away*. Same grey, three positions
  on the arc.
- **Brown** is the grounding band. **Solidarity** carries it as *collective* grounding
  (the working-class root); **body-awareness** carries it as *personal* grounding (the
  body on the floor).

## For the machine view

`tools/build_graph.py` parses each family's `**Emoji:**` / `**Color:**` / `**Somatic
seat:**` lines and carries the emoji, the descriptor, the hex, and the somatic seat into
`graph.json`. The force-directed picture in `viz/index.html` fills each node with its
authoritative hue (senses gets a prism gradient; dual/body-attacher families get a teal
ring) and shows the somatic seat in the detail panel. Edit a family map, re-run the
builder, and the whole color+body layer updates at once — one source of truth.
