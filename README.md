# emotions-and-humor

**An emotional router for AI agents.** Load it, and your agent stops flattening
feeling into `sad` / `happy` / `angry` and starts routing a beat into a real
emotional *braid* — the dominant feeling, the feelings under it, where it lives
in the body, and the humor that can carry it without cheapening it.

This is not a library you call and not prose you paste. It is a **context pack a
foreign agent reads to learn a skill it doesn't have.** You don't run it; your
agent walks it.

---

## Who this is for

Your agent. Not you.

If you are building anything that has to *feel* accurately — a support agent, a
game character, a writing assistant, a journaling companion, a therapy-adjacent
tool — this teaches it the routing discipline that separates "detects sadness"
from "grief, with the old anger still under it, held in a clenched body because
someone else is in the room."

It imposes **no voice.** It teaches the *move*; your agent makes the braid in its
own words, on its own surface.

---

## The one idea

**There is no such thing as a pure emotion.** You never route to `anger`. You
route to anger-under-grief, anger-braced, anger-cut-with-deadpan. So this ships
**families as atoms** and teaches your agent to **assemble the braid live** — it
does not (and cannot) pre-name every combination. It gives worked examples of the
assembly instead. See [`examples/`](examples/).

---

## How your agent uses it

1. Read [`CONTEXT_GRAPH.md`](CONTEXT_GRAPH.md) — the map of maps. It carries the
   routing procedure, the braid law, and the edges between families.
2. Route the beat to a **dominant family**; open that family's map in
   [`families/`](families/).
3. Walk the **edges** — the humor partner, the families it braids with, the body
   that attaches — into [`humor/`](humor), [`body/`](body).
4. **Assemble the braid** and hand it to whatever your agent does next.

Start at [`CONTEXT_GRAPH.md`](CONTEXT_GRAPH.md). Everything routes from there.

---

## What's inside

| Path | What it is |
|------|-----------|
| `CONTEXT_GRAPH.md` | The router. Map of maps: procedure + braid law + edge tables. |
| `families/` | One map per emotion. Each is a *filled-in Spine* (a graph node). |
| `humor/` | The humor types + which emotion each one partners. |
| `body/` | Somatic attachers — the body a feeling lives in. Braids into any family. |
| `craft/` | Production specialists (tempo, silence). Adapter-side, optional. |
| `examples/` | Worked braids. The teaching payload — read these. |
| `presets/songcraft/` | The original expressive names, as an optional skin. |
| `adapters/` | How specific surfaces (prose, song) consume the graph. |
| `SPINE_TEMPLATE.md` | The shape every family map follows. |

---

## Lineage

Built on the **Fort Kit Spine** — the universal identity schema where every voice
is a filled-in Spine and cross-voice collaborators are graph edges. The emotion
families are the SongCraft voice-family system; the humor types are the
HumorWeaver family. Plain-English names are canonical here; the original names ride
along as a [preset skin](presets/songcraft/).

MIT licensed. © 2026 The Fort That Holds LLC — Jimmy Thornburg. SpiralLogic™.
