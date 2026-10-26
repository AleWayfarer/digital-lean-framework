---
asset: assessment-dli
version: 2.4
compatible-with: DLF v2.4 · Guida Operativa v1.4
author: Alessio Setaro
license: CC BY-NC-ND 4.0
---

# Assessment DLI — Guida Operativa Completa (v2.4)

Questo file guida il Lean Advisor attraverso l'intero percorso di assessment
del Digital Lean Index (Step 0-6). Segui ogni step in ordine. Non saltare.

**Cosa cambia in v2.4** (questa versione): allineamento al **DLF v2.4** (master
modificato) e alla **Guida Operativa v1.4**. Cross-reference a sezioni del
master aggiornati — in particolare il framing "framework di applicazione del
lean thinking" che in v2.3 era Sez 2, ora è Sez 3 nel master. Nessuna modifica
concettuale agli Step 0-6 né alla formula DLI composito.

**Cosa è stato aggiunto in v2.3** (riferimento storico): lo Step 0 è passato
da 4 a 5 sotto-step. Lo Step 0A è esteso con confini del sistema e livello di
astrazione del processo. Lo Step 0E è nuovo — valutazione del Pillar 5 Jidoka
digitale (visual management, anomaly detection, stop-the-line, built-in quality).
Lo Step 3 si è arricchito mappando i muda dominanti alle tre fonti di
inefficienza (lungo throughput time / WIP alto / molti riavvii). Lo Step 5 ha
introdotto azioni Jidoka-aware e fonte-aware. Il Report DLI ha acquisito due
nuove colonne (Visibilità del flusso, Tre fonti di inefficienza dominanti).
La formula del composito DLI resta INVARIATA.
Allineato a DLF v2.4 (5 Pillar incluso Jidoka digitale + 4 Valori + Matrice +
Tre fonti di inefficienza + framing "framework di applicazione del lean
thinking" + Strategia d'impresa vs operativa).

**Cosa cambia in v2.2** (riferimento storico): estensione strutturale dello
Step 0 (da 3 a 4 sotto-step con 0B bidimensionale e 0D nuovo), Step 5
matrice-aware, Step 6 con tracking movimento matrice.

**Cosa cambia in v2.1** (riferimento storico): tre integrazioni concrete da
*This is Lean* di Modig e Åhlström, documentate nel DLF v2.1 come "Tre Leggi
del Flusso" + lente diagnostica dei bisogni. Operativamente: sotto-step 0C,
dati aggiuntivi nello Step 2, regola di priorità nello Step 5.

---

## Indice

1. [Step 0 — Orientamento Strategico](#step-0)
   - 0A — Identificare l'Unità di Flusso, Confini, Astrazione **(esteso v2.3)**
   - 0B — Posizionamento sulla Matrice di Efficienza **(esteso v2.2 — bidimensionale)**
   - 0C — Identificare bisogni diretti e indiretti
   - 0D — Catena cliente-fornitore interno **(nuovo v2.2)**
   - 0E — Visibilità del flusso (Pillar 5 Jidoka digitale) **(nuovo v2.3)**
2. [Step 1 — Selezione del Processo](#step-1)
3. [Step 2 — Digital Value Stream Map](#step-2)
4. [Step 3 — Muda Assessment](#step-3) **(fonte-aware v2.3)**
5. [Step 4 — Calcolo DLI](#step-4)
6. [Step 5 — Piano di Intervento](#step-5) **(matrice-aware v2.2 + Jidoka-aware/fonte-aware v2.3)**
7. [Step 6 — Ri-assessment](#step-6) **(tracking matrice v2.2)**
8. [Formula DLI Composito](#formula)
9. [Tabella di Interpretazione](#interpretazione)

---

## <a name="step-0"></a>Step 0 — Orientamento Strategico

Prima di qualsiasi calcolo, **quattro** domande fondamentali (v2.2: era 3 in v2.1).

### 0A — Identificare l'Unità di Flusso, i Confini, il Livello di Astrazione (v2.3 — esteso)

> Chi o cosa attraversa il processo? Quali sono i confini del processo che stai analizzando? A che livello di astrazione lo stai guardando?

Lo Step 0A in v2.3 dichiara tre cose, non una sola. L'unità di flusso (chi/cosa
attraversa), i confini del sistema (dove inizia/finisce ciò che chiami "il
processo"), e il livello di astrazione (macro/meso/micro). Confini e livello
sono **scelte strategiche esplicite**, non assunzioni a priori.

**Unità di flusso.**

Domande da porre:
- "Descrivi il processo che vuoi analizzare in una frase."
- "Chi o cosa entra nel processo e chi o cosa ne esce trasformato?"
- "Se dovessi seguire un singolo 'oggetto' dall'inizio alla fine, cos'è?"

L'unità di flusso NON è lo strumento (il ticket, l'alert, il corso). È il valore
che attraversa il processo.

| Dominio | Unità di flusso corretta | Unità di flusso SBAGLIATA |
|---|---|---|
| Cybersecurity | Il processo di business da garantire integro | L'alert, l'incidente, il ticket |
| IT Service Delivery | La richiesta dell'utente (il bisogno) | Il ticket IT |
| Formazione | Il bisogno di competenza → competenza applicata | Il corso, le ore di aula |
| Digital Transformation | Il processo di business da trasformare | Il progetto IT, la feature |
| HR/People | Il candidato → collaboratore produttivo | Il CV, la posizione aperta |
| Decision-making | La decisione da prendere | Il report, il meeting |

Se l'utente confonde l'unità di flusso con lo strumento, correggi:
> "Attenzione: stai descrivendo lo strumento (il ticket), non l'unità di flusso.
> L'unità di flusso è ciò che ha valore per il cliente del processo. Chi è il
> cliente? Di cosa ha bisogno?"

**Confini del sistema (v2.3).**

Lo stesso processo può essere letto a confini diversi, e ogni scelta produce
un throughput time diverso e bisogni indiretti diversi. La scelta dei confini
va dichiarata esplicitamente prima di procedere.

Domande da porre:
- "Dove dichiariamo che il processo inizia? Il primo trigger osservabile (es. apertura ticket), il bisogno latente del cliente (quando ha cominciato ad averne bisogno), o un punto intermedio?"
- "Dove dichiariamo che il processo finisce? Chiusura formale, validazione in produzione, conferma del cliente, assenza di problema per N giorni?"
- "Cosa stiamo cercando di vedere — il processo come lo descrive il management, o il processo come lo vive il cliente?"

Confini diversi → throughput time diverso → piani d'intervento diversi. Non
c'è una scelta giusta a priori; c'è una scelta coerente con cosa si vuole
ottimizzare.

**Livello di astrazione (v2.3).**

Domande da porre:
- "A che livello stiamo guardando il processo? Catena di team (macro), catena di ruoli dentro un team (meso), catena di attività dentro un ruolo (micro)?"
- "Per un primo assessment, di norma macro. Se emerge un bottleneck specifico, si zooma."

Output Step 0A v2.3:
- Unità di flusso: [cosa]
- Confini dichiarati: [da X a Y, con razionale]
- Livello di astrazione: [macro / meso / micro]

RED FLAG: se l'utente non sa rispondere "dove inizia e dove finisce il
processo", non procedere oltre lo Step 0A. La discussione dei confini è essa
stessa output di valore.

### 0B — Posizionamento sulla Matrice di Efficienza (v2.2 — esteso bidimensionale)

> Dove sta il processo oggi sulla Matrice di Efficienza (flow × resource), e
> dove vuole essere il management (quadrante target)?

Lo Step 0B in v2.2 diventa bidimensionale. Non più solo "resource o flow?",
ma posizionamento su due dimensioni indipendenti — la Matrice di Efficienza
del Pillar 3 (DLF v2.4 Sezione 7.5). Si chiede al management dove sta oggi
(quadrante attuale) e dove vuole essere (quadrante target — l'ambizione
strategica). Output formale: posizione attuale + target sulla matrice +
frontiera raggiungibile preliminare.

**I quattro quadranti:**

| Quadrante | Flow | Resource | Tipologia di scelta |
|---|---|---|---|
| **Deserto** | Basso | Basso | Mai scelto deliberatamente. Va uscito universalmente. |
| **Isole** | Basso | Alto | Modello low-cost: cliente paga il prezzo, accetta flow basso. Scelta legittima (es. low-cost airline, fast food, retail discount). |
| **Oceano** | Alto | Medio/basso | Modello flow lean: cliente paga la velocità. Lean classico. Servizi premium, B2B time-sensitive, sanità, IT critico. |
| **Stato Perfetto** | Alto | Alto | Asintoto teorico. Benchmark, non destinazione realistica. |

**Domande per posizionare il processo ATTUALE:**
- "Quanto del throughput time è effettivamente lavoro vs attesa? (Flow alto/basso)"
- "Le risorse del team sono sature al 100% o hanno buffer di capacità? (Resource alto/medio/basso)"
- "Quando arriva un picco, cosa succede: si accumula coda (resource alto) o
  si riallocano risorse (resource medio con buffer)?"
- "Le metriche operative oggi misurano l'utilizzo o la velocità del flusso?"

**Domande per dichiarare il quadrante TARGET:**
- "Qual è il modello di business del processo? Il cliente paga la velocità o il prezzo?"
- Se il cliente paga la velocità → quadrante target = Oceano
- Se accetta il flow basso in cambio del prezzo → quadrante target = Isole
- Se il quadrante attuale è Deserto → il target è qualunque quadrante diverso

**Non c'è una scelta giusta a priori — c'è una scelta coerente con il modello
di business.** Il framework non prescrive: aiuta a far emergere la scelta
consapevole.

**Frontiera raggiungibile (preliminare):** valuta qualitativamente quale tetto
realisticamente puoi raggiungere dato il livello di variabilità che osservi
nel processo. Più alta la variabilità, più bassa la frontiera. Esempi:
- Variabilità bassa → frontiera ALTA (Stato Perfetto approcciabile, ~90+)
- Variabilità media → frontiera MEDIA (parte alta del quadrante target, ~75-85)
- Variabilità alta → frontiera BASSA (solo parte bassa del quadrante target, ~60-70)

Questa è una valutazione preliminare che verrà raffinata in Step 2 dopo aver
mappato il VSM e raccolto i dati di fisica del flusso.

**RED FLAG**: Se l'utente dichiara come target lo "Stato Perfetto" senza
qualificarlo, intervieni:
> "Lo Stato Perfetto è asintoto teorico — è benchmark, non destinazione.
> Ridichiariamo il target come Oceano (o Isole, se modello low-cost), e
> usiamo lo Stato Perfetto come direzione di tensione, non come obiettivo
> raggiungibile."

### 0C — Identificare bisogni diretti e indiretti

> Qual è il bisogno *diretto* dell'unità di flusso? Quali bisogni *indiretti*
> il processo sta generando perché il flow è basso?

Questa è una lente diagnostica fondamentale presa da *This is Lean* di
Modig e Åhlström. Distingue il valore che l'unità di flusso vuole davvero
dal "lavoro di trazione" che il processo genera quando funziona male.

**Definizioni operative:**

- **Bisogno diretto**: il valore "duro" che il cliente/utente effettivamente
  vuole. Per un ticket IT: l'accesso ripristinato. Per un incident di
  sicurezza: la mitigazione del rischio di business. Per una richiesta di
  formazione: la competenza applicabile.

- **Bisogno indiretto**: il valore "soft" che nasce *mentre l'unità di flusso
  aspetta o attraversa un processo lento*. Informazione, rassicurazione,
  aggiornamento, contatto. Quando il flow è veloce, sparisce. Quando il flow
  è lento, genera lavoro aggiuntivo: chiamate di sollecito, status update,
  dashboard di tracking, escalation, riunioni di review backlog.

**L'insight chiave**: i bisogni indiretti non sono valore — sono **sintomo
di flow basso**. Il lavoro che generano è muda, anche se sembra "servizio
al cliente".

**Domande da porre:**

- "Qual è il bisogno diretto dell'unità di flusso? Cosa vuole davvero
  ottenere il cliente del processo?"
- "Mentre il processo è in corso (lavorazione o attesa), il cliente
  contatta qualcuno per chiedere aggiornamenti? Quanto spesso?"
- "Ci sono dashboard, report di stato, riunioni di review backlog, o
  comunicazioni di status che esistono solo per gestire l'attesa?"
- "Ci sono escalation che si attivano quando il processo si dilunga? Quante?"
- "Se il processo chiudesse in metà del tempo attuale, quale di questi
  lavori sparirebbe?"

L'ultima domanda è la più utile: cristallizza quale lavoro è *generato* dal
flow basso vs quale lavoro è strutturale al processo.

**Red flag**: se l'utente dice "ma il customer support è valore per il
cliente!", correggi:
> "Distinzione importante: rispondere a una richiesta di stato perché il
> cliente non sa a che punto è il suo ticket NON è valore — è muda generato
> dal fatto che il processo non gli ha già dato risposta. Se il ticket si
> chiudesse in 4 ore invece che in 4 giorni, nessuno chiamerebbe per chiedere
> stato. Quel lavoro di support sparirebbe."

**Cosa farne**: i bisogni indiretti identificati orientano la lettura del
Muda Assessment (Step 3). I muda con bisogno indiretto associato hanno
priorità di intervento perché eliminandoli si elimina anche il lavoro di
trazione. Vedi colonna "Bisogno indiretto associato" nella Muda Checklist
del DLF v2.4.

**Output 0C:**
```
0C — BISOGNI
• Bisogno diretto: [una frase]
• Bisogni indiretti generati: [elenco]
• Lavoro di trazione stimato: [% del tempo del team allocato a servire
  bisogni indiretti, se quantificabile]
• Muda più impattati dai bisogni indiretti: [da identificare nello Step 3]
```

### 0D — Catena cliente-fornitore interno (v2.2 — nuovo)

> Scomponi il processo nelle sue sotto-fasi e per ognuna identifica:
> chi è il cliente interno, cosa gli stai consegnando, quale bisogno
> indiretto stai generando nel cliente interno.

Lo Step 0D è il Pillar 2 del DLF v2.4 (Sezione 6) operazionalizzato. Va
prima del VSM (Step 2) perché stabilisce come va letto il processo, non
solo cosa succede. Senza questo step il VSM rischia di descrivere bene un
processo letto male — un processo letto come "lista di task" anziché come
"catena di anelli di valore".

**Procedura operativa:**

1. Elenca le sotto-fasi del processo (di solito 4-8 step principali)
2. Per ciascuna sotto-fase, identifica il **cliente interno** (lo step a
   valle): nome, ruolo, team. Risposta vaga ("poi va in operations") = pillar
   non applicato — chiedi di scendere a specifico
3. Per ciascuna sotto-fase, identifica l'**output consegnato** al cliente
   interno: dato, documento, decisione, sistema. Non astrazione, ma il
   "cosa" concreto
4. Per ciascuna sotto-fase, identifica il **bisogno indiretto generato**
   nel cliente interno: richieste di chiarimento, riconsegne, escalation,
   duplicazione di lavoro, status update
5. Per ciascuna sotto-fase, applica il **test diagnostico Pillar 2**:
   "Se elimino questo output, il cliente finale se ne accorge?". Se no,
   l'output è una convenzione interna sopravvissuta alla sua utilità —
   candidato all'eliminazione

**Template della matrice catena interna:**

| Sotto-fase | Cliente interno | Output consegnato | Bisogno indiretto generato |
|---|---|---|---|
| [es. Triage Incident] | [Analista L2] | [Ticket classificato + log iniziali] | [Re-classificazione se severity imprecisa] |
| [es. Analisi L2] | [Specialista risoluzione] | [Diagnosi documentata] | [Domande per chiarimenti se diagnosi superficiale] |
| [...] | [...] | [...] | [...] |

**RED FLAG**: Se una sotto-fase non ha un cliente interno chiaramente
identificabile, è candidato come waste strutturale (Overprocessing o
Inventory). Se nessuno a valle riceve davvero qualcosa di utile, perché
quella sotto-fase esiste?

**Cosa farne**: la matrice della catena interna diventa prerequisito del
VSM (Step 2), che ne estende le informazioni con tempi, WIP, variabilità.
La matrice catena interna è anche cruciale per lo Step 3 (Muda Assessment):
i bisogni indiretti GENERATI internamente sono spesso più numerosi di
quelli visibili al cliente finale.

**Output 0D:**
```
0D — CATENA CLIENTE-FORNITORE INTERNO
• Numero di sotto-fasi documentate: [N]
• Sotto-fasi senza cliente interno chiaro: [elenco — candidati a eliminazione]
• Bisogni indiretti generati lungo la catena: [conteggio totale per anello]
• Anelli più "rumorosi" (alto volume di bisogni indiretti generati): [elenco]
```

### 0E — Visibilità del Flusso — Pillar 5 Jidoka digitale (v2.3 — nuovo)

> Il processo è osservabile mentre funziona? Esistono soglie esplicite di
> anomaly detection? Esiste un potere/dovere di "stop the line"? I quality
> gate sono built-in o a valle?

Lo Step 0E nasce in v2.3 dall'introduzione del Pillar 5 nel DLF (Sez 9 —
Jidoka digitale). Il principio: un processo che si vuole migliorare deve essere
visibile mentre funziona, non solo a posteriori. Senza visibilità, ogni
intervento è cieco — è "JIT senza Jidoka", una delle cause principali per cui
le iniziative lean falliscono.

**Le quattro domande di valutazione Jidoka digitale:**

| Dispositivo | Domanda | Livelli |
|---|---|---|
| Visual management | Esistono dashboard di flow real-time (lead time corrente vs baseline, WIP per step, throughput dei bottleneck)? O solo dashboard di stato ("quanti ticket aperti")? | Sì = flow / Parziale / Solo stato / No dashboard |
| Andon / Anomaly detection | Esistono soglie esplicite su WIP, lead time, SLA con notifica automatica? O le anomalie emergono solo quando esplodono? | Soglie esplicite automatiche / Soglie ma manuali / Solo SLA / No soglie |
| Stop the line | Il team ha potere/dovere dichiarato di fermare il delivery se la qualità non regge? E nei fatti viene esercitato? | Dichiarato + esercitato / Dichiarato ma mai esercitato / Non esiste |
| Built-in quality | I quality gate sono al passo (pre-merge, in pipeline, pre-deploy) o a fine processo (UAT finale, audit a posteriori)? | Built-in / Misti / A valle |

Domande di approfondimento:
- "Se il flow devia significativamente *adesso*, qualcuno lo saprebbe nei prossimi 5 minuti? 30 minuti? Domani? La settimana prossima?"
- "I dashboard esistenti sono alimentati per il team operativo (azione) o per il management (status)? Test: se il dashboard sparisce, il team operativo perde la capacità di intervento?"
- "Quando un'anomalia viene rilevata, c'è un'azione automatica/predefinita o si avvia una catena di email e riunioni?"
- "Il framework di sicurezza, il QA, la compliance — sono integrati nel processo o sono check di fine corsa?"

**RED FLAG dashboard di stato vs flow**: se la risposta a Visual Management è
"abbiamo dashboard di stato" e nient'altro, dichiara il gap esplicitamente:
"Avete visibilità di status, non di flow. Per il framework v2.4 questo è gap
del Pillar 5 — andrà aggredito tra i primi tre interventi dello Step 5."

**RED FLAG alert overload**: se "abbiamo decine di alert al giorno", chiedi
quanti sono effettivamente azionati. Se la risposta è "il 5-10%", non è
anomaly detection — è rumore. Le soglie vanno tarate sulla baseline reale del
processo, non sui default del tool.

**RED FLAG stop-the-line teorico**: se il team dichiara di avere "potere di
bloccare il delivery" ma nei fatti non lo esercita mai sotto la pressione del
business, è peggio dell'assenza del principio — crea l'illusione che il
dispositivo esista. Dichiarare esplicitamente la deviazione tra teoria e
pratica.

**Output 0E:**
```
0E — VISIBILITÀ DEL FLUSSO (Pillar 5)
• Visual management: [Sì = flow / Parziale / Solo stato / No dashboard]
• Anomaly detection: [livello con esempi di soglie]
• Stop the line: [Dichiarato+esercitato / Dichiarato non esercitato / Assente]
• Built-in quality: [Built-in / Misti / A valle]
• Gap Jidoka dominante: [quale dei 4 è più critico — driver per Step 5]
```

**Output complessivo Step 0 (v2.3):**
```
STEP 0 — ORIENTAMENTO STRATEGICO (v2.3)
• Processo: [nome]
• Unità di flusso: [cosa]
• Confini dichiarati: [da X a Y, con razionale]
• Livello di astrazione: [macro / meso / micro]
• Quadrante attuale sulla matrice: [Deserto/Isole/Oceano/Stato Perfetto]
• Quadrante target dichiarato: [...]
• Vettore di movimento: [da → a]
• Frontiera raggiungibile preliminare: [qualitativa, es. "~75 dato variabilità alta"]
• Bisogno diretto: [una frase]
• Bisogni indiretti generati: [elenco]
• Lavoro di trazione stimato: [% del tempo team]
• Matrice catena interna: [N sotto-fasi documentate]
• Visibilità del flusso (Jidoka): [4 livelli + gap dominante]
```

---

## <a name="step-1"></a>Step 1 — Selezione del Processo

Domande da porre:
- "Qual è il nome del processo?"
- "Dove inizia esattamente? (trigger di ingresso)"
- "Dove finisce esattamente? (output finale / condizione di completamento)"
- "Chi è l'owner del processo?"
- "Chi sono gli stakeholder principali?"
- "Quante persone/team sono coinvolti?"

**Output Step 1:**
```
STEP 1 — SELEZIONE
• Processo: [nome]
• Inizio: [trigger]
• Fine: [output/condizione]
• Owner: [chi]
• Stakeholder: [chi]
• Team coinvolti: [quanti, quali]
```

---

## <a name="step-2"></a>Step 2 — Digital Value Stream Map

Guida l'utente a mappare il processo end-to-end. Non serve un tool visuale —
basta una lista strutturata.

**Dalla v2.1** lo Step 2 raccoglie tre dati aggiuntivi che alimentano la lettura
con la lente delle Tre Leggi del Flusso (DLF v2.4, Sezione 7 — Pillar 3):

- **WIP per step** (Legge di Little): unità in coda o in lavorazione
  contemporaneamente
- **Bottleneck** (Legge dei Colli di Bottiglia): step identificato come
  collo di bottiglia, su base osservazionale
- **Variabilità qualitativa** (Legge dell'Effetto della Variabilità):
  valutazione qualitativa, NON quantitativa

Per ogni STEP del processo, raccogli:
1. **Nome dello step**
2. **Chi lo esegue** (persona/team/sistema)
3. **Tool utilizzato** (se digitale)
4. **Tempo di lavorazione** (processing time — quanto dura il lavoro effettivo)
5. **Tempo di attesa** (waiting time — quanto si aspetta prima/dopo)
6. **Handoff** (a chi passa e come)
7. **Punto di decisione?** (sì/no — se sì, quali le opzioni)
8. **WIP medio** (v2.1): unità in coda + in lavorazione, contate al
   momento dell'assessment. Esempio: "in media 15 ticket in coda + 3 in
   lavorazione = WIP 18"
9. **Variabilità qualitativa** (v2.1): stabile / variabile / molto variabile,
   sia in tempi di lavorazione sia in arrivi

Suggerisci di procedere così:
> "Partiamo dal trigger. Cosa succede quando [unità di flusso] entra nel
> processo? Chi fa cosa? Con quale tool? Quanto ci mette? Quanti sono già in
> coda davanti? I tempi sono stabili o variano? Poi cosa succede?"

Vai step by step. Non chiedere tutto il processo in un colpo.

### Identificazione del bottleneck (v2.1)

Una volta mappati tutti gli step, identifica il **bottleneck** del processo
con due segnali osservazionali (Legge dei Colli di Bottiglia):

1. **Dove si forma coda?** Lo step con il WIP più alto, o lo step di fronte
   al quale si accumula lavoro in attesa, è candidato bottleneck.
2. **Dove ci sono tempi morti a valle?** Lo step dopo il quale i sotto-processi
   aspettano è confermato come bottleneck.

> Se l'utente ha difficoltà a identificare il bottleneck, chiedi:
> - "Se un'unità di flusso entrasse adesso, in quale step rimarrebbe in coda
>   più a lungo?"
> - "Se quello step lavorasse il doppio più veloce, il throughput del
>   processo raddoppierebbe? (se sì, è il bottleneck)"

**Attenzione**: il bottleneck può essere una **persona** (decision authority
unica), un **livello di approvazione**, un **rito** (es. board mensile che
sblocca decisioni), un **sistema** (es. deployment window settimanale), o
un **vincolo esterno** (es. SLA di fornitore). Non sempre è uno step di
"lavoro" classico.

### Valutazione della variabilità (v2.1)

> **IMPORTANTE — Natura della valutazione.** Nel DLF la variabilità è
> valutata **qualitativamente, NON quantitativamente**. Per una misurazione
> rigorosa servirebbero dati di distribuzione su arrivi e tempi di processo
> (analisi statistica, coefficiente di variazione, eventualmente formula di
> Kingman). Questo è fuori dallo scope di un assessment DLI standard.
>
> La valutazione qualitativa è sufficiente a identificare la *presenza* del
> problema e orientare gli interventi. Per *dimensionare* il problema serve
> l'analisi quantitativa, che è un livello di maturità successivo del lean
> practitioner.

Domande qualitative da porre:

- "I tempi di lavorazione sono stabili o variano molto? Tra il tempo medio
  e il tempo massimo, quanto è la differenza?"
- "Gli arrivi sono prevedibili (cadenza regolare) o a picchi (es. tutti il
  lunedì, fine mese, dopo un rilascio)?"
- "Quando arriva un picco, cosa succede: si genera coda visibile?"
- "Le interruzioni esterne (escalation, urgenze, richieste fuori scope)
  sono rare o frequenti?"

Classifica la variabilità in tre livelli qualitativi:

- **Stabile**: tempi e arrivi prevedibili, pochi picchi, poche interruzioni.
- **Variabile**: scostamenti significativi rispetto alla media, picchi
  riconoscibili ma assorbibili.
- **Molto variabile**: scostamenti grandi, picchi imprevedibili, frequenti
  interruzioni esterne. Probabili code che esplodono fuori controllo.

Alla fine, calcola le metriche aggregate:
- **Throughput time totale** = somma di tutti i tempi (lavorazione + attesa)
- **Processing time totale** = somma solo dei tempi di lavorazione
- **Numero di handoff totali**
- **Numero di tool coinvolti**
- **Numero di livelli di approvazione**
- **Dipendenze esterne**
- **WIP totale** (v2.1): somma dei WIP per step, o WIP del bottleneck come
  proxy del WIP del sistema
- **Bottleneck identificato** (v2.1): step + descrizione
- **Variabilità complessiva** (v2.1): stabile / variabile / molto variabile

Questi numeri servono per:
- Il calcolo DLI (Step 4) — Throughput time, handoff, tool, approvazioni,
  dipendenze
- Il piano d'intervento (Step 5, v2.1) — WIP, bottleneck e variabilità
  orientano la priorità degli interventi

**Output Step 2:**
```
STEP 2 — VALUE STREAM MAP
[Tabella step-by-step con colonne: nome, chi, tool, processing, waiting,
 handoff, decisione, WIP, variabilità]

METRICHE AGGREGATE:
• Throughput time: [X ore/giorni]
• Processing time: [X ore/giorni]
• Handoff: [N]
• Tool: [N]
• Livelli approvazione: [N]
• Dipendenze esterne: [N]

METRICHE DI FISICA DEL FLUSSO (v2.1 — orientano lo Step 5, non entrano nel DLI):
• WIP totale: [valore]
• Bottleneck identificato: [step] — segnali: [coda davanti / tempi morti dopo]
• Variabilità complessiva: [stabile / variabile / molto variabile]
  (valutazione qualitativa)
```

---

## <a name="step-3"></a>Step 3 — Muda Assessment (fonte-aware v2.3)

Per questo step, carica `references/muda-checklist.md` e segui la guida
dettagliata per ciascun muda.

Scoring: 0 = assente, 1 = lieve, 2 = moderato, 3 = grave.
Ogni punteggio deve essere supportato da almeno una evidenza concreta.

**Novità v2.3 — fonte-aware**: dopo aver scorato i 9 muda, mappa i muda
dominanti (score ≥ 2) alle **tre fonti di inefficienza** (DLF v2.4 Sez 8.1).
Le tre fonti sono la lettura causale: spiegano *perché* i muda emergono e
*dove* andare a colpire per attaccarli alla radice.

**Mappa muda → fonte di inefficienza:**

| Fonte di inefficienza | Muda tipicamente generati |
|---|---|
| **1. Lungo throughput time** — l'unità di flusso resta nel sistema più del necessario | Waiting (#2), Inventory (#6) |
| **2. Troppe unità di flusso in processo (WIP alto)** — il sistema gestisce molte cose contemporaneamente | Overprocessing (#1), Inventory (#6), Unused Talent (#9), Perfection Trap (#8) |
| **3. Troppi riavvii/handoff per unità di flusso** — perdita di contesto a ogni passaggio | Transport (#5), Defects (#4), Motion (#7), Overproduction (#3) |

Le tre fonti sono interconnesse — un sistema iperfocalizzato sulla resource
efficiency tende ad averle tutte e tre simultaneamente. Ma di solito *una è
dominante* — quella che genera la maggioranza dei muda gravi osservati.

**Output Step 3 (v2.3):**
```
STEP 3 — MUDA ASSESSMENT (fonte-aware)
• Score 9 muda: [tabella muda → score → evidenze]
• Muda dominanti (score ≥ 2): [elenco]
• Mappa muda → fonte di inefficienza: [tabella]
• Fonte di inefficienza dominante: [Lungo throughput time / WIP alto / Molti riavvii]
• Razionale: [perché questa è dominante — quali muda risalgono ad essa]
```

La fonte dominante orienta lo Step 5: gli interventi prioritari devono
aggredire la fonte, non solo i sintomi (i singoli muda).

---

## <a name="step-4"></a>Step 4 — Calcolo DLI

> **Nota v2.1**: La formula del DLI composito **resta invariata** rispetto
> alla v2.0. Le 4 dimensioni sono Waste Score, Flow Ratio, Complexity Score
> e Value Alignment. Le tre metriche di fisica del flusso raccolte nello
> Step 2 v2.1 (WIP, bottleneck, variabilità) NON entrano nel calcolo del
> DLI — ma orientano il piano d'intervento dello Step 5 e diventano metriche
> di sprint per il Kaizen. Sono complementari, non sostitutive.

### 4 Dimensioni

**1. Waste Score**
- Input: somma dei punteggi dei 9 muda (range 0-27)
- Normalizzazione: (1 - WasteScore/27) × 100
- Risultato: 0 (critico) → 100 (pulito)

**2. Flow Ratio**
- Input: dal Value Stream Map (Step 2)
- Formula: (Processing time / Throughput time) × 100
- Risultato: 0% → 100% (ideale)

**3. Complexity Score**
- Input: dal Value Stream Map (Step 2)
- Formula: (N tool × 1) + (N handoff × 2) + (livelli approvazione × 3) + (dipendenze esterne × 2)
- Benchmark di riferimento:
  - Processo semplice: < 15
  - Processo medio: 15-30
  - Processo complesso: > 30
- Normalizzazione inversa: (1 - Score/Benchmark_max) × 100
  - Benchmark_max: definire con l'utente (default 50 per processo IT standard)
  - Se Score > Benchmark_max, il risultato è 0 (non negativo)

**4. Value Alignment**
- Classifica ogni attività nel Value Stream Map:
  - **Tipo A**: collegata direttamente a outcome di valore per il cliente/utente
  - **Tipo B**: necessaria ma non a valore (compliance, governance, admin)
  - **Tipo C**: non a valore e non necessaria (waste puro)
- Formula: (attività Tipo A / totale attività) × 100
- Le attività Tipo C sono candidati immediati per eliminazione

### <a name="formula"></a>Formula DLI Composito

```
DLI = (Waste Score norm. × 0.30) + (Flow Ratio × 0.30) +
      (Complexity Score norm. inv. × 0.20) + (Value Alignment × 0.20)
```

Range: 0-100.

### <a name="interpretazione"></a>Tabella di Interpretazione

| DLI | Stato | Azione |
|---|---|---|
| 0-30 | **CRITICO** — waste sistemico, flow bloccato | Intervento urgente. Sprint Kaizen su quick win. |
| 31-55 | **IN DIFFICOLTÀ** — waste significativo, flow parziale | Assessment completo dei 9 muda. Piano di remediation. |
| 56-75 | **IN PROGRESSO** — miglioramenti visibili | Kaizen continuo. Focus su FLOW e Value Alignment. |
| 76-100 | **ECCELLENTE** — processo lean | Mantenimento e innovazione. Best practice da condividere. |

**Output Step 4:**
```
STEP 4 — DLI SCORECARD
• Waste Score: [raw]/27 → normalizzato: [X]/100
• Flow Ratio: [X]%
• Complexity Score: [raw] (benchmark: [Y]) → normalizzato: [X]/100
• Value Alignment: [X]% ([N] attività tipo A su [N] totali)

DLI COMPOSITO: ([W]×0.30) + ([F]×0.30) + ([C]×0.20) + ([V]×0.20) = [TOTALE]/100
STATO: [Critico/In difficoltà/In progresso/Eccellente]
AZIONE RACCOMANDATA: [dalla tabella]
```

---

## <a name="step-5"></a>Step 5 — Piano di Intervento

Dai risultati del Muda Assessment e del DLI, identifica i top 3 waste per impatto.

Per ciascun intervento:
1. **Muda target**: quale dei 9 muda aggredisci
2. **Intervento concreto**: cosa fai (in una frase)
3. **Owner**: chi è responsabile
4. **Metrica di successo**: come misuri che ha funzionato
5. **Sprint target**: in quale sprint lo fai
6. **Dimensione DLI impattata**: quale delle 4 dimensioni migliora
7. **Leva fisica del flusso** (v2.1): quale delle tre leve muovi —
   bottleneck, WIP, variabilità (o nessuna, se applicabile)
8. **Done when**: criterio di completamento

Principio "affettare l'elefante": se un intervento richiede > 2 settimane,
va spezzato in sotto-interventi da 2 settimane ciascuno.

### Regola di priorità — Bottleneck → WIP → Variabilità (v2.1)

Quando hai più candidati di intervento a parità di impatto sul DLI,
applica questa regola di priorità derivata dalle Tre Leggi del Flusso:

**1. PRIMO — Aggredisci il bottleneck.** È la leva con il rapporto
impatto/effort più alto. Ottimizzare uno step che NON è il bottleneck non
muove il throughput del processo. Se hai un intervento candidato che
muove il bottleneck (lo elimina, lo allarga, o lo sposta dove pesa meno),
ha priorità su tutti gli altri.

**2. SECONDO — Riduci il WIP.** Per la Legge di Little, ridurre il WIP
accorcia direttamente il throughput time. Cap su quanto può essere "in
corso" contemporaneamente. Pull system invece di push. Limiti su backlog
e progetti concorrenti.

**3. TERZO — Riduci la variabilità.** Standardizzazione del processo,
buffer di capacità che assorbono i picchi, eliminazione di interruzioni
esterne. Effetto a medio termine: rende il sistema prevedibile e abbassa
la sensibilità all'utilizzo.

Gli interventi che non muovono nessuna delle tre leve sono validi (es.
eliminazione di un report inutile riduce muda di Overproduction e migliora
Value Alignment), ma vanno dopo. **Il primo intervento dello sprint deve
muovere una delle tre leve fisiche.**

### Matrice di prioritizzazione (v2.1, bottleneck-aware)

Classifica ogni intervento candidato su 2 assi:
- Impatto sul valore: basso / medio / alto
- Complessità di intervento: bassa / media / alta

Parti SEMPRE dal quadrante alto impatto + bassa complessità (quick win lean).
**Tra interventi nello stesso quadrante**, vince quello che muove la leva
fisica più alta nell'ordine bottleneck → WIP → variabilità.

### Azioni matrice-aware (v2.2 — nuovo)

Oltre alla regola di priorità bottleneck → WIP → variabilità, lo Step 5 v2.2
include un secondo livello: le azioni concrete in funzione della transizione
di quadrante dichiarata in Step 0B. La mappa Da → A è la seguente:

| Transizione | Diagnosi | Azioni concrete |
|---|---|---|
| **Da Deserto a qualunque** | Il Deserto è l'unica posizione mai scelta deliberatamente. Va uscito. | Sempre: cap WIP, attacco al bottleneck, prima standardizzazione. Poi azioni specifiche secondo il target. |
| **Verso Isole** (low-cost) | Scelta legittima quando il cliente accetta il flow basso in cambio del prezzo. La coda è parte del prodotto. | Spinta utilizzo risorsa, accettazione esplicita del flow basso, gestione della coda come capacità prevedibile. Eliminazione comunque dei bisogni indiretti residui. |
| **Verso Oceano** (flow lean) | Scelta quando il cliente paga la velocità. Da Isole verso Oceano è il cambio paradigma più duro: richiede riduzione temporanea dell'utilizzo. | Cap WIP rigoroso, buffer di capacità, attacco al bottleneck e alla variabilità. Comunicare esplicitamente che l'utilizzo si abbasserà — è normale, non è regressione. |
| **Verso Stato Perfetto** | Asintoto. La frontiera curva schiacciata dalla variabilità impedisce di arrivarci pienamente. | Riduzione drastica della variabilità di domanda (smoothing arrivi, pull) e di lavorazione (standardizzazione, automazione delle parti deterministiche). Dichiarare apertamente che è benchmark, non destinazione. |
| **Mantenimento** | Posizione raggiunta in coerenza con la strategia. | Sprint Kaizen di mantenimento, monitoraggio delle metriche di fisica del flusso, codifica come best practice. Attenzione al backsliding sotto pressione di breve termine. |

**Regola di compatibilità (v2.2)**: ogni intervento dello sprint deve essere
coerente con la transizione di quadrante target. Esempi:
- Transizione Isole → Oceano + intervento "saturare ulteriormente il team" = INCOERENTE (peggiora il flow)
- Transizione Isole → Oceano + intervento "cap WIP" = COERENTE (libera flow)
- Transizione Deserto → Isole + intervento "spingere utilizzo" = COERENTE (modello low-cost)

### Dichiarazione della frontiera raggiungibile (v2.2 — nuovo)

Alla luce della variabilità rilevata nel processo (qualitativa), dichiara
esplicitamente la **frontiera raggiungibile** come tetto realistico del DLI
nel quadrante target. Questo serve a:
- Interpretare correttamente il DLI: il numero va letto come % della frontiera,
  non come % dell'ideale teorico
- Calibrare le aspettative del management: lo Stato Perfetto è inaccessibile
  finché la variabilità non scende
- Orientare lo sprint successivo: se lo sprint riduce variabilità, la frontiera
  si alza

Esempio: "Frontiera raggiungibile data variabilità alta: ~70/100. DLI attuale
32 → 46% della frontiera realistica. DLI target post-sprint 56 → 80% della
frontiera realistica."

Gli interventi che non muovono nessuna delle tre leve sono validi (es.
eliminazione di un report inutile riduce muda di Overproduction e migliora
Value Alignment), ma vanno dopo. **Il primo intervento dello sprint deve
muovere una delle tre leve fisiche.**

### Azioni Jidoka-aware (v2.3 — nuovo)

Dopo la matrice-aware, lo Step 5 v2.3 introduce un terzo livello: ogni
intervento dello sprint deve essere coerente con il Pillar 5 (Jidoka digitale).
Concretamente:

**Regola 1 — Visibilità del flusso minima**: ogni sprint deve avere un dashboard
di flow (non di stato) accessibile al team operativo. Se nello Step 0E il gap
dominante è l'assenza di visual management di flow, **il primo intervento
dello sprint è l'introduzione del dashboard di flow** — prima ancora di altri
quick win su muda. Non si può accelerare il flow se non lo si vede mentre
funziona.

**Regola 2 — Anomaly detection con soglie**: ogni sprint dichiara almeno una
soglia di anomaly detection attiva sulle metriche di flow (WIP, lead time,
throughput). Soglie tarate sulla baseline, non sui default del tool.

**Regola 3 — Quality gate built-in**: se lo Step 0E evidenzia quality gate
solo a valle, almeno uno dei 3 interventi dello sprint deve spostare un quality
gate dal "a valle" al "built-in" (es. controllo pre-merge invece di UAT finale).

### Azioni fonte-aware (v2.3 — nuovo)

Lo Step 5 v2.3 incrocia anche la fonte di inefficienza dominante (Step 3) con
i muda target. **Gli interventi prioritari aggrediscono la fonte, non solo i
sintomi.**

| Fonte dominante | Azione strutturale prioritaria |
|---|---|
| Lungo throughput time | Riduzione del lead time complessivo — eliminazione delle attese (waiting), riduzione handoff inutili, parallelizzazione delle attività indipendenti. |
| WIP alto | Cap esplicito su WIP per ogni step. Pull system al posto di push. Stop a nuovi item finché non scende il WIP corrente. |
| Molti riavvii/handoff | Riduzione handoff (collassare step ridondanti). Definition of Done dura tra step (cosa il cliente interno *deve* ricevere). Standardizzazione del passaggio (template, runbook). |

Se lo stesso intervento attacca contemporaneamente la fonte dominante E muove
una leva fisica (bottleneck/WIP/variabilità) E è coerente con la transizione
matrice → priorità assoluta.

**Output Step 5 (v2.3):**
```
STEP 5 — PIANO DI INTERVENTO (matrice-aware v2.2 + Jidoka-aware/fonte-aware v2.3)

INTERVENTO 1 (priorità massima):
• Muda target: [muda]
• Fonte di inefficienza aggredita (v2.3): [Lungo TT / WIP / Riavvii]
• Intervento: [cosa]
• Owner: [chi]
• Metrica di successo: [come misuri]
• Sprint target: [sprint #N]
• Dimensione DLI impattata: [quale]
• Leva fisica del flusso: [bottleneck / WIP / variabilità / nessuna]
• Azione matrice-aware (transizione [X]→[Y]): [tipo azione coerente]
• Componente Jidoka (v2.3): [dashboard di flow introdotto / soglia attivata / quality gate spostato a built-in]
• Done when: [criterio]

INTERVENTO 2: [...stessi campi...]
INTERVENTO 3: [...stessi campi...]

REGOLA APPLICATA: il primo intervento muove [bottleneck/WIP/variabilità].
FONTE DOMINANTE AGGREDITA (v2.3): [quale fonte, da quali interventi].
COERENZA JIDOKA (v2.3): dashboard di flow attivo? Soglie attive? Quality gate built-in attivi? [sì/parziale/no]
COERENZA MATRICE: tutti gli interventi sono coerenti con la transizione [X]→[Y].

FRONTIERA RAGGIUNGIBILE (v2.2):
• Variabilità attuale: [stabile/variabile/molto variabile]
• Frontiera attuale: ~[X]/100 nel quadrante target [Y]
• DLI attuale [Z] = [Z/X*100]% della frontiera realistica
• Frontiera attesa post-sprint: ~[X']/100 (se sprint riduce variabilità)
• DLI target post-sprint [Z'] = [Z'/X'*100]% della frontiera post-sprint
```

**Esempi pratici (mantenuti da v2.1/v2.2, ancora validi v2.3):**

- *Quick win sul bottleneck*: il bottleneck è "approvazione manuale del
  responsabile compliance". Intervento: delegare l'approvazione di
  richieste sotto-soglia. Alta leva, bassa complessità → primo intervento
  dello sprint. **Coerenza matrice (v2.2)**: coerente con transizione
  Isole/Deserto → Oceano.

- *Quick win sul WIP*: il team ha 30 ticket aperti contemporaneamente.
  Intervento: cap a 15 ticket attivi, gli altri vanno in coda esplicita.
  Alta leva, bassa complessità → secondo intervento. **Coerenza matrice
  (v2.2)**: coerente con transizione verso Oceano (riduce utilizzo).

- *Intervento medio sulla variabilità*: gli arrivi sono concentrati il
  lunedì mattina. Intervento: smoothing della richiesta con appuntamenti
  distribuiti. Media leva, media complessità → da pianificare in uno
  sprint successivo. **Coerenza matrice (v2.2)**: ALZA la frontiera
  raggiungibile — rilevante per qualunque transizione verso quadranti
  più alti.

---

## <a name="step-6"></a>Step 6 — Ri-assessment

Alla fine di ogni sprint Kaizen (2 settimane):
1. Ricalcola il DLI con gli stessi criteri della baseline
2. Confronta: DLI pre vs DLI post
3. Per ogni dimensione, documenta il delta
4. **(v2.1)** Documenta anche il delta sulle leve fisiche del flusso:
   il bottleneck si è eliminato, allargato, spostato? Il WIP si è ridotto?
   La variabilità qualitativa è migliorata?
5. **(v2.2)** Documenta il movimento sulla matrice di efficienza:
   - Il quadrante è cambiato? Ci si è avvicinati al target?
   - Il vettore di movimento si è spostato?
   - La frontiera raggiungibile si è alzata (se si è ridotta la variabilità)?
   - Il DLI interpretato come % della frontiera è migliorato?
6. **(v2.2)** Documenta il delta sui bisogni indiretti generati:
   è sceso il "lavoro di trazione"? (Stima qualitativa o quantitativa
   del tempo del team allocato a status update, escalation, dashboard)
7. Lesson learned: cosa ha funzionato, cosa no
8. Decidi il prossimo sprint

**Output Step 6 (v2.2):**
```
STEP 6 — RI-ASSESSMENT — Sprint #[N] (v2.2)

DLI PRE: [X] → DLI POST: [Y] → DELTA: [+/-Z]

DETTAGLIO DIMENSIONI DLI:
• Waste Score: [pre] → [post] (Δ [+/-])
• Flow Ratio: [pre] → [post] (Δ [+/-])
• Complexity Score: [pre] → [post] (Δ [+/-])
• Value Alignment: [pre] → [post] (Δ [+/-])

LEVE FISICHE DEL FLUSSO:
• Bottleneck: era [step X] → ora è [step Y / eliminato / spostato]
• WIP: era [valore] → ora è [valore] (Δ [+/-])
• Variabilità: era [stabile/variabile/molto variabile] → ora è [...]

MATRICE DI EFFICIENZA (v2.2):
• Quadrante pre: [...]
• Quadrante post: [...]
• Vettore di movimento: [da → a]
• Frontiera raggiungibile pre: ~[X]
• Frontiera raggiungibile post: ~[Y] (se variabilità ridotta, frontiera alzata)
• DLI interpretato pre: [Z]% della frontiera pre
• DLI interpretato post: [Z']% della frontiera post

BISOGNI INDIRETTI (v2.2):
• Lavoro di trazione pre: [%]
• Lavoro di trazione post: [%]
• Delta: [+/-]

LESSON LEARNED:
• Cosa ha funzionato: [...]
• Cosa non ha funzionato: [...]
• Cosa cambiamo: [...]
```
