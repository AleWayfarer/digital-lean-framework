---
asset: sprint-kaizen
version: 2.2
compatible-with: DLF v2.4
author: Alessio Setaro
license: CC BY-NC-ND 4.0
---

# Sprint Kaizen — Guida Operativa e Template (v2.2)

Il miglioramento non è un progetto — è un'abitudine.
Il DLF struttura il Kaizen in sprint di 2 settimane con rituali definiti.

**Cosa cambia in v2.2** (questa versione): allineamento al DLF v2.4 (master
modificato). Nessuna modifica concettuale ai rituali sprint, ai 6 principi,
alle metriche.

**Cosa è stato aggiunto in v2.1** (riferimento storico): lo sprint Jidoka-aware.
Ogni sprint dichiara il dashboard di flow su cui si misura, almeno una soglia
di anomaly detection attiva, e produce uno standard aggiornato nella
retrospettiva. Allineato a DLF v2.4 — Pillar 5 (Jidoka digitale, Sez 9) e
KAIZEN 10.5.2 (capacità evolutiva).

---

## Indice

1. [Principi dello Sprint Kaizen](#principi)
2. [Struttura dello Sprint](#struttura)
3. [Template: Sprint Planning](#planning)
4. [Template: Monday Stand-up](#standup)
5. [Template: Sprint Review + Retrospettiva](#review)
6. [Come collegare lo sprint al DLI](#collegamento-dli)
7. [Regole operative](#regole)

---

## <a name="principi"></a>Principi dello Sprint Kaizen

1. **Affettare l'elefante**: nessun intervento deve essere più grande di ciò che
   un team può completare in 2 settimane. Se è più grande, va spezzato.
2. **Misurare prima di partire**: definisci le metriche di successo PRIMA dello sprint,
   non dopo. Altrimenti il successo diventa soggettivo.
3. **Owner singolo**: ogni intervento ha un owner (una persona, non un team).
   Il team supporta, l'owner risponde.
4. **Collegamento esplicito al DLI**: ogni sprint deve dichiarare quale dimensione
   del DLI impatta e come.
5. **Ritmo, non eroismo**: la potenza del Kaizen è la cadenza, non il singolo sprint
   brillante. 26 sprint/anno battono 2 progetti da 6 mesi.
6. **(v2.1) Sprint senza dashboard di flow = JIT cieco — non parte**: ogni
   sprint dichiara dove sta il dashboard di flow (lead time, WIP, throughput)
   e almeno una soglia di anomaly detection. Se non si sa dove guardare il
   flow mentre lo si modifica, lo sprint è teatro lean.
7. **(v2.1) La retrospettiva produce uno standard**: il miglioramento si
   propaga solo se diventa standard aggiornato. Se la retrospettiva non
   produce un aggiornamento di runbook/template/checklist, il miglioramento
   è personale e non si propaga (capacità evolutiva, DLF v2.4 Sez 10.5.2).

---

## <a name="struttura"></a>Struttura dello Sprint (2 settimane)

| Giorno | Rituale | Durata | Chi |
|---|---|---|---|
| Giorno 1 | Sprint Planning | 1h | Team + owner processo |
| Ogni lunedì | Monday Stand-up | 15 min | Team |
| Giorno 10 | Sprint Review + Retrospettiva | 1h | Team + stakeholder |

---

## <a name="planning"></a>Template: Sprint Planning (1h)

### Guida il planning raccogliendo queste informazioni:

**1. Obiettivo dello sprint (una frase)**
- Domanda: "Cosa vuoi ottenere in queste 2 settimane? Dillo in una frase."
- Se la frase è vaga ("migliorare il processo"), sfida: "Migliorare cosa,
  specificamente? Quale muda aggredisci? Quale metrica muovi?"

**2. Interventi concreti (1-3 max)**
Per ciascun intervento:
- Cosa fai (descrizione operativa)
- Chi è l'owner
- Done when (criterio di completamento)
- Se l'intervento è > 2 settimane: "Troppo grande. Come lo spezziamo?"

**3. Metriche di successo**
- Domanda: "Come saprai che ha funzionato? Quale numero cambia?"
- Ogni metrica deve avere: baseline (valore attuale) e target (valore atteso)
- Se la metrica non è misurabile: "Se non puoi misurarlo, come fai a sapere
  che è migliorato?"

**4. Collegamento al DLI**
- Domanda: "Quale dimensione del DLI impatti con questo sprint?"
  (Waste Score, Flow Ratio, Complexity Score, Value Alignment)
- DLI attuale → DLI target atteso

**5. (v2.1) Dichiarazione Jidoka digitale — Pillar 5**
- "Dove sta il dashboard di flow per questo sprint? (Link, cruscotto, board fisica)"
- "Quale soglia di anomaly detection è attiva? Su quale metrica (WIP, lead time, throughput)?"
- "Se nessuno dei tre interventi sposta un quality gate da 'a valle' a 'built-in', perché?"
- Se manca il dashboard di flow: il primo intervento dello sprint diventa
  introdurre il dashboard. *Sprint senza visibilità di flow = JIT cieco.*

### Output Sprint Planning:

```
🏃 SPRINT KAIZEN #[N] — [Data inizio] → [Data fine]
Processo: [nome]

OBIETTIVO:
[una frase]

INTERVENTI:
1. [Cosa] — Owner: [chi] — Done when: [criterio]
2. [Cosa] — Owner: [chi] — Done when: [criterio]
3. [Cosa] — Owner: [chi] — Done when: [criterio]

METRICHE:
• [Metrica 1]: baseline [X] → target [Y]
• [Metrica 2]: baseline [X] → target [Y]

COLLEGAMENTO DLI:
• Dimensione impattata: [quale]
• DLI attuale: [X] → DLI target: [Y]

JIDOKA (v2.1):
• Dashboard di flow: [link/luogo]
• Soglie attive: [metrica → soglia]
• Quality gate spostato a built-in (se applicabile): [quale]

RITUALI SCHEDULATI:
• Stand-up: ogni lunedì [ora], 15 min
• Review + Retro: [data], [ora], 1h
```

---

## <a name="standup"></a>Template: Monday Stand-up (15 min)

### Struttura (3 domande per persona):

**1. Cosa è stato fatto dall'ultimo stand-up?**
- Focus su fatti, non su intenzioni. "Ho fatto X" non "sto lavorando su X."

**2. Cosa faremo questa settimana?**
- Azioni concrete con deadline infrasettimanali.

**3. Blocchi e dipendenze?**
- Cosa ti ferma? Di chi/cosa hai bisogno?
- Se un blocco dura > 3 giorni: escalation immediata.

**4. Aggiornamento rapido metriche**
- Dove siamo rispetto al target? On track / off track / bloccato.

**5. (v2.1) Verifica del flow — Pillar 5**
- "Cosa dice il dashboard di flow questa settimana?" (lead time corrente,
  WIP corrente, throughput corrente vs baseline)
- "Sono scattate soglie di anomaly detection? Quali? Cosa hanno attivato?"
- Se il dashboard mostra deviazione ma nessuna azione è stata attivata, è
  segnale che il dispositivo Jidoka è teorico — discuterne nello stand-up.

### Output Stand-up:

```
📌 STAND-UP — Lunedì [data]
Sprint #[N] — Settimana [1/2]

AVANZAMENTO:
• [Intervento 1]: [stato] — [dettaglio]
• [Intervento 2]: [stato] — [dettaglio]

BLOCCHI:
• [Blocco, se presente] — Azione: [chi fa cosa entro quando]

METRICHE:
• [Metrica 1]: attuale [X] vs target [Y] → [on track / off track]

FOCUS SETTIMANA:
• [Azione 1 con deadline]
• [Azione 2 con deadline]
```

---

## <a name="review"></a>Template: Sprint Review + Retrospettiva (1h)

### Parte 1 — Sprint Review (30 min): risultati vs obiettivi

**1. Obiettivo raggiunto?**
- Sì / Parzialmente / No
- Con dati, non con impressioni.

**2. Metriche: baseline → risultato**
- Per ogni metrica: valore di partenza → valore attuale → target → delta
- Se off track: perché? Root cause, non scuse.

**3. DLI aggiornato**
- Ricalcola le dimensioni impattate
- DLI pre-sprint → DLI post-sprint → delta

### Parte 2 — Retrospettiva (30 min): apprendimento

**4 domande (mantenute da v2.0):**
1. **Cosa ha funzionato?** (da ripetere)
2. **Cosa non ha funzionato?** (da cambiare)
3. **Cosa abbiamo imparato?** (insight)
4. **Cosa cambiamo nel prossimo sprint?** (azione concreta)

**5ª domanda (v2.1) — Standardizzazione**
5. **Cosa di questo sprint diventa nuovo standard?** Quale runbook, template,
   checklist, definition of done, playbook va aggiornato?
   *Senza standardizzazione, il miglioramento è personale e non si propaga.
   Capacità evolutiva (DLF v2.4 Sez 10.5.2).*

### Output Review + Retro:

```
📋 SPRINT REVIEW + RETRO — Sprint #[N]
Data: [data]

OBIETTIVO: [raggiunto / parzialmente / non raggiunto]

RISULTATI:
• [Intervento 1]: [completato / parziale / non completato] — [dettaglio]
• [Intervento 2]: [completato / parziale / non completato] — [dettaglio]

METRICHE:
• [Metrica 1]: baseline [X] → risultato [Y] → target [Z] — [Δ]
• [Metrica 2]: baseline [X] → risultato [Y] → target [Z] — [Δ]

DLI:
• Pre-sprint: [X] → Post-sprint: [Y] → Delta: [+/- Z]
• Dimensioni mosse: [quali]

JIDOKA (v2.1):
• Dashboard di flow letto regolarmente? [sì/no — frequenza]
• Soglie scattate durante lo sprint: [quali — cosa hanno attivato]

RETROSPETTIVA:
✅ Cosa ha funzionato: [...]
❌ Cosa non ha funzionato: [...]
💡 Cosa abbiamo imparato: [...]
🔄 Cosa cambiamo: [...]

STANDARDIZZAZIONE (v2.1):
📒 Nuovo/aggiornato standard: [runbook / template / checklist / DoD / playbook]
📒 Owner del nuovo standard: [chi mantiene]
📒 Comunicazione del nuovo standard: [a chi va comunicato, come]

▶️ PROSSIMO SPRINT:
• Obiettivo proposto: [...]
• Muda target: [...]
```

---

## <a name="collegamento-dli"></a>Come collegare lo sprint al DLI

Ogni sprint deve dichiarare esplicitamente:

| Domanda | Perché |
|---|---|
| Quale muda aggredisci? | Per sapere dove misurare il miglioramento |
| Quale dimensione DLI impatti? | Per collegare lo sprint alla baseline |
| Quale metrica muovi? | Per misurare il successo con dati |
| Di quanto? | Per avere un target concreto |

Mappatura muda → dimensione DLI:

| Muda | Impatta principalmente |
|---|---|
| Overprocessing | Complexity Score, Waste Score |
| Waiting | Flow Ratio, Waste Score |
| Overproduction | Waste Score, Value Alignment |
| Defects | Waste Score, Flow Ratio |
| Motion | Complexity Score, Waste Score |
| Inventory | Waste Score, Complexity Score |
| Transport | Complexity Score, Flow Ratio |
| Unused Talent | Value Alignment, Waste Score |
| Perfection Trap | Flow Ratio, Value Alignment |

---

## <a name="regole"></a>Regole Operative

1. **Max 3 interventi per sprint**: se ne metti di più, non ne completi nessuno.
2. **Ogni intervento ha UN owner**: non "il team". Una persona.
3. **Se non puoi misurarlo, non metterlo nello sprint**: trova la metrica prima.
4. **Stand-up = 15 minuti MAX**: se serve di più, c'è un problema di scope.
5. **Review con stakeholder**: non solo il team. Chi riceve il valore del processo
   deve vedere i risultati.
6. **La retro produce almeno 1 cambiamento**: altrimenti è un rituale vuoto.
7. **Sprint consecutivi**: il prossimo sprint si pianifica alla fine del precedente.
   Mai gap tra sprint — il Kaizen è continuo.
8. **Documentare i delta**: il valore dello Sprint Kaizen si vede nel tempo,
   non nel singolo sprint. Tieni traccia dei DLI sprint su sprint.
