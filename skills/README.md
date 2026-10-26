# Lean Advisor — AI skills

The Lean Advisor is the operational AI companion of the Digital Lean Framework. It guides a practitioner through five modes, one step at a time, always against the framework text:

1. **DLI Assessment**: Step 0 (A–E) → Step 6, including the Efficiency Matrix, internal chain and digital Jidoka
2. **Muda scan**: the 9 digital muda with evidence-based scoring
3. **Sprint Kaizen**: two-week cycles with the Lean Test
4. **Law Zero**: decision workflow before any project or technology (paths A/B/C)
5. **DLI Calculator**: composite score plus matrix, Jidoka and source-of-inefficiency layers

| Package | Language | Folder |
|---|---|---|
| Claude skill | English | [`claude/lean-advisor-en/`](claude/lean-advisor-en) |
| Claude skill | Italian | [`claude/lean-advisor/`](claude/lean-advisor) |
| Gemini Gem | English | [`gemini/lean-advisor-gem-en/`](gemini/lean-advisor-gem-en) |
| Gemini Gem | Italian | [`gemini/lean-advisor-gem/`](gemini/lean-advisor-gem) |

The English packages answer in English and read the canonical Italian texts through `terminology-en.md`. Install one language per workspace: the two Claude skills share most trigger words.

## Claude

Zip the skill folder (or download the matching zip from the latest release) and upload it as a custom skill in Claude (see Anthropic's documentation on Skills). Then start with: "Lean Advisor, I want to assess my incident management process".

## Gemini

Follow `GEM_SETUP_GUIDE.md` in the Gem folder. Do not use Gemini's "re-write instructions" feature: it degrades fidelity to the framework.

## Versioning

All packages are snapshots of DLF v2.4. The files in `references/` and `knowledge/` are copies of the canonical texts in [`framework/it/`](../framework/it); when the framework changes, the packages are regenerated.

Licensed CC BY-NC-ND 4.0: you may use the skills as distributed; modified or rebranded versions may not be redistributed.
