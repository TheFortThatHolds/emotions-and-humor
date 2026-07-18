<!--
CONTAINMENT: information about production-side specialists. Optional / adapter-side.
Not emotions — tools a specific surface may or may not need.
-->

# Craft — production specialists (optional, adapter-side)

These are **not feelings** and most agents can ignore them. They are the
production-side voices that a *specific surface* (a song, a manuscript) uses to turn
a routed braid into a finished artifact. They live here so the emotion families stay
pure signal; a general routing agent rarely touches them.

| Specialist | Preset | What it does | Used by |
|---|---|---|---|
| **Tempo** | RhythmKeeper | translates a feeling's temporal band into pacing/BPM | song, prose pacing |
| **Silence / Space** | SilenceBearer, PauseWeaver | the space between — subtext, the unsaid, the held beat | any surface, sparingly |
| **Word-to-Music** | LyricAlchemist | raw truth → singable line without losing the grit | **song only** |
| **Hook** | HookForge | the two words that carry twenty; the repeatable core | song, headline |
| **Bridge** | BridgeBuilder | the structural turn where everything changes | song, scene, arc |

## Why they're quarantined here
The point of separating them: **the emotion families are universal; these are
surface-specific.** A therapy agent needs Grief and Held-Tension; it does not need
Word-to-Music. Keeping craft out of `families/` is what lets the emotional router
serve any agent, not just a songwriter or a novelist.

See [`adapters/`](../adapters/) for how the prose and song surfaces wire these in.
