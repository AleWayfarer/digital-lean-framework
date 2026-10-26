# Changelog

Versioning: the master framework drives the baseline version. Each operational asset carries its own version and declares the master version it is compatible with.

## DLF v2.4.1 — packaging fix (2026-10-26)

No change to the framework text: all assets keep the versions of v2.4.

- Figures added: Efficiency Matrix and Efficiency Frontier (Italian in `framework/it/`, English in `framework/en/img/`).
- Italian PDF editions with figures added in `pdf/it/`.
- Lean Advisor packages (Claude, Gemini; IT and EN): the copy of the master framework realigned with the canonical text; links to figures and PDFs now point to this repository.
- Slides "Lean Digital: The Next Step" (EN, 41 slides) added in `talks/`.

## DLF v2.4 — first public release (2026-10-26)

| Asset | Version | Compatible with |
|---|---|---|
| Digital Lean Framework (master) | 2.4 | — |
| Operating Guide | 1.4 | DLF v2.4 |
| DLI Assessment | 2.4 | DLF v2.4 · Operating Guide v1.4 |
| Muda Checklist | 2.3 | DLF v2.4 |
| Sprint Kaizen | 2.2 | DLF v2.4 |
| Law Zero Workflow | 2.1 | DLF v2.4 |
| Lean Advisor skill (Claude, Gemini; IT and EN) | — | DLF v2.4 |
| DLF on a page | Companion 1.4 | DLF v2.4 |

Highlights of the v2.4 baseline: framework positioned explicitly as an application layer for lean thinking; four cultural values separated from the five pillars; Pillar 5 (flow visibility and digital Jidoka); three sources of inefficiency; Efficiency Matrix with reachable frontier; Lean Test against lean theater; 4 operational tracks + 1 transversal layer (Digital Transformation Programs); five practitioner superpowers.

Framework lineage: v2.0 → v2.1 → v2.2 → v2.3 → v2.4 (pre-publication, maintained privately).

## Asset history (pre-publication)

#### assessment-dli v2.4
  - Allineamento al DLF v2.4 (master modificato: struttura riorganizzata con Sez 2 Architettura, Sez 3 Framework di applicazione lean, Sez 4 Valori Culturali separati, Sez 12 estesa con transversal layer Digital Transformation Programs, Sez 13 estesa a 5 Superpoteri)
  - Cross-reference a sezioni del master aggiornati a v2.4 — in particolare il framing "framework di applicazione del lean thinking" che in v2.3 era Sez 2, in v2.4 è Sez 3
  - Allineamento a Guida Operativa v1.4 (era v1.3)
  - Nessuna modifica concettuale agli Step 0-6, alla formula DLI composito, ai layer del Report DLI
  - Report DLI rinominato da "Report DLI v2.3" a "Report DLI v2.4" per coerenza con master

#### assessment-dli v2.3
  - Step 0A esteso → unità di flusso + confini del sistema + livello di astrazione (DLF Sez 6.5)
  - Step 0E nuovo — Visibilità del flusso (Pillar 5 Jidoka digitale). Valutazione 4 dispositivi (visual mgmt, anomaly detection, stop-the-line, built-in quality)
  - Step 3 esteso → mappatura dei muda dominanti alle tre fonti di inefficienza (lungo throughput time / WIP alto / molti riavvii)
  - Step 5 esteso → azioni Jidoka-aware (dashboard di flow e soglie come parte dello sprint) e fonte-aware (intervento sulla fonte di inefficienza dominante)
  - Report DLI con nuove colonne: Visibilità del flusso (Pillar 5) + Tre fonti di inefficienza dominanti
  - Framework: framing "framework di applicazione del lean thinking", strategia d'impresa vs operativa, PULL e Standardizzazione esplicitate
  - Formula DLI composito INVARIATA. Pillar 5 e fonti entrano come layer nel Report, non come fattori del composito

