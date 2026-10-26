# Guida Setup — Gem "Lean Advisor" per Gemini

Porting della skill Claude `lean-advisor` (DLF v2.4) in un Gem Gemini.

## Contenuto del pacchetto

```
lean-advisor-gem/
├── GEM_ISTRUZIONI.md              → da incollare nel campo "Istruzioni" del Gem
├── GEM_SETUP_GUIDE.md             → questa guida
└── knowledge/                     → 7 file da caricare come Knowledge
    ├── lean-advisor-istruzioni-complete.md   (versione integrale delle istruzioni)
    ├── digital-lean-framework.md             (framework master v2.4)
    ├── assessment-dli.md
    ├── muda-checklist.md
    ├── sprint-kaizen.md
    ├── legge-zero-workflow.md
    └── guida-operativa.md
```

7 file su un cap di 10 → 3 slot liberi per estensioni future.

## Setup passo-passo

1. Vai su **gemini.google.com** → menu a sinistra → **Esplora Gems** → **Nuovo Gem** (la creazione è possibile solo da web, non da mobile)
2. **Nome**: `Lean Advisor` (o `Lean Advisor — DLF v2.4`)
3. **Istruzioni**: apri `GEM_ISTRUZIONI.md`, copia tutto il contenuto e incollalo nel campo istruzioni. **NON usare "Use Gemini to re-write instructions"**: riscriverebbe il testo perdendo la fedeltà al framework
4. **Knowledge** → **Aggiungi file**: carica i 7 file della cartella `knowledge/`
   - Se l'upload di file `.md` fallisse, rinominali in `.txt` (il contenuto resta identico)
   - Alternativa: caricali su Google Drive e collegali da Drive, così un aggiornamento del file si propaga al Gem
5. **Default tool**: lascia "No default tool" (il Lean Advisor è conversazionale)
6. (Opzionale) **Disable knowledge citations**: consigliato lasciare le citazioni ATTIVE (tracciabilità verso il framework)
7. **Anteprima**: nel pannello destro, testa con i prompt di smoke test qui sotto
8. **Salva** (l'anteprima non salva automaticamente)

## Smoke test post-setup

| Prompt | Comportamento atteso |
|---|---|
| "Voglio fare un assessment del nostro processo di incident management" | Instrada in Modalità 1, riconduce a IT and Digital Service Delivery, parte dallo Step 0A (unità di flusso), UNA domanda alla volta |
| "Calcolami il DLI: Waste Score 14/27, Flow Ratio 12%, Complexity 60/100, Value Alignment 45%" | Modalità 5: applica la formula del framework, poi chiede quadrante target e frontiera per l'interpretazione, non si ferma al numero secco |
| "Il management non sa dirmi il quadrante target" | Si ferma allo Step 0B e dichiara che la riflessione strategica precede l'assessment, NON improvvisa un target |

Se il Gem risponde con lezioni teoriche lunghe o fa tutte le domande insieme, le istruzioni non sono state incollate integralmente.

## Differenze rispetto alla skill Claude (limiti noti)

- **Nessun caricamento selettivo**: il Gem fa retrieval sui knowledge file; il recupero è probabilistico, non deterministico. Le istruzioni compensano indicando quale file consultare per ciascuna modalità
- **Nessuna generazione file nativa**: il Gem produce markdown strutturato (o Canvas)
- **Nessun trigger automatico**: il Gem si attiva solo aprendolo esplicitamente
- **Governance versioni**: il Gem è uno snapshot della v2.4. Quando il framework evolve, i knowledge file vanno riaggiornati

## Aggiornamento futuro

1. Scarica i file aggiornati da questo repository
2. Modifica il Gem → sostituisci i file in Knowledge
3. Aggiorna il riferimento di versione nelle istruzioni (cerca "v2.4")
4. Ripeti lo smoke test
