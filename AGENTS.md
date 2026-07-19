# AGENTS.md — Codex/OpenAI compatibility

These instructions apply to the entire repository.

## Canonical instruction source

This repository's canonical agent instructions live in `CLAUDE.md` when that file is present in the checkout.

Before doing any work:

1. Read `CLAUDE.md` in full.
2. Treat every instruction addressed to **Claude** as addressed to the current Codex/OpenAI agent.
3. Follow its file-walking order, routing discipline, refusal rules, verification steps, and output contract exactly.
4. Do not replace it with a summary from memory.

`AGENTS.md` is the Codex entry point; `CLAUDE.md` remains the shared behavioral source of truth. When both exist, use this file for Codex mechanics and `CLAUDE.md` for repository behavior.

## Canonical fallback when `CLAUDE.md` is unavailable

Do not improvise a generic emotion answer. Walk the repository itself:

1. Read `CONTEXT_GRAPH.md` first.
2. Read `THE_FIELD.md` in full. It is required, not optional background.
3. When the beat names color, texture, temperature, body location, numbness, or shutdown, read `COLOR_SPINE.md`.
4. Open the dominant family's `families/<family>/CONTEXT_GRAPH.md`.
5. Open no more than two supporting family maps.
6. Read `body/CONTEXT_GRAPH.md` and the relevant body map when the state is held, observed, braced, released, or somatically specific.
7. Read `humor/CONTEXT_GRAPH.md` and the routed humor partner only when humor survives the `B(f)` check.
8. Use `examples/BRAIDS.md` for calibration when needed.

## Routing law

Route the whole field, never one clean label.

- Choose one dominant family.
- Add at most two modulators.
- Trace the causal stack all the way beneath the surface before rendering the top.
- Keep opposing high-weight feelings in superposition; do not average or resolve them.
- Treat controlled surfaces—cold or bright—as dense states carrying weight, not as empty, flat, fine, or merely happy.
- Do not mistake numbness or dorsal shutdown for Calm.
- Attach the body.
- Use at most one humor move, and use silence when the container cannot bear the wound.
- Refuse stock body language, performance-emotion, decorative color, cheap jokes, and any line that merely announces that several feelings are present.
- Render the field so the reader feels the braid without being told that it is mixed.

When a routing trace is requested, include the full contract from `CONTEXT_GRAPH.md`: dominant, under it, stack, superposition, sharpness read, body, 4 AM truth, humor move, and refused notes. When only the answer is requested, render the result without dumping the trace.

## Repository changes

The Markdown maps are the source of truth. `graph.json` and `viz/index.html` are generated projections.

After changing family maps, routing edges, colors, emojis, or graph-bearing metadata, run:

```bash
python3 tools/build_graph.py
```

The build must complete successfully. Do not hand-edit generated projections to conceal drift. Keep braid edges symmetric and keep the router, family maps, machine projection, and visualization in agreement.

Before finishing a code or content change, inspect the diff and report what changed and what verification ran.

## Tool and agent boundary

Tool receipts, async-agent metadata, internal IDs, temporary paths, continuation instructions, and orchestration payloads are never user-facing output. A launch receipt is not a completed result. Wait for the actual completion event, then render only the finished work. If completion is still pending, say only that the work is still running.
