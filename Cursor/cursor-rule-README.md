# Cursor Rules — Sentient Triangle

Two rules for Cursor, both agent-requested (they load automatically when relevant, not on every prompt) rather than always-on.

## Files

- **`sentient-triangle-ideation.mdc`** — loads when scoping a new AI-enabled feature or exploring how something could behave. Walks through 3-5 deliberately divergent postures, writes a short provocation for each, then converges the strongest into prototype briefs.
- **`sentient-triangle-posture.mdc`** — loads when scaffolding or reviewing a prototype that's been assigned a named posture (e.g. "build this as a Steward"). Keeps the interaction logic — who has initiative, whether a persistent UI exists, how failure is handled — faithful to that posture instead of drifting back to a generic chat pattern. Includes a check at the end to flag if two posture-builds ended up behaviorally identical under different skins.
- **`docs/sentient-triangle-postures.md`** — the shared posture taxonomy and provocation questions both rules read from.
- **`docs/triangle-diagram.png`** — visual reference for the triangle and where postures/patterns sit on it.

## Setup

1. Copy the `.cursor/rules/` files into your project's `.cursor/rules/` directory, and `docs/` into your project root (or wherever your docs live — just update the path references in the rules if you move it).
2. Commit and push. Rules apply to anyone with the repo open in Cursor.
3. The build-fidelity rule is scoped by default to a `prototypes/` folder. If your repo structure differs, edit the scoping note at the top of `sentient-triangle-posture.mdc`.

## Using it

**Ideation:** describe your feature/problem naturally, or mention "posture," "sentient triangle," or "how should this behave" — the rule loads on its own.

**Building:** name the posture explicitly when asking Cursor to scaffold something — e.g. "prototype the Sculptor version of this." Naming it is what triggers the fidelity rule; Cursor won't guess which posture you mean.
