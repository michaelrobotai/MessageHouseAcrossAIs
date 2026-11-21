# Loading the Message House into AI tools

Keep **one** master `message-house.md` in this repo. Every AI workspace gets a copy of that file plus the
instructions block from `template/ai-instructions.md`. When the master changes, bump `version` and
`last_approved`, then re-upload everywhere. Anyone can spot a stale copy by its date.

| Tool | Where it goes | Instructions | Knowledge file |
| --- | --- | --- | --- |
| Claude | A Project | Project instructions | Add `message-house.md` to project knowledge |
| Claude (automatic) | A Skill | Skill description: "Use when drafting any <Company> marketing, sales, or PR copy" | Bundle `message-house.md` inside the skill |
| ChatGPT | A Custom GPT or a Project | GPT/Project instructions | Upload under Knowledge / project files |
| Perplexity | A Space | Space instructions | Upload to the Space's files |
| Gemini | A Gem | Gem instructions | Attach as a knowledge file |
| Microsoft Copilot | An agent | Agent instructions | Add as a knowledge source (or point to the file in SharePoint) |
| Any tool with web or Drive access | — | — | Point it at the raw file URL in this repo or a shared Drive/Notion copy |

Product menus change often. If a label above doesn't match what you see, look for "instructions" and
"knowledge" or "files" in the workspace settings.

## Tip: link the raw file
GitHub serves the plain text at
`https://raw.githubusercontent.com/<your-github-username>/ai-message-house/main/examples/revgrow/message-house.md`.
Tools that can browse can read the current version from that URL. That's useful for one-off chats
outside a configured workspace.

## Keep humans in the loop
Markdown converts back to a formatted Word or PDF file (for example with Pandoc:
`pandoc message-house.md -o message-house.docx`) for anyone who prefers the classic document.
