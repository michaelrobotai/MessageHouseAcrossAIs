# AI Message House

A Message House template built for AI. One Markdown file gives Claude, ChatGPT, Perplexity, Gemini, and
Copilot the same approved branding, messages, proof points, and boilerplates, so the drafts they write
for marketing, sales, and PR stay on-message.

Created by [Michael Williams](https://www.revgrow.pro) of Revgrow.pro.

## Why not a Word document?
A classic Message House is a Word file with a hyperlinked table of contents. That works for people, who
navigate. AI tools retrieve: they split a file into chunks and pull back the pieces that look relevant.
Hyperlinks mean nothing to them, and a blurb separated from its heading loses its meaning and rules.

This template fixes that:

| Problem in Word | Fix in this template |
| --- | --- |
| TOC links are invisible to AI | Stable section IDs (`PL-01`, `PP-07`, `BP-50`) anyone can cite |
| Chunks lose their context | Every block carries its own ID, usage rule, channels, and audience |
| Rules live in people's heads | Section 0 tells the AI exactly how to use the file |
| Models trim or "improve" approved copy | Pre-approved length variants: 10, 25, 50, 100 words |
| Models invent or round stats | A proof point table with sources and an Approved / Do-not-use status |
| .docx parsing varies by tool | Plain Markdown, read cleanly by every major model |

## What's inside
```
template/
  message-house.md     Blank template with placeholders
  ai-instructions.md   Text to paste into each AI workspace's instructions field
examples/
  revgrow/message-house.md   A complete, real example (Revgrow.pro)
docs/
  distribution.md      How to load it into Claude, ChatGPT, Perplexity, Gemini, Copilot
  testing.md           Cross-model test prompts and a scoring checklist
```

## Quick start
1. Click **Use this template** (or fork) to create your own copy.
2. Fill in `template/message-house.md`. Use `examples/revgrow/message-house.md` as a guide.
3. Paste `template/ai-instructions.md` into your AI workspace and attach your `message-house.md`
   ([details](docs/distribution.md)).
4. Run the [test prompts](docs/testing.md) in each tool and tighten the file wherever a model improvises.
5. When messaging changes, update the file, bump `version` and `last_approved`, and re-upload.

## The structure
| Section | ID | Purpose |
| --- | --- | --- |
| Instructions for AI | AI-00 | Rules the model follows on every request |
| Brand essentials | BR-01 | Name, tagline, category, contact |
| Visual identity | BR-02 | Colors, fonts, approved logo URLs |
| Roof | RF-01 | The umbrella message |
| Pillars | PL-01… | 3–4 key messages, each linked to proof |
| Differentiator | DF-01 | What only you can claim |
| Proof points | PP-01… | Sourced facts with approval status |
| Copy blocks | BP-, EP-, BIO-, CTA- | Boilerplates, pitch, bios, calls to action |
| Vocabulary | VC-01 | Say / don't-say rules |
| Tone | TN-01 | Voice rules with good and bad examples |
| Audience matrix | AU-01 | Which pillar and copy to use for whom |
| Open questions | OQ-01 | Unresolved items the AI must not answer itself |

## License
MIT. Use it, adapt it, share it.
