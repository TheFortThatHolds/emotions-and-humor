<!-- CONTAINMENT: reference for routing, not a prompt to become any voice. -->

# Color + Emoji Spine

Every family carries a **signature emoji** and a **signature color** (with a hex anchor
so the visualization renders the true hue). These are not decoration — the color is a
*routing signal*. When an agent is asked "what color is this feeling," or when a beat
names a color, the color maps back to a family the same way a body-signal or a 4-AM-truth
does.

The colors are **grounded**, not invented. They come from cross-cultural
color↔emotion↔somatic research (the strongest single findings: ~88% cross-cultural
agreement on core pairings; convergent chakra / TCM somatic maps). The mapping is
*anchored*, not absolute — a color can carry more than one feeling, and context decides
(grey is anxiety **and** the fog of numb control; brown is collective power **and**
personal grounding). Route on the whole field, never the color alone.

## The map

| Family | Emoji | Color | Hex | Grounding |
|---|---|---|---|---|
| anger | 🔥 | red | `#C0392B` | Red = anger / boundary / courage / heat |
| grief | 💧 | deep drained blue | `#34506B` | Blue/white = grief, seated in throat + chest (NOT grey) |
| fear | 😰 | black going anxious grey | `#2B2B33` | Black = primal fear (TCM Water/Kidneys); Grey = anxiety |
| calm | 🕊️ | soft healing green | `#4E9E7E` | Green = peace / calm / balance / healing |
| joy | 🌟 | warm yellow → orange | `#F4B43A` | Yellow = optimism/confidence; Orange = joy/pleasure |
| love | 💕 | warm rose-pink | `#D96A8B` | Pink/Rose = love / tenderness |
| self-compassion | ❤️ | rose warming to green | `#86B49A` | Pink (self-love) + Green (compassion/healing) |
| solidarity | ✊ | earth brown | `#6E4A2A` | Brown = collective power / community / working-class solidarity |
| excitement | ✨ | orange → magenta | `#F5793B` | Orange = pleasure; Magenta = desire / aliveness / life-force |
| held-tension | 😶 | white-knuckle grey | `#8A8D91` | Grey = uncertainty / numbness / the fog of control |
| senses | 🌈 | full spectrum (prism) | `prism` | Rainbow/Prismatic = full-spectrum integration |
| body-awareness | 🧘 | grounded earth brown | `#8A6D4B` | Brown = grounding / earth (warm/personal register) |
| relief | 🌬️ | grey → gold | `#B8A46A` | Grey (anxiety) draining → Gold (standing down) |

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

`tools/build_graph.py` parses each family's `**Emoji:**` / `**Color:**` line and carries
the emoji, the descriptor, and the hex into `graph.json`. The force-directed picture in
`viz/index.html` fills each node with its authoritative hue (senses gets a prism
gradient; dual/body-attacher families get a teal ring). Edit a family map, re-run the
builder, and the color layer updates everywhere at once — one source of truth.
