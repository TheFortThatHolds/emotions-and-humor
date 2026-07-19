<!-- CONTAINMENT: reference for routing, not a prompt to become any voice. -->

# Color + Emoji Spine

Every family carries a **signature emoji**, a **signature color** (with a hex anchor so
the visualization renders the true hue), a **somatic seat** (where the feeling lives in
the body), and a **nervous-system state** (its polyvagal register). These are not
decoration — they are *routing signals*. When an agent is asked "what color is this
feeling," or where it sits in the body, or when a beat names a color or a body-region, it
maps back to a family the same way a 4-AM-truth does. Color and body are two faces of one
grounding: the hue a feeling wears and the place it seats converge.

**The anchor is SongCraft's own map; the research is support.** The somatic seats and the
nervous-system states come from SongCraft's Emotion-Body Map (the nine emotional families'
somatic signatures — location, sensation, energy, breath, and polyvagal state — plus
SomaticScribe's body-dictionary). The cross-cultural color↔emotion↔somatic **research**
(≈88% agreement on core pairings; chakra / TCM maps) is cited as *corroboration* — it
backs the SongCraft map up, it does not overrule it. The research isn't definitive; it's
support. Every mapping is *anchored*, not absolute — a color or a body-signal can carry
more than one feeling, and context decides (grey is anxiety **and** the fog of numb
control; numbness is dorsal shutdown, **not** ventral calm; brown is collective power
**and** personal grounding). Route on the whole field, never one signal alone.

## The map

Color, somatic seat, and nervous-system state are faces of one grounding: where a feeling
shows up as color, where it seats in the body, and which polyvagal register it runs in all
converge. The **body + NS columns are SongCraft's Emotion-Body Map**; the color hue draws
on the color↔emotion research as support.

| Family | Emoji | Color | Hex | Somatic seat (SongCraft body-map) | Nervous system |
|---|---|---|---|---|---|
| anger | 🔥 | red | `#C0392B` | chest, jaw, fists, shoulders — heat/pressure rising, breath held | sympathetic (fight) |
| grief | 💧 | deep drained blue | `#34506B` | throat + heart/chest, heavy limbs — weight/ache, sighs | dorsal (shutdown of loss) |
| fear | 😰 | black going anxious grey | `#2B2B33` | stomach + chest, restless limbs — flutter/tight, shallow fast breath | sympathetic (flight) |
| calm | 🕊️ | soft healing green | `#4E9E7E` | whole body soft, breath easy — settled | ventral (safe/social) |
| joy | 🌟 | warm yellow → orange | `#F4B43A` | chest open, whole-body lightness — warmth expanding | ventral |
| love | 💕 | warm rose-pink | `#D96A8B` | chest warm, hands reaching, face soft — flowing | ventral |
| self-compassion | ❤️ | rose warming to green | `#86B49A` | chest softening, shoulders dropping, breath deepening — hand on heart | shame easing toward ventral |
| solidarity | ✊ | earth brown | `#6E4A2A` | chest opening (not alone), strength in spine, breath deepening | sympathetic heat → ventral |
| excitement | ✨ | orange → magenta | `#F5793B` | chest + restless limbs, animated — buzzing, alive, forward | sympathetic+ (toward) |
| held-tension | 😶 | white-knuckle grey | `#8A8D91` | shoulders at ears, jaw clenched, belly tight — breath trapped | sympathetic held / freeze |
| senses | 🌈 | full spectrum (prism) | `prism` | the whole sensorium — reads every body-map, owns none | any (reads, doesn't own) |
| body-awareness | 🧘 | grounded earth brown | `#8A6D4B` | whole body to the floor — feet down, breath tracked | ventral grounding |
| relief | 🌬️ | grey → gold | `#B8A46A` | long exhale, shoulders down, legs unlocking — the discharge | sympathetic → ventral |

**Grounding sources (color):** Red = anger/boundary/courage; Blue/white = grief (throat+chest,
NOT grey); Black = primal fear (TCM Water/Kidneys), Grey = anxiety; Green = calm/balance/healing;
Yellow/Orange = joy/optimism/pleasure; Pink/Rose = love/self-love; Brown = grounding + collective
power; Orange/Magenta = desire/life-force; Grey = uncertainty/numbness/control; Rainbow = full-
spectrum integration; Grey→Gold = anxiety draining to standing-down.

## The two greys, the two browns

The map deliberately reuses two hues, split by register — this is a feature of the map,
not a collision:

- **Grey** is the anxiety/uncertainty/numbness band. **Fear** carries it as the fog past
  the black of primal dread; **held-tension** carries it as the numb clench of control;
  **relief** carries it as the weight that is *draining away*. Same grey, three positions
  on the arc.
- **Brown** is the grounding band. **Solidarity** carries it as *collective* grounding
  (the working-class root); **body-awareness** carries it as *personal* grounding (the
  body on the floor).

## The nervous-system layer (why numbness ≠ calm)

SongCraft's map runs a polyvagal register under every family, and it is the sharpest
anti-collapse tool the spine has. **Calm and numbness look alike on the surface and are
opposite in the body:**

- **Ventral** (safe/social) is real settling — calm, joy, love, grounded body-awareness.
  The system is *open*.
- **Sympathetic** (fight/flight) is mobilized — anger, fear, excitement, the held brace
  of held-tension. The system is *charged*.
- **Dorsal** (shutdown) is collapse — the heavy conserving state of grief, and the
  floating numbness of dissociation. The system is *gone*.

So when a beat reads flat, still, "fine," or numb, that is almost never Calm (ventral). It
is **dorsal** — a shutdown *of* grief, fear, or overwhelm — and routes to the dense
feeling underneath, not to peace. (This is the polyvagal form of THE_FIELD Step 0: *look
truly, don't collapse.*) Numbness is a body that has left, not a body at rest.

## For the machine view

`tools/build_graph.py` parses each family's `**Emoji:**` / `**Color:**` / `**Somatic
seat:**` / `**Nervous system:**` lines and carries the emoji, the descriptor, the hex, the
somatic seat, and the polyvagal state into `graph.json`. The force-directed picture in
`viz/index.html` fills each node with its authoritative hue (senses gets a prism gradient;
dual/body-attacher families get a teal ring) and shows the somatic seat and nervous-system
state in the detail panel. Edit a family map, re-run the builder, and the whole
color+body+NS layer updates at once — one source of truth.
