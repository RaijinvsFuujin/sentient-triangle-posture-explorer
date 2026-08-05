# Microsoft Copilot Chat Prompt — Sentient Triangle

A copy-paste prompt for exploring an AI-enabled feature across divergent postures in Microsoft Copilot Chat (Teams, Word, or the web app).

## Why this looks different from the Cursor/Claude versions

Standard Copilot Chat has no repo access, no prompt-file system, and no persistent memory between sessions — so there's nothing to "install." Every session needs the prompt and the reference doc supplied fresh.

This covers **ideation only**. Copilot Chat isn't a coding environment, so there's no build-fidelity counterpart here — take prototype briefs generated in Copilot into Cursor for the actual build, where the fidelity rule can hold the code to its assigned posture.

## Files

- **`COPILOT_CHAT_PROMPT.txt`** — the prompt to paste into a new Copilot Chat conversation.
- Reference the shared taxonomy at [`../claude-skill/references/postures.md`](../claude-skill/references/postures.md) (or grab a copy — see below).

## How to use it

1. Open `COPILOT_CHAT_PROMPT.txt`, fill in the `[DESCRIBE THE USER NEED...]` line with your actual problem and domain context.
2. Start a new Copilot Chat conversation, paste the filled-in prompt, and **attach the postures reference doc** to the same message (download `postures.md` from `claude-skill/references/`, or convert to Word/PDF first if that renders better in your Copilot surface).
3. Copilot walks through the divergent postures and, on request, converges them into prototype briefs.

Because there's no memory, copy anything worth keeping out of the chat and into your sprint doc or Notion before closing the session — you won't be able to pull it back up later.