#### assessment-dli v2.2
  - Step 0B esteso → bidimensionale, posizionamento sulla Matrice di Efficienza (quadrante attuale + target + frontiera raggiungibile)
  - Step 0D nuovo — Catena cliente-fornitore interno (Pillar 2). Compilazione matrice per sotto-fase (cliente interno / output / bisogno indiretto generato)
  - Step 5 esteso → matrice-aware. Oltre alle azioni bottleneck/WIP/variabilità, azioni concrete in funzione della transizione di quadrante (Da → A) e dichiarazione frontiera raggiungibile come tetto realistico del DLI
  - Step 6 esteso → tracking del movimento sulla matrice di efficienza e aggiornamento della frontiera raggiungibile
  - Formula DLI composito INVARIATA rispetto a v2.0/v2.1. Cambia solo l'interpretazione (DLI letto come % della frontiera raggiungibile, non % dell'ideale teorico)

#### assessment-dli v2.1
  - Step 0 espanso con sotto-step 0C — identificazione bisogni diretti e indiretti
  - Step 2 espanso con raccolta WIP per step, identificazione bottleneck, variabilità qualitativa
  - Step 5 con nuova regola di prioritizzazione (bottleneck → WIP → variabilità) come primo criterio
  - Formula DLI composito invariata (le tre metriche di fisica del flusso non entrano nel composito ma orientano il piano)

#### muda-checklist v2.3
  - Allineamento al DLF v2.4 (master modificato, struttura: 5 Pillar + 5 Principi Operativi + 4 Valori Culturali + 5 Superpoteri + 4+1 Domini)
  - Fix ordinamento muda 8/9 — coerente con master v2.4 Sez 10.3 (#8 Unused Talent classico, #9 Perfection Trap originale DLF)
  - Nessuna modifica a scoring, domande diagnostiche, metriche quantitative, mappatura bisogno indiretto, mappatura tre fonti
  - Cross-reference al master aggiornati a v2.4

#### muda-checklist v2.2
  - Aggiunta annotazione "Fonte di inefficienza tipica" per ciascuno dei 9 muda (lungo throughput time / WIP alto / molti riavvii)
  - Riferimento al framework v2.3 (Sez 8.1 — Le tre fonti di inefficienza)
  - Aggiunto raccordo con Pillar 5 Jidoka (per i muda visibili solo in mancanza di dashboard di flow)
  - Nessuna modifica a scoring, domande diagnostiche o metriche quantitative

#### muda-checklist v2.1
  - Aggiunta annotazione "Bisogno indiretto associato" per ciascuno dei 9 muda
  - Aggiunta nota di lettura sui muda con bisogno indiretto SÌ (doppio dividendo)
  - Nessuna modifica a scoring, domande diagnostiche o metriche quantitative

#### sprint-kaizen v2.2
  - Allineamento al DLF v2.4 (master modificato — struttura riorganizzata, Pillar 5 Sez 9 invariato, KAIZEN Sez 10.5 invariato)
  - Nessuna modifica concettuale ai rituali sprint, ai 6 principi, alle metriche di sprint
  - Cross-reference al master aggiornati a v2.4

#### sprint-kaizen v2.1
  - Sprint Planning esteso → dichiarazione del dashboard di flow e delle soglie di anomaly detection attive (Pillar 5 DLF Sez 9)
  - Monday Stand-up esteso → verifica delle deviazioni del flow (non solo task done/todo)
  - Sprint Review + Retrospettiva esteso → "standardizzazione" come output esplicito (cosa di questo sprint diventa nuovo standard? Quale runbook/template si aggiorna?)
  - Principio aggiuntivo: "Sprint senza dashboard di flow = JIT cieco — non parte"

#### legge-zero-workflow v2.1
  - Allineamento esplicito al DLF v2.4 (master modificato, struttura: 5 Pillar + 5 Principi Operativi + 4 Valori Culturali + 5 Superpoteri + 4+1 Domini)
  - Nessuna modifica concettuale ai 3 percorsi (A non digitalizzato / B remediation / C processi umani)
  - Nessuna modifica al Decision Record template
  - Aggiunto front-matter di compatibilità con master v2.4
