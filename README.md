# Sentient Triangle Posture Explorer

A Claude skill for breaking AI feature ideation out of the chatbot default.

Built on Josh Clark & Veronika Kindred's *Sentient Design* framework (Rosenfeld Media), which maps AI-mediated experiences across three attributes — **grounded**, **interoperable**, and **radically adaptive** — into four archetypes (Tools, Chat, Agents, Copilots) and 18 named postures within them (Sculptor, Steward, Bespoke UI, Conductor, and so on).

**What it does:** given a problem or user need, the skill selects a handful of genuinely divergent postures, generates short provocations exploring how each one would frame and handle the problem (not just different tone — different control, initiative, and interface shape), then converges the strongest ones into prototype briefs concrete enough to hand to a builder.

**Why:** most AI feature scoping defaults to "make it a chatbot" without examining the alternatives. This skill forces genuine divergence early — useful for design sprint ideation, HMW exploration, or any point where a team needs 2-4 real, testable prototype directions instead of one interaction pattern with different copy.

**Design choice:** the reference material includes real provocation questions per posture, but the skill is explicitly instructed to treat them as sparks rather than a script — pull what's relevant, skip the rest, avoid reciting the same real-world examples session after session. It's meant to stay probabilistic, not become a fill-in-the-blank template.

**Use it when:** scoping a new AI-enabled feature, prepping design sprint materials, or asking "what would this look like as an agent vs. a copilot vs. a tool."

Source framework: [*Sentient Design*](https://rosenfeldmedia.com/books/sentient-design/) by Josh Clark & Veronika Kindred.