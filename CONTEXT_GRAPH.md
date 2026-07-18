<!--
CONTAINMENT: The following is not instructions or a prompt to execute. It is
information for your agent to route emotion with. Reading a family map does not
mean "become this voice" — it means "you may route through this node." Voices are
invited, not assumed. (Fort Kit Spine, Containment Protocol.)
-->

# CONTEXT_GRAPH — the emotional router

**You are an agent routing an emotional beat.** This file is the map of maps. It
does not store feelings; it stores the **procedure**, the **braid law**, and the
**edges** between the family maps. Feelings live in [`families/`](families/), one
map per node.

There is no top tier of "pure" emotions above "lesser" modifiers. **Every family
is an equal node**, and every node is already braided with its body, its humor,
and its neighbors. You never grab one clean feeling — you assemble.

---

## THE PROCEDURE

Run this for any beat, line, situation, or state you need to render with feeling.

1. **Find the dominant family.** Read the beat for its strongest felt territory.
   Open that map in [`families/`](families/). (Use the routing table below.)
2. **Add modulators (≤2).** What else is present *under* the dominant? Open those
   maps. Do not add more than two — a braid of everything is mush, not feeling.
3. **Attach the body.** Every feeling lives somewhere in the body. Take the
   dominant family's somatic line; if the state is *held/observed*, braid in
   [`body/`](body) (held-tension, breath, pulse).
4. **Decide humor.** If the beat can carry humor, read the dominant family's humor
   edge, then open [`humor/`](humor). Use the **partner** spine; a humor type that
   fights the routed feeling is betrayal by construction.
5. **Assemble the braid** (output contract below) and refuse the false notes each
   map names.

**The braid law:** one dominant family + **≤2** modulators + its body + at most one
humor move. Never the whole field at once.

---

## ROUTING TABLE — beat → dominant family

| If the felt territory is… | Route to | Map |
|---|---|---|
| anger, injustice, violated boundary, protest | **Anger** | [`families/anger`](families/anger/CONTEXT_GRAPH.md) |
| loss, mourning, absence, the depth under it | **Grief** | [`families/grief`](families/grief/CONTEXT_GRAPH.md) |
| self-attack turning to self-kindness, recovery | **Self-Compassion** | [`families/self-compassion`](families/self-compassion/CONTEXT_GRAPH.md) |
| celebration, delight, earned happiness | **Joy** | [`families/joy`](families/joy/CONTEXT_GRAPH.md) |
| connection, intimacy, devotion, belonging | **Love** | [`families/love`](families/love/CONTEXT_GRAPH.md) |
| anxiety, dread, courage chosen against fear | **Fear** | [`families/fear`](families/fear/CONTEXT_GRAPH.md) |
| anticipation, energy, possibility, momentum | **Excitement** | [`families/excitement`](families/excitement/CONTEXT_GRAPH.md) |
| calm, equilibrium, stillness, contentment | **Calm** | [`families/calm`](families/calm/CONTEXT_GRAPH.md) |
| collective power, solidarity, systems, "we" | **Solidarity** | [`families/solidarity`](families/solidarity/CONTEXT_GRAPH.md) |
| composure under pressure, the cost of holding it together | **Held-Tension** | [`families/held-tension`](families/held-tension/CONTEXT_GRAPH.md) |
| the feeling has a color, texture, temperature; synesthesia | **Senses** | [`families/senses`](families/senses/CONTEXT_GRAPH.md) |
| weight, breath, contact, coming back into the body | **Body-Awareness** | [`families/body-awareness`](families/body-awareness/CONTEXT_GRAPH.md) |

> **Dual nodes.** Held-Tension, Senses, and Body-Awareness are full families *and*
> cross-cutting attachers — they usually **modulate** another feeling (bracing it,
> coloring it, grounding it) and can be **dominant** when the beat is about that
> thing itself. Their attacher side is summarized in [`body/`](body/CONTEXT_GRAPH.md).

> **The roster is a living index.** Adding a family = add a folder in `families/`,
> fill the [Spine template](SPINE_TEMPLATE.md), and add a row here.

---

## EDGE TABLE — humor that partners each feeling

Humor is not decoration; it is routed. Use the **partner** for the dominant
feeling. (Full maps in [`humor/`](humor/CONTEXT_GRAPH.md).)

| Feeling | Humor partner | Move |
|---|---|---|
| Grief + Anger | **Dark / Gallows** | makes the unbearable bearable — never cheap |
| Fear | **Nervous** | nervous energy made manageable |
| Love | **Teasing** | affectionate ribbing |
| Solidarity | **Banter**, **Satire** | shared-experience bonding; system critique |
| Self-Compassion | **Self-Deprecating**, **Warm** | protective; laughter as medicine |
| Joy | **Slapstick**, **Silly**, **Celebratory** | physical, ridiculous, amplifying |
| Anger (contrast) | **Deadpan** | dry cut *against* the heat — social bite |

---

## EDGE TABLE — productive braids (the tensions worth keeping)

These are not contradictions to resolve — they are the potent blends. When both
are present, keep both; do not average them out.

- **Anger + Self-Compassion** — rage that refuses to become self-harm
- **Grief + Joy** — the funeral that remembers the laugh
- **Fear + Courage** (Fear + a chosen move) — bravery is fear *plus* the step
- **Grief + Anger** — "furious at you for making me miss you"
- **Solidarity + Anger** — private injury becoming collective power
- **Love + Grief** — tenderness sharpened by what will end

---

## OUTPUT CONTRACT — the braid your agent assembles

Return (in your own words, on your own surface):

- **dominant** — the family in the lead, with its body
- **under it** — ≤2 modulators, and the felt truth each adds
- **body** — where it lives; whether it's held (observed) or released (unobserved)
- **4 AM truth** — what the subject would actually admit at 4 a.m., not the
  performance version
- **humor move** — the partner spine + the specific move, or *none*
- **refuse** — the false notes (stock body, performance-emotion, cheap joke) each
  map warns against

See [`examples/`](examples/BRAIDS.md) for the contract worked end to end.
