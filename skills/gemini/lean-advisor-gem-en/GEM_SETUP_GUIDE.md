# Setup guide — "Lean Advisor" Gem for Gemini (English)

## Package

```
lean-advisor-gem-en/
├── GEM_INSTRUCTIONS.md     → paste into the Gem "Instructions" field
├── GEM_SETUP_GUIDE.md      → this guide
└── knowledge/              → 8 files to upload as Knowledge (cap: 10)
    ├── lean-advisor-full-instructions.md
    ├── terminology-en.md
    ├── digital-lean-framework.md     (canonical Italian text)
    ├── guida-operativa.md            (canonical Italian text)
    ├── assessment-dli.md             (canonical Italian text)
    ├── muda-checklist.md             (canonical Italian text)
    ├── sprint-kaizen.md              (canonical Italian text)
    └── legge-zero-workflow.md        (canonical Italian text)
```

The Gem answers in English and renders the Italian canonical texts through `terminology-en.md`.

## Steps

1. Go to **gemini.google.com** → **Explore Gems** → **New Gem** (web only).
2. **Name**: `Lean Advisor — DLF v2.4`.
3. **Instructions**: paste the full content of `GEM_INSTRUCTIONS.md`. **Do not use "Use Gemini to re-write instructions"**: it degrades fidelity to the framework.
4. **Knowledge** → **Add files**: upload the 8 files in `knowledge/` (rename to `.txt` if `.md` uploads fail).
5. Leave **Default tool** on "No default tool"; keep knowledge citations on.
6. Run the smoke tests in the preview, then **Save**.

## Smoke tests

| Prompt | Expected behavior |
|---|---|
| "I want to assess our incident management process" | Mode 1, IT and Digital Service Delivery, starts at Step 0A (flow unit), one question at a time |
| "Calculate the DLI: Waste Score 14/27, Flow Ratio 12%, Complexity 60/100, Value Alignment 45%" | Mode 5: applies the framework formula, then asks for target quadrant and frontier to interpret it |
| "Management can't tell me the target quadrant" | Stops at Step 0B: strategic reflection precedes the assessment; does not improvise a target |

If answers come back in Italian or as long theory lectures, the instructions were not pasted in full.
