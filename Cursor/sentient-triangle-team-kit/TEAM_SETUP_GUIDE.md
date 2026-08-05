# Sentient Triangle Toolkit — Team Setup Guide (Cursor + Microsoft Copilot)

Framework: Josh Clark & Veronika Kindred's *Sentient Design*. This kit helps us explore how an AI-enabled feature could behave (ideation) and keeps prototypes true to whichever posture they're built as (build fidelity).

Two tools, two roles:
- **Cursor** does both ideation and build fidelity — it has repo access, so it can hold rules that load automatically.
- **Microsoft Copilot Chat** does ideation only. It doesn't have repo access, memory between sessions, or a prompt-file system for standard users — so it works as a copy-paste prompt plus an attached reference doc, fresh each time.

## One-time setup

1. Unzip `sentient-triangle-team-kit.zip` into the repo root. It adds:
   - `.cursor/rules/` — two Cursor rules (ideation + build fidelity)
   - `docs/sentient-triangle-postures.md` — the shared posture reference
   - `COPILOT_CHAT_PROMPT.txt` — the paste-in prompt for Microsoft Copilot Chat
2. Commit and push the `.cursor/` and `docs/` folders so the team gets them on pull.
3. `COPILOT_CHAT_PROMPT.txt` and `docs/sentient-triangle-postures.md` aren't tied to the repo — save them somewhere the whole team can grab easily too (Teams channel, SharePoint, Notion), since not everyone doing ideation will have the repo open.
4. Build-fidelity rules are scoped to a `prototypes/` folder by default. If your repo structure differs, edit the scoping note at the top of `.cursor/rules/sentient-triangle-posture.mdc`.

## Using it in Cursor

1. Open Cursor's chat/agent in the repo.
2. **Ideation:** describe the problem naturally, or mention "posture," "sentient triangle," or "how should this behave" — the ideation rule loads automatically and walks through 3-5 divergent postures.
3. Review the provocations, pick 2-4 to take further.
4. **Building a prototype:** explicitly name the posture when asking Cursor to scaffold it — e.g. "build this as a Steward" or "prototype the Sculptor version." Naming it triggers the build-fidelity rule, which keeps the interaction logic honest to that posture instead of drifting back to a generic chat pattern.
5. Before calling a prototype done, Cursor should flag if two posture-builds ended up with identical interaction logic under different skins. If it doesn't, ask it to check.

## Using it in Microsoft Copilot Chat (Teams, Word, or the web app)

Copilot Chat has no persistent memory of this framework, so every session needs both pieces attached fresh:

1. Open `COPILOT_CHAT_PROMPT.txt`, fill in the `[DESCRIBE THE USER NEED...]` line with your problem/feature and domain context.
2. Start a new Copilot Chat conversation, paste the filled-in prompt, and **attach `docs/sentient-triangle-postures.md`** (or a Word/PDF copy if that renders better in your Copilot surface) to the same message.
3. Copilot will walk through the divergent postures the same way Cursor does.
4. If you want prototype briefs from the same session, just ask it to converge — step 3 of the prompt covers that, or say "go ahead and give me the prototype briefs now."
5. To take a prototype into build, bring the resulting briefs into Cursor and name the posture explicitly when scaffolding — Copilot Chat itself isn't the tool for code fidelity.

## Ground rules worth stating up front

- Always name the posture explicitly before asking Cursor to build a prototype.
- Treat the provocation questions in `docs/sentient-triangle-postures.md` as sparks, not a checklist — divergent thinking is the point, not answering every question for every posture.
- If prototypes end up looking different but behaving the same, that's a signal to swap a posture, not a signal the tool is broken.
- Since Copilot Chat has no memory, save good sessions (copy the output into the relevant Notion/sprint doc) rather than relying on being able to pull them back up later.
