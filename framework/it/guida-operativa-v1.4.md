# Digital Lean Framework — Guida Operativa

**Versione 1.4** · Maggio 2026 · Allineata a DLF v2.4 · Autore: [Alessio Setaro](https://www.linkedin.com/in/alessiosetaro/)

*Meno complessità, più risultati.* — Il manuale che rende il DLF actionable.

DLF — Digital Lean Framework © 2026 Alessio Setaro · [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)

---

# Come usare questa guida

Questa è la Guida Operativa del Digital Lean Framework (DLF). Non è una riscrittura del framework, è il manuale di istruzioni per applicarlo. Se il DLF v2.4 dice COSA fare, questa guida dice COME farlo, passo dopo passo.

## Principio guida

*Se dopo aver letto una sezione della guida, il lettore non sa ESATTAMENTE cosa fare come primo passo**,** la sezione ha fallito.*

## Struttura ricorrente

Ogni sezione operativa segue la stessa struttura in 7 elementi:

| **Elemento** | **Descrizione** |
| --- | --- |
| **COSA FARE** | L'azione concreta da eseguire |
| **COME FARLO** | Istruzioni passo-passo, metodo, sequenza |
| **CON CHI** | Ruoli coinvolti e responsabilità |
| **QUANTO TEMPO** | Stima realistica (non ottimistica) |
| **COSA NE ESCE** | Output atteso con esempio concreto |
| **COME SI MISURA** | Metrica di successo |
| **TEMPLATE** | Checklist o template di supporto |

## Sequenza consigliata

Se è la prima volta che applichi il DLF, segui questa sequenza:

- **Legge Zero (Sezione 1)**: classifica il processo e decidi il percorso

- **Assessment DLI (Sezione 2)**: misura la salute lean del processo, incluse le tre metriche di fisica del flusso e il posizionamento sulla matrice di efficienza

- **Muda Scan (Sezione 3):** identifica gli sprechi specifici e i bisogni indiretti generati

- **Sprint Kaizen (Sezione 4):** struttura gli interventi in sprint da 2 settimane, indicando la leva fisica impattata e il movimento atteso sulla matrice

- **Matrice FLOW (Sezione 5)**: prioritizza gli interventi sul flusso (bottleneck-aware). Nota: la Matrice FLOW di questa sezione è la matrice impatto/complessità di prioritizzazione, NON la Matrice di Efficienza del Pillar 3 (vedi glossario).

Le Sezioni 6 e 7 sono di riferimento: guide rapide per i 4 operational tracks + 1 transversal layer e istruzioni per il Lean Advisor AI.

## Glossario rapido

| **Termine** | **Significato** |
| --- | --- |
| **DLF** | Digital Lean Framework |
| **DLI** | Digital Lean Index — indice composito di salute lean (0-100) |
| **Muda** | Spreco — qualsiasi attività che consuma risorse senza creare valore |
| **Value Stream** | Flusso di valore — la sequenza di attività dal trigger all'output |
| **Kaizen** | Miglioramento continuo a piccoli passi |
| **Flow Ratio** | % del tempo totale che è effettivamente lavoro (non attesa) |
| **Legge Zero (Pillar 1)** | Il processo prima della tecnologia |
| **Catena cliente-fornitore interno (Pillar 2)** | Ogni step del processo è cliente del precedente e fornitore del successivo. L'esigenza del cliente finale (unità di flusso) si propaga lungo tutta la catena |
| **Tre Leggi del Flusso (Pillar 3)** | Le tre leggi fisiche che governano qualsiasi processo: Legge di Little, Legge dei Colli di Bottiglia, Legge dell'Effetto della Variabilità |
| **Matrice di Efficienza (Pillar 3)** | Quadrante strategico flow × resource. Quattro quadranti: Deserto, Isole, Oceano, Stato Perfetto. Frontiera curva schiacciata dalla variabilità |
| **Quadranti della matrice** | Deserto (basso flow, basso resource — da uscire), Isole (basso flow, alto resource — scelta low-cost legittima), Oceano (alto flow, resource moderato — lean classico), Stato Perfetto (asintoto teorico) |
| **Frontiera raggiungibile** | Il tetto realistico di posizionamento nella matrice dato il livello di variabilità qualitativa del processo. Più alta la variabilità, più bassa la frontiera |
| **Bisogni diretti/indiretti (Pillar 4)** | Bisogno diretto: il valore "duro" che l'unità di flusso vuole. Bisogno indiretto: il valore "soft" che nasce mentre attende (informazione, status, escalation). Sintomo di flow basso |
| **Lavoro di trazione** | Il lavoro generato dai bisogni indiretti — non sarebbe necessario se il flow fosse veloce |
| **WIP / Cycle Time / Throughput Time** | Work in Progress (unità in coda + lavorazione), tempo di lavorazione singolo, tempo totale di attraversamento |
| **Bottleneck** | Step del processo con la capacità minore — governa il throughput dell'intero processo |
| **Variabilità qualitativa** | Valutazione qualitativa (stabile/variabile/molto variabile) di quanto i tempi di arrivo e di lavorazione variano |
| **Prossimità al cliente** | Sotto-principio di VALUE: il bisogno reale si comprende solo standoci vicino. Gemba walk applicato al digitale |
| **Tassonomia comunicazione** | Quattro tipi: rituale, strutturata, di servizio (valore), di trazione (muda) |

# 1. Legge Zero — Workflow Operativo

*Non partire mai dalla tecnologia per plasmare il processo. Parti dal processo per scegliere la tecnologia.*

**COSA FARE:** Classificare il processo in uno dei 3 percorsi (A, B, C) e seguire il workflow decisionale di 4 step specifici per quel percorso. Alla fine si produce un Decision Record strutturato.

| **Elemento** | **Dettaglio** |
| --- | --- |
| **CON CHI** | Owner del processo + 1-2 persone che vivono il processo ogni giorno |
| **QUANTO TEMPO** | 45-90 minuti per la prima sessione di classificazione e primi 2 step. 30-60 minuti per gli step successivi. Totale: 2-3 ore distribuite su 1-2 sessioni. |
| **COSA NE ESCE** | Un Decision Record: percorso scelto, evidenze raccolte, decisione motivata, prossimo passo. |
| **COME SI MISURA** | Il processo ha un Decision Record completato prima di qualsiasi scelta tecnologica o metodologica. |

## 1.1 Decision Tree — Quale percorso?

La prima domanda da porre:

*Il processo che vuoi affrontare è già digitalizzato, non ancora digitalizzato, o è un processo prevalentemente umano/organizzativo?*

| **Risposta** | **Percorso** | **Descrizione** |
| --- | --- | --- |
| Non ancora digitalizzato | **Percorso A** | Il processo esiste ma non ha componenti digitali significative. Stai per decidere se e come digitalizzare. |
| Sì, già digitalizzato | **Percorso B** | Il processo è su sistemi digitali ma genera complessità, workaround, sprechi. Serve remediation. |
| Umano / organizzativo | **Percorso C** | Riguarda leadership, formazione, decision-making, cultura. La "tecnologia" è un framework, una metodologia, un tool HR. |
| Un mix | **Follow-up** | Chiedi: "Qual è la parte che dà più problemi?" e classifica quella parte. |

## 1.2 Percorso A — Non hai ancora digitalizzato

4 step in sequenza. Non saltare nessuno step.

### Step A1 — COMPRENDI

**Obiettivo:** capire il problema reale e il processo esistente. Parla con chi lo vive ogni giorno.

- Quali sono i pain point quotidiani delle persone che lo vivono?

- Qual è l'obiettivo del processo? Quale outcome di business serve?

- Quali sono i workaround attualmente in uso?

### Step A2 — OTTIMIZZA il processo (senza tecnologia)

**Obiettivo:** eliminare sprechi, semplificare passaggi, ridurre handoff — a prescindere dalla tecnologia.

- Quali step sono ridondanti o non aggiungono valore?

- Quanti handoff ci sono? Si possono ridurre?

- Quali sono i tempi di attesa? Si possono eliminare?

### Step A3 — SCEGLI la tecnologia

**Obiettivo:** scegliere la tecnologia che serve il processo ottimizzato. Non il contrario.

- Quale tecnologia supporta il processo ottimizzato, senza imporre modifiche?

- Le funzionalità che il vendor mostra servono al processo o lo stravolgono?

- Esiste una soluzione più semplice che copre l'80% del bisogno?

### Step A4 — ADATTA la tecnologia

**Obiettivo:** adattare la tecnologia al processo, mai il processo alla tecnologia.

- Quale customizzazione minima serve per allineare la tecnologia al processo ottimizzato?

- Stai disattivando funzioni che non servono?

- Hai il piano di formazione sul processo (non sul tool)?

## 1.3 Percorso B — Hai già digitalizzato (Remediation)

### Step B1 — MAPPA lo stato attuale

- Come funziona davvero il processo digitalizzato? (Non come dovrebbe funzionare sulla carta)

- Quali sono i workaround che le persone usano?

- Quali parti del sistema sono usate al 100%, e quali a meno del 20%?

### Step B2 — IDENTIFICA il waste della digitalizzazione

- Quali funzionalità sono state aggiunte ma non vengono usate?

- Quanti tool fanno la stessa cosa?

- Dove la digitalizzazione ha creato più handoff invece di ridurli?

- Dove la digitalizzazione ha aumentato la complessità senza valore?

### Step B3 — SEMPLIFICA dentro il sistema

- Quali workflow possono essere accorciati senza buttare via il sistema?

- Quali integrazioni possono essere disattivate?

- Quali approvazioni possono essere automatizzate o eliminate?

### Step B4 — DECIDI cosa tenere/eliminare/riprogettare

- Cosa funziona e va mantenuto?

- Cosa è waste puro e va eliminato?

- Cosa va riprogettato (e merita investimento)?

## 1.4 Percorso C — Processi umani e organizzativi

### Step C1 — COMPRENDI il bisogno organizzativo

- Qual è il bisogno organizzativo reale? Non partire dalla soluzione.

- Quali comportamenti vuoi cambiare? In chi? Perché?

**RED FLAG:** Se qualcuno dice "Vogliamo implementare [piattaforma/framework]": "Perché? Qual è il bisogno sottostante? Potrebbe esserci una soluzione più semplice."

### Step C2 — OSSERVA il processo umano

- Come si prendono le decisioni oggi? Chi decide cosa? Quanto ci vuole?

- Come circolano le informazioni? Meeting, email, chat, passaparola?

- Dove si creano i silos?

### Step C3 — PROGETTA l'intervento

- Dato il bisogno e il processo attuale, quale intervento ha senso?

- Serve uno strumento o basta un cambiamento di processo?

- A volte lo strumento migliore è una conversazione strutturata, non una piattaforma.

### Step C4 — SCEGLI lo strumento (solo se serve)

- L'intervento progettato richiede uno strumento? Se sì, serve il processo o lo definisce?

- Potete partire senza strumento e aggiungere dopo, quando il processo è rodato?

## 1.5 Template: Decision Record

Alla fine di qualsiasi percorso, compila questo template:

| **Campo** | **Contenuto** |
| --- | --- |
| **Data** | [data della decisione] |
| **Processo** | [nome del processo analizzato] |
| **Percorso** | [A / B / C] |
| **Contesto** | [breve descrizione del punto di partenza] |
| **Step percorsi** | [sintesi di ciascuno dei 4 step con output] |
| **Decisione** | [cosa si è deciso e perché] |
| **Red Flag identificati** | [violazioni della Legge Zero intercettate] |
| **Prossimo passo** | [azione concreta con owner e data] |

## 1.6 Red Flag — Segnali di violazione

| **Segnale** | **Violazione** | **Risposta** |
| --- | --- | --- |
| Abbiamo scelto [tool], ora progettiamo il processo | Processo adattato al tool | Stai partendo dalla tecnologia. Torniamo al processo. |
| Il vendor dice che [feature] ci serve | Vendor-driven design | Il vendor vende funzionalità. Tu hai bisogno di risolvere un problema. Qual è? |
| Tutti usano [piattaforma] | Benchmark senza contesto | Il fatto che altri la usino non significa che serva a te. Qual è il TUO processo? |
| Mettiamo l'AI su [processo] | AI washing | Prima: il processo è pulito? L'AI su un processo sporco amplifica il disordine. |
| Aggiorniamo perché è vecchio | Modernizzazione fine a sé stessa | Vecchio non è automaticamente sbagliato. Il processo funziona? Genera waste? |

# 2. Assessment DLI — Guida Completa

L'Assessment DLI è il percorso strutturato in 7 step (da 0 a 6) che misura la salute lean di un processo. Produce una baseline numerica (il DLI composito, scala 0-100) da cui partire e su cui misurare il progresso. Lo Step 0 è esteso da 4 a 5 sotto-step e include lo Step 0B bidimensionale (matrice di efficienza).

**COSA FARE:** Guidare un processo attraverso tutti i 7 step dell'assessment DLI, dalla definizione dell'unità di flusso al calcolo del DLI composito, fino al piano di intervento matrice-aware.

| **Elemento** | **Dettaglio** |
| --- | --- |
| **CON CHI** | Owner del processo, 2-3 operatori che vivono il processo, 1 stakeholder di business. Per lo Step 0B è essenziale la presenza di chi può dichiarare il quadrante target strategico. |
| **QUANTO TEMPO** | Assessment completo: 4-6 ore distribuite su 2-3 sessioni. Step 0-1: 75-105 min (con 0C bisogni e 0D catena interna ). Step 2: 75-105 min. Step 3: 60-90 min. Step 4-5: 60-90 min (esteso con matrice-aware). Step 6: 30 min (a fine sprint). |
| **COSA NE ESCE** | Report DLI completo: baseline, muda assessment, DLI scorecard, metriche di fisica del flusso, posizionamento sulla matrice di efficienza con frontiera raggiungibile, matrice della catena interna, piano di intervento matrice-aware. |
| **COME SI MISURA** | DLI composito calcolato e documentato. Quadrante attuale e target dichiarati. Piano di intervento con owner, metriche, sprint target, leva fisica del flusso impattata, transizione di quadrante. |

## 2.1 Step 0 — Orientamento Strategico

Prima di qualsiasi calcolo, cinque domande fondamentali. Non saltare nessun sotto-step:

- 0A — senza unità di flusso e confini del sistema, il Flow Ratio non ha senso

- 0B — senza posizionamento sulla matrice non sai in che direzione andare

- 0C — senza la lente dei bisogni diretti/indiretti rischi di confondere valore e lavoro di trazione

- 0D — senza la catena cliente-fornitore interno la mappa del valore è descrittiva, non normativa

- 0E — senza visibilità del flusso e quality gate built-in, stai applicando JIT cieco (Pillar 5 — Jidoka digitale)

### 0A — Identificare l'Unità di Flusso e i Confini del Sistema

*Chi o cosa attraversa il processo, e quali sono i confini di ciò che chiami **"**il processo**"**?*

Lo Step 0A in v1.4 ha due output, non uno solo: l'unità di flusso (chi/cosa attraversa) e i confini del sistema (dove inizia e dove finisce il processo che stai analizzando). I confini sono parte della definizione del processo, e nel framework v2.4 vengono trattati come **scelta strategica esplicita**,non come dato di fatto assunto a priori.

**Perché i confini sono una scelta.** Lo stesso processo può essere letto a confini diversi, e ogni scelta produce un throughput time diverso e bisogni indiretti diversi. Esempio IT Service Request:

- **Confini stretti:** dal momento in cui l'utente apre il ticket al momento in cui il ticket è chiuso. Throughput time = es. 24h. Bisogni indiretti = "a che punto è il mio ticket?".

- **Confini medi:** dal momento in cui l'utente *capisce di aver bisogno* (es. quando non riesce ad accedere) al momento in cui *l'accesso è ripristinato e validato in produzione*. Throughput time = es. 48h (include tempo di "cosa devo fare" + validazione). Bisogni indiretti = "come faccio mentre aspetto?" + "è davvero risolto?".

- **Confini ampi:** dalla prima volta che l'utente si è accorto del problema (es. lentezza percepita 2 settimane prima del ticket vero) fino a quando il problema *non si ripresenta nelle 4 settimane successive*. Throughput time = mesi. Bisogni indiretti = workaround, comunicazioni di reassurance, gestione della frustrazione cronica.

Tre processi diversi, tre throughput time diversi, tre piani d'intervento diversi. **La scelta dei confini va dichiarata esplicitamente** prima di procedere oltre. Non c'è una scelta giusta a priori — c'è una scelta coerente con cosa si vuole vedere e cosa si vuole migliorare.

**Livello di astrazione del processo.** Connesso ai confini: lo stesso processo può essere descritto a livelli diversi di astrazione (DLF v2.4, Sez 6.5). Macro = il processo end-to-end come catena di team. Medio = dentro un team, la catena di ruoli. Micro = dentro un ruolo, la catena di attività. La scelta del livello è parte della scelta dei confini, e va dichiarata.

**L'unità di flusso:** L'unità di flusso NON è lo strumento (il ticket, l'alert, il corso). È il valore che attraversa il processo entro i confini scelti.

| **Dominio** | **Unità di flusso corretta** | **Unità SBAGLIATA** |
| --- | --- | --- |
| **Cybersecurity** | Il processo di business da garantire integro | L'alert, l'incidente, il ticket |
| **IT and Digital Service Delivery** | La richiesta dell'utente (il bisogno) | Il ticket IT,la query SQL, il report |
| **Leadership & People** | isogno di competenza o decisione → competenza applicata o decisione presa | Il corso, il CV, il report, il meeting |
| **Digital Transformation Programs** | L'iniziativa di redesign / migrazione end-to-end di un processo di business | Il progetto IT, la feature,il deliverable singolo |
| **AI Adoption** | Il processo con lavoro ripetitivo da assistere | Il modello, il prompt, l'API call |

**Domande da porre per dichiarare unità di flusso E confini:**

- Chi o cosa attraversa il processo? (Unità di flusso)

- Dove dichiariamo che il processo inizia? Il primo trigger osservabile (apertura ticket), il bisogno latente del cliente (quando ha cominciato ad averne bisogno), o un punto intermedio?

- Dove dichiariamo che il processo finisce? Chiusura del ticket, validazione in produzione, conferma del cliente, assenza di problema per N giorni?

- A che livello di astrazione stiamo guardando? Macro (catena team), meso (catena ruoli), micro (catena attività)?

**RED FLAG sui confini:** se l'utente non sa rispondere "dove inizia e dove finisce il processo", non procedere oltre lo Step 0A. La discussione dei confini è essa stessa output di valore, chiarifica cosa il management vuole davvero ottimizzare.

**OUTPUT STEP 0A (v1.4):** Unità di flusso: [cosa] │ Confini dichiarati: [inizio → fine, con razionale] │ Livello di astrazione: [macro / meso / micro]

### 0B — Posizionamento sulla Matrice di Efficienza

Si valuta dove siamo oggi (quadrante attuale) e dove si vuole essere (quadrante target, "ambizione" strategica).

**Output formale:** posizione attuale + target sulla matrice.

**Nota importante v1.4:** il quadrante target è scelta di **strategia operativa**, conseguenza della strategia d'impresa che il framework NON discute (DLF v2.4, Sez 7.5.4 — strategia d'impresa out of scope). Il practitioner non sceglie il quadrante per il management; ne facilita la dichiarazione. Se il management non sa dichiarare il quadrante target, il framework si ferma qui, la discussione è essa stessa output.

**I quattro quadranti:**

| **Quadrante** | **Flow** | **Resource** | **Significato strategico** |
| --- | --- | --- | --- |
| **Deserto** | Basso | Basso | Posizione mai scelta deliberatamente. Universalmente da uscire. |
| **Isole** | Basso | Alto | Modello low-cost: cliente accetta flow basso in cambio del prezzo. Scelta legittima se consapevole. |
| **Oceano** | Alto | Medio/basso | Modello lean classico: valore veloce, buffer di capacità. Scelta per servizi premium e time-sensitive. |
| **Stato Perfetto** | Alto | Alto | Asintoto teorico. Benchmark, non destinazione realistica. |

**Domande da porre per posizionare il processo ATTUALE:**

- Quanto del throughput time è effettivamente lavoro vs attesa? (Flow alto/basso)

- Le risorse del team sono sature al 100% o hanno buffer di capacità? (Resource alto/medio/basso)

- Quando arriva un picco, cosa succede: si accumula coda (resource alto) o si riallocano risorse (resource medio con buffer)?

- Le metriche operative oggi misurano l'utilizzo o la velocità del flusso?

**Domande da porre per dichiarare il quadrante TARGET:**

- Qual è il modello di business del processo? Il cliente paga la velocità o il prezzo?

- Se il cliente paga la velocità → quadrante target = Oceano. Se accetta il flow basso in cambio del prezzo → quadrante target = Isole. Non c'è una scelta giusta a priori — c'è una scelta coerente con il modello di business.

- Se il quadrante attuale è Deserto → il target è qualunque quadrante diverso. Il Deserto va uscito.

**Frontiera raggiungibile:** Una volta dichiarato il target, valutare qualitativamente quale tetto realisticamente puoi raggiungere dato il livello di variabilità che osservi nel processo. Variabilità alta → frontiera bassa: non si raggiunge la parte alta dell'Oceano e lo Stato Perfetto è inaccessibile. Variabilità bassa → frontiera alta: tutto il quadrante target è approcciabile. La frontiera raggiungibile va dichiarata QUI per essere usata nello Step 5 e nel Report DLI.

**RED FLAG:** Se l'utente dichiara come target lo "Stato Perfetto" senza qualificarlo, intervieni: "Lo Stato Perfetto è asintoto teorico, è benchmark, non destinazione. Ridichiariamo il target come Oceano (o Isole, se modello low-cost), e usiamo lo Stato Perfetto come direzione di tensione, non come obiettivo raggiungibile."

### 0C — Identificare bisogni diretti e indiretti

Qual è il bisogno diretto dell'unità di flusso? Quali bisogni indiretti il processo sta generando perché il flow è basso?

Distingue il valore che l'unità di flusso vuole davvero dal "lavoro di trazione" che il processo genera quando funziona male.

**Definizioni operative:**

- **Bisogno diretto:** il valore "duro" che il cliente/utente effettivamente vuole. Per un ticket IT: l'accesso ripristinato. Per un incident di sicurezza: la mitigazione del rischio di business. Per una richiesta di formazione: la competenza applicabile.

- **Bisogno indiretto:** il valore "soft" che nasce mentre l'unità di flusso aspetta o attraversa un processo lento. Informazione, rassicurazione, aggiornamento. Quando il flow è veloce, sparisce. Quando il flow è lento, genera lavoro aggiuntivo: chiamate di sollecito, status update, dashboard di tracking, escalation, riunioni di review backlog.

**L'insight chiave:** i bisogni indiretti non sono valore, sono sintomo di flow basso. Il lavoro che generano è muda, anche se sembra "servizio al cliente".

**Domande da porre:**

- Qual è il bisogno diretto dell'unità di flusso? Cosa vuole davvero ottenere il cliente del processo?

- Mentre il processo è in corso, il cliente contatta qualcuno per chiedere aggiornamenti? Quanto spesso?

- Ci sono dashboard, report di stato, riunioni di review backlog, o comunicazioni di status che esistono solo per gestire l'attesa?

- Ci sono escalation che si attivano quando il processo si dilunga? Quante?

- Se il processo chiudesse in metà del tempo attuale, quale di questi lavori sparirebbe?

L'ultima domanda è la più utile: cristallizza quale lavoro è generato dal flow basso vs quale lavoro è strutturale.

**RED FLAG:** se l'utente dice "ma il customer support è valore per il cliente!", correggi: "Distinzione importante (cfr. tassonomia comunicazione, DLF v2.4 Sez 4.2): rispondere a una richiesta di stato perché il cliente non sa a che punto è il suo ticket è comunicazione di trazione, NON di servizio, è muda generato dal fatto che il processo non gli ha già dato risposta. Se il ticket si chiudesse in 4 ore invece che in 4 giorni, nessuno chiamerebbe per chiedere stato."

### 0D — Catena cliente-fornitore interno

Scomporre il processo nelle sotto-fasi e per ognuna compilare la matrice della catena interna (cliente interno / output consegnato / bisogno indiretto generato). Questo è il Pillar 2 del DLF v2.4 (Sezione 6) operazionalizzato.

**Perché farlo in Step 0D e non in Step 2 (VSM):** lo Step 2 mappa cosa succede (descrittivo); lo Step 0D dichiara come va letto il processo (normativo). La matrice della catena è prerequisito del VSM, non un suo sottoprodotto. Senza questo step il VSM rischia di descrivere bene un processo letto male.

**Procedura operativa:**

- Elencare le sotto-fasi del processo (di solito 4-8 step principali).

- Per ciascuna sotto-fase, identificare il cliente interno (lo step a valle): nome, ruolo, team.

- Per ciascuna sotto-fase, identificare l'output consegnato al cliente interno: dato, documento, decisione, sistema.

- Per ciascuna sotto-fase, identificare il bisogno indiretto generato nel cliente interno: richieste di chiarimento, riconsegne, escalation, duplicazione di lavoro, status update.

- Per ciascuna sotto-fase, applicare il test diagnostico del Pillar 2: "se elimino questo output, il cliente finale se ne accorge?". Se no, l'output è una convenzione interna sopravvissuta alla sua utilità — candidato all'eliminazione.

**Template della matrice catena interna:**

| **Sotto-fase** | **Cliente interno** | **Output consegnato** | **Bisogno indiretto generato** |
| --- | --- | --- | --- |
| [Step 1 — es. Triage Incident] | [Analista L2] | [Ticket classificato + log iniziali] | [Richieste di re-classificazione se severity imprecisa] |
| [Step 2 — es. Analisi L2] | [Specialista risoluzione] | [Diagnosi documentata] | [Domande per chiarimenti se diagnosi superficiale] |
| [Step N...] | [...] | [...] | [...] |

**RED FLAG:** se una sotto-fase non ha un cliente interno chiaramente identificabile, è candidato come waste strutturale (Overprocessing o Inventory). Se nessuno a valle riceve davvero qualcosa di utile, perché esiste?

### 0E — Visibilità del Flusso (v1.4 — Pillar 5 Jidoka digitale)

*Il processo è osservabile mentre funziona? Esistono soglie esplicite di anomaly detection? Esiste un potere/dovere di **"**stop the line**"**? I quality gate sono built-in o a valle?*

Lo Step 0E nasce in v1.4 dall'introduzione del Pillar 5 nel DLF v2.4 (Sezione 9 — Jidoka digitale). Il principio è: un processo che si vuole migliorare deve essere visibile mentre funziona, non solo a posteriori. Se non sai cosa sta facendo il flow adesso, ogni intervento è cieco, è "JIT senza Jidoka",una delle cause principali per cui le iniziative lean falliscono.

**Le quattro domande di valutazione Jidoka digitale:**

| **Dispositivo Jidoka** | **Domanda da porre** | **Risposta atteso** |
| --- | --- | --- |
| **Visual management** | Esistono dashboard di flow real-time (lead time corrente vs baseline, WIP per step, throughput dei bottleneck)? O solo dashboard di stato ("quanti ticket aperti")? | Sì = flow / Parziale / Solo stato / No dashboard |
| **Andon / Anomaly detection** | Esistono soglie esplicite su WIP, lead time, SLA con notifica automatica quando vengono superate? O le anomalie emergono solo quando esplodono? | Soglie esplicite / Soglie ma manuali / No soglie |
| **Stop the line** | Il team ha potere/dovere dichiarato di fermare il delivery se la qualità non regge? E nei fatti viene esercitato? | Dichiarato + esercitato / Dichiarato ma mai esercitato / Non esiste |
| **Built-in quality** | I quality gate sono al passo (pre-merge, in pipeline, pre-deploy) o a fine processo (UAT finale, audit a posteriori)? | Built-in / Misti / A valle |

**Domande di approfondimento:**

- Se il flow devia in modo significativo *adesso*, qualcuno lo saprebbe nei prossimi 5 minuti? 30 minuti? Domani? La settimana prossima?

- I dashboard esistenti sono alimentati per il team operativo (azione) o per il management (status)? Test: se il dashboard sparisce, il team operativo perde la capacità di intervento?

- Quando un'anomalia viene rilevata, c'è un'azione automatica/predefinita o si avvia una catena di email e riunioni?

- Il framework di sicurezza (cybersecurity), il QA, la compliance — sono integrati nel processo o sono check di fine corsa?

**RED FLAG critico:** se la risposta a Visual Management è "abbiamo dashboard di stato" e nient'altro, dichiara il gap esplicitamente: "Avete visibilità di status, non di flow. Per il framework v2.4 questo è gap del Pillar 5, andrà aggredito tra i primi tre interventi dello Step 5."

**RED FLAG sull'alert overload:** se la risposta a Anomaly detection è "abbiamo decine di alert al giorno", chiedi quante sono *effettivamente azionate*. Se la risposta è "il 5-10%", non è anomaly detection, è rumore. Le soglie vanno tarate sulla baseline reale del processo, non sui default del tool.

**RED FLAG sullo stop-the-line teorico:** se il team dichiara di avere "potere di bloccare il delivery" ma nei fatti non lo esercita mai sotto la pressione del business, è peggio dell'assenza del principio, crea l'illusione che il dispositivo esista. Dichiarare esplicitamente la deviazione tra teoria e pratica.

**OUTPUT STEP 0E (v1.4):** Visual management: [livello] │ Anomaly detection: [livello] │ Stop the line: [livello] │ Built-in quality: [livello] │ Gap Jidoka dominante: [quale dei quattro è più critico]

**OUTPUT STEP 0 (v1.4 — completo):** Processo: [nome] │ Unità di flusso: [cosa] │ Confini dichiarati: [inizio → fine] │ Livello di astrazione: [macro/meso/micro] │ Quadrante attuale: [Deserto/Isole/Oceano/Stato Perfetto] │ Quadrante target: [...] │ Frontiera raggiungibile data variabilità: [qualitativa] │ Bisogno diretto: [una frase] │ Bisogni indiretti generati: [elenco] │ Lavoro di trazione stimato: [% tempo del team] │ Matrice catena interna: [N sotto-fasi documentate] │ Visibilità del flusso (Jidoka): [4 livelli + gap dominante]

## 2.2 Step 1 — Selezione del Processo

**Domande da porre:**

- Qual è il nome del processo?

- Dove inizia esattamente? (trigger di ingresso)

- Dove finisce esattamente? (output finale / condizione di completamento)

- Chi è l'owner del processo?

- Chi sono gli stakeholder principali?

- Quante persone/team sono coinvolti?

**OUTPUT STEP 1:** Processo: [nome] │ Inizio: [trigger] │ Fine: [output] │ Owner: [chi] │ Stakeholder: [chi] │ Team coinvolti: [N, quali]

## 2.3 Step 2 — Digital Value Stream Map

Mappa il processo end-to-end. Non serve un tool visuale: basta una lista strutturata. Lo Step 2 raccoglie tre dati aggiuntivi di fisica del flusso: WIP per step (Legge di Little), bottleneck identificato (Legge dei Colli di Bottiglia), variabilità qualitativa (Legge dell'Effetto della Variabilità).

**Relazione con lo Step 0D :** lo Step 0D ha già stabilito la matrice della catena interna (cliente interno / output / bisogno indiretto per sotto-fase). Lo Step 2 ne è la naturale estensione descrittiva: per ciascuna sotto-fase aggiunge tempi, WIP, variabilità. Non si rifà da capo — si arricchisce quello già fatto in 0D.

Per ogni STEP del processo, raccogli:

| **Dato da raccogliere** | **Esempio** |
| --- | --- |
| Nome dello step | Triage dell'incidente |
| Chi lo esegue | Analista SOC L1 |
| Tool utilizzato | SIEM + ITSM |
| Tempo di lavorazione (processing time) | 15 minuti |
| Tempo di attesa (waiting time) | 2 ore (attesa escalation) |
| Handoff | Passa a SOC L2 via ticket |
| Punto di decisione? | Sì: se severity > medium → escalation |
| **WIP medio** | 15 ticket in coda + 3 in lavorazione = 18 |
| **Variabilità** | Stabile / variabile / molto variabile |
| **Cliente interno (da 0D)** | Analista L2 |
| **Bisogno indiretto generato (da 0D)** | Re-classificazione se severity imprecisa |

### Identificazione del bottleneck

Una volta mappati tutti gli step, identifica il bottleneck con due segnali osservazionali:

- Dove si forma coda? Lo step con il WIP più alto, o lo step di fronte al quale si accumula lavoro in attesa, è candidato bottleneck.

- Dove ci sono tempi morti a valle? Lo step dopo il quale i sotto-processi aspettano è confermato come bottleneck.

Se difficile identificarlo, chiedi:

- Se un'unità di flusso entrasse adesso, in quale step rimarrebbe in coda più a lungo?

- Se quello step lavorasse il doppio più veloce, il throughput raddoppierebbe? (se sì, è il bottleneck)

**Attenzione:** il bottleneck può essere una persona (decision authority unica), un livello di approvazione, un rito (board mensile), un sistema (deployment window), un vincolo esterno (SLA fornitore). Non sempre è uno step di "lavoro" classico.

### Valutazione della variabilità

**IMPORTANTE — Natura della valutazione:** nel DLF la variabilità è valutata qualitativamente, NON quantitativamente. Per una misurazione rigorosa servirebbero dati di distribuzione su arrivi e tempi (analisi statistica, coefficiente di variazione). Questo è fuori dallo scope di un assessment DLI standard. La valutazione qualitativa è sufficiente a identificare la presenza del problema e orientare gli interventi e a stimare qualitativamente la frontiera raggiungibile sulla matrice .

Domande qualitative:

- I tempi di lavorazione sono stabili o variano molto?

- Gli arrivi sono prevedibili (cadenza regolare) o a picchi?

- Quando arriva un picco, si genera coda visibile?

- Le interruzioni esterne (escalation, urgenze, richieste fuori scope) sono rare o frequenti?

Classifica in tre livelli qualitativi:

- **Stabile:** tempi e arrivi prevedibili, pochi picchi, poche interruzioni. → Frontiera matrice ALTA (Stato Perfetto approcciabile)

- **Variabile:** scostamenti significativi, picchi riconoscibili ma assorbibili. → Frontiera matrice MEDIA (parte alta del quadrante target raggiungibile)

- **Molto variabile:** scostamenti grandi, picchi imprevedibili, interruzioni frequenti. → Frontiera matrice BASSA (solo parte bassa del quadrante target accessibile)

Alla fine, calcola le metriche aggregate: Throughput time totale, Processing time totale, Numero di handoff totali, Numero di tool coinvolti, Numero di livelli di approvazione, Dipendenze esterne, WIP totale.

**OUTPUT STEP 2:** Value Stream Map completa per step + metriche aggregate + WIP totale + bottleneck identificato + variabilità qualitativa complessiva + frontiera raggiungibile data variabilità (aggiornata rispetto a quanto dichiarato in 0B).

## 2.4 Step 3 — Muda Assessment

Vedi Sezione 3 di questa guida per la checklist dettagliata. Per ogni muda: punteggio 0-3, evidenza concreta, metrica quantitativa (se possibile), bisogno indiretto associato annotato.

**OUTPUT STEP 3:** Muda Assessment Report con Waste Score totale (/27) e top 3 muda per impatto con bisogno indiretto associato.

## 2.5 Step 4 — Calcolo DLI

Applica la formula del DLI composito. La formula resta INVARIATA, cambia l'interpretazione del numero (vedi Step 5).

DLI = (Waste Score normalizzato × 0.30) + (Flow Ratio × 0.30) + (Complexity Score normalizzato inverso × 0.20) + (Value Alignment × 0.20)

Dettagli di calcolo per ciascuna dimensione: vedi DLF v2.4 Sezioni 11.1, 11.2, 11.4.

## 2.6 Step 5 — Piano di Intervento

Il piano di intervento estende la regola di priorità v1.1 (bottleneck → WIP → variabilità) con un livello strategico in più: le azioni matrice-aware in funzione della transizione di quadrante.

**Struttura del piano d'intervento** 

Il piano produce quattro output strutturati:

- **1. Le 3 azioni prioritarie sui 9 muda** (Step 5 v1.1, mantenuto).

- **2. La leva fisica del flusso impattata dalla prima azione** (Step 5 v1.1, mantenuto): bottleneck → WIP → variabilità in ordine di priorità.

- **3. Le azioni matrice-aware in funzione della transizione (Step 5 , nuovo):** data la coppia (quadrante attuale → quadrante target) dichiarata in 0B, le azioni specifiche secondo la tabella sotto.

- **4. La dichiarazione della frontiera raggiungibile** come tetto realistico del DLI nel quadrante target (qualitativa, basata sulla variabilità rilevata).

### Tabella delle azioni matrice-aware

| **Transizione** | **Diagnosi** | **Azioni** |
| --- | --- | --- |
| **Da Deserto a qualunque quadrante** | Il Deserto è l'unica posizione mai scelta deliberatamente. Va uscito. | Sempre: cap WIP, attacco al bottleneck, prima standardizzazione. Poi azioni specifiche secondo il target. |
| **Verso Isole (modello low-cost)** | Scelta legittima quando il cliente accetta il flow basso in cambio del prezzo. La coda è parte del prodotto. | Spinta utilizzo risorsa, accettazione esplicita del flow basso, gestione della coda come capacità prevedibile. Eliminazione comunque dei bisogni indiretti residui. |
| **Verso Oceano (modello lean classico)** | Da Isole a Oceano è il cambio paradigma più duro: richiede riduzione temporanea dell'utilizzo per liberare flow. | Cap WIP rigoroso, buffer di capacità, attacco al bottleneck, attacco alla variabilità. Comunicazione esplicita che l'utilizzo si abbasserà — è normale, non regressione. |
| **Verso Stato Perfetto** | Asintoto. La frontiera curva schiacciata dalla variabilità impedisce di arrivarci pienamente. | Riduzione drastica della variabilità di domanda (smoothing arrivi, pull) e di lavorazione (standardizzazione, automazione delle parti deterministiche). Dichiarare apertamente che è benchmark, non destinazione. |
| **Mantenimento (target già raggiunto)** | Posizione raggiunta in coerenza con la strategia. | Sprint Kaizen di mantenimento, monitoraggio metriche di fisica del flusso, codifica come best practice. Attenzione al backsliding sotto pressione di breve termine sui costi. |

### Compilazione del Report DLI

Il Report DLI contiene un layer di posizionamento strategico aggiuntivo:

| **Elemento del Report DLI** | **Cosa contiene** |
| --- | --- |
| **DLI composito** | Numero 0-100 calcolato con la formula invariata. |
| **Quadrante attuale e target** | Da Step 0B esteso. |
| **Vettore di movimento** | Da quadrante attuale a quadrante target. |
| **Frontiera raggiungibile** | Tetto realistico dato il livello di variabilità qualitativa rilevato in Step 2. |
| **DLI interpretato** | DLI letto come % della frontiera raggiungibile, non % dell'ideale teorico. Es: "DLI 56 su frontiera 75 → 75% della frontiera realistica". |
| **3 metriche fisica flusso** | WIP totale, bottleneck identificato, variabilità complessiva. |
| **Top 3 muda con bisogno indiretto** | Da Step 3 muda assessment. |
| **Piano d'intervento** | 3 azioni prioritarie + leva fisica + transizione matrice + frontiera dichiarata. |

**OUTPUT STEP 5 :** Report DLI completo con baseline numerica, posizionamento matrice, frontiera raggiungibile, piano d'intervento matrice-aware pronto per essere portato in Sprint Kaizen.

## 2.7 Step 6 — Ri-assessment ( — con tracking matrice)

Ad ogni fine sprint, ricalcola il DLI con gli stessi criteri e documenta il delta. il ri-assessment traccia anche:

- Il movimento sulla matrice di efficienza (cambiato il quadrante? Ci si è avvicinati al target? Si è spostato il vettore di movimento?)

- Il delta sulla frontiera raggiungibile (la riduzione di variabilità ha alzato la frontiera?)

- Il delta sulle metriche di fisica del flusso (bottleneck eliminato/spostato? WIP ridotto? Variabilità qualitativa migliorata?)

- Il delta sui bisogni indiretti generati (è sceso il "lavoro di trazione"?)

**OUTPUT STEP 6:** Delta Report tra Sprint N-1 e Sprint N che include tutte le dimensioni sopra. Decisione: stiamo andando nella direzione del target? Cambiamo strategia? Confermiamo la traiettoria?

## 2.8 Esempio: IT Service Request (v1.4 — con confini, matrice, catena interna e Jidoka)

Per concretezza, ecco un assessment DLI completo su un processo reale. L'esempio v1.4 estende quello con Step 0A (confini espliciti) e Step 0E (visibilità del flusso — Pillar 5 Jidoka digitale).

### Step 0 — Orientamento Strategico

**0A — Unità di flusso, confini, livello di astrazione (v1.4):**

- **Unità di flusso:** la richiesta dell'utente (bisogno di accesso/strumento/risoluzione). NON il ticket.

- **Confini dichiarati:** dal momento in cui l'utente apre il ticket (trigger osservabile) al momento in cui la soluzione è validata in produzione *e* il problema non si ripresenta nelle 48h successive. Razionale: confini più stretti (solo ticket aperto → chiuso) sotto-stimerebbero il muda di trazione che si genera dopo la chiusura formale ma prima della stabilizzazione effettiva.

- **Livello di astrazione:** macro (catena di team: User → Tier 1 → Manager → Tier 2 → Validazione). Se l'assessment trovasse il bottleneck dentro Tier 2, si zoomerebbe a meso (ruoli interni a Tier 2).

**0B — Posizionamento sulla matrice :**

- **Quadrante attuale:** Isole, flow basso (throughput time 48h con solo 1.2h di lavoro effettivo), resource alto (team Tier 1 sempre occupato a gestire ticket E richieste di stato).

- **Quadrante target:** Oceano, il management dichiara che il cliente IT interno paga la velocità (è un processo che impatta produttività aziendale). Modello di business compatibile con Oceano. *Nota strategica: scelta di strategia operativa coerente con la strategia d'impresa del business core; la strategia d'impresa non è discussa qui.*

- **Vettore:** Isole → Oceano (transizione classica più difficile).

- **Variabilità rilevata:** molto variabile (disponibilità manager approvazioni a picchi, urgenze frequenti).

- **Frontiera raggiungibile:** qualitativamente ~70/100, la variabilità alta impedisce di andare oltre la parte bassa dell'Oceano fino a quando non si riduce la variabilità.

**0C — Bisogni:**

- **Bisogno diretto:** accesso/strumento/risoluzione ottenuti.

- **Bisogni indiretti generati:** chiamate al service desk per chiedere "a che punto è il mio ticket?", email di sollecito ai team di II livello, riunione settimanale di review backlog (1.5h × 4 persone), dashboard di stato ticket con aggiornamento manuale, escalation a management quando il ticket supera 5 giorni.

- **Lavoro di trazione stimato:** ~25% del tempo del team Tier 1 dedicato a rispondere a richieste di stato, non a risolvere ticket.

- **Tre fonti di inefficienza dominanti (v1.4):** lungo throughput time (48h vs 1.2h di lavoro effettivo) è la dominante; WIP alto e numerosi handoff (4 livelli) sono concorrenti.

**0D — Catena cliente-fornitore interno :**

| **Sotto-fase** | **Cliente interno** | **Output consegnato** | **Bisogno indiretto generato** |
| --- | --- | --- | --- |
| 1. Apertura ticket | Triage Tier 1 | Ticket con dettagli del problema | Richieste di chiarimento se descrizione vaga |
| 2. Triage Tier 1 | Manager (se serve approvazione) o Tier 2 | Ticket classificato + priorità + routing | Re-classificazione se severity imprecisa |
| 3. Approvazione manager | Specialista Tier 2 | Sblocco autorizzativo | Solleciti su approvazioni in ritardo |
| 4. Esecuzione Tier 2 | Utente (per validazione) | Soluzione implementata | Email di update durante l'esecuzione |
| 5. Validazione utente | Tier 1 (per chiusura) | Conferma di soluzione efficace | Re-apertura ticket se validazione superficiale |
| 6. Chiusura | Sistema reporting | Ticket chiuso e archiviato | — |

**0E — Visibilità del flusso (v1.4 — Pillar 5):**

| **Dispositivo Jidoka** | **Stato attuale** | **Gap** |
| --- | --- | --- |
| Visual management | Dashboard di stato presenti (ticket aperti, ticket per analista, ticket overdue). Nessuna dashboard di flow (lead time corrente vs baseline, WIP per step, throughput dei bottleneck). | **Gap dominante** — il team opera senza visibilità del flow. |
| Anomaly detection | Soglia esistente: alert quando ticket > 5gg supera SLA. Nessuna soglia su WIP, lead time medio, throughput. | Soglie parziali e tarate solo su SLA, non sulla fisica del flow. |
| Stop the line | Non dichiarato. Sotto pressione, i ticket vengono "passati avanti" anche se la qualità del triage è scarsa. | Non esiste come dispositivo. |
| Built-in quality | Quality gate solo al validation finale (Step 5). Nessun controllo built-in nei passaggi intermedi (triage, approvazione, esecuzione). | Misti — controllo solo a valle. |

**Gap Jidoka dominante:** assenza di visual management di flow. Da aggredire come uno dei primi interventi nello Step 5 (vedi sotto).

### Step 2 — Value Stream Map

| **Step** | **Chi** | **Processing** | **Waiting** | **WIP** | **Variabilità** |
| --- | --- | --- | --- | --- | --- |
| 1. Apertura ticket | Utente / portale | 5 min | 0 | n/a | stabile |
| 2. Triage Tier 1 | Analista Tier 1 | 15 min | 2 ore | 15 | variabile |
| **3. Approvazione (se serve)** | Manager | 5 min | **18 ore** | **8** | **molto variabile** |
| 4. Esecuzione Tier 2 | Specialista | 30 min | 12 ore | 12 | variabile |
| 5. Validazione utente | Utente | 10 min | 6 ore | 5 | molto variabile |
| 6. Chiusura | Tier 1 | 5 min | 1 ora | 3 | stabile |

**Metriche aggregate:** Throughput time 48 ore, Processing time ~1.2 ore, 6 tool, 4 handoff, 3 livelli approvazione, 2 dipendenze esterne. 20 attività totali: 8 tipo A, 7 tipo B, 5 tipo C. Waste Score: 14/27.

**Metriche di fisica del flusso:** WIP totale ~43, bottleneck Step 3 (Approvazione manager), variabilità complessiva variabile/molto variabile.

### Step 4 — Calcolo DLI

| **Dimensione** | **Calcolo** | **Risultato** |
| --- | --- | --- |
| **Waste Score** | (1 - 14/27) × 100 | 48 |
| **Flow Ratio** | (1.2/48) × 100 | 2.5% |
| **Complexity Score** | (6×1)+(4×2)+(3×3)+(2×2) = 27 → (1-27/50)×100 | 46 |
| **Value Alignment** | 8/20 × 100 | 40% |

**DLI COMPOSITO** = (48 × 0.30) + (2.5 × 0.30) + (46 × 0.20) + (40 × 0.20) = 14.4 + 0.75 + 9.2 + 8.0 = **32.4** → Stato: **IN DIFFICOLTÀ**

**DLI interpretato :** 32.4 su frontiera raggiungibile ~70 → siamo al 46% della frontiera realistica. Non al 32% dell'ideale teorico. Lo spazio di miglioramento c'è, ma il tetto è 70 finché non riduciamo la variabilità.

### Step 5 — Piano d'intervento ( — matrice-aware)

Applicando la regola di priorità (bottleneck → WIP → variabilità) e le azioni della transizione Isole → Oceano (cap WIP rigoroso, buffer capacità, attacco bottleneck e variabilità, comunicazione esplicita sulla riduzione utilizzo):

**Intervento 1 — Aggredisce il bottleneck (priorità massima):**

- Muda target: Waiting (#2) + Overprocessing (#1) sull'approvazione

- Intervento: delegare l'approvazione di ticket sotto-soglia direttamente al Tier 1, mantenendo solo i ticket ad alto rischio nella catena manager

- Leva fisica: bottleneck (Step 3 eliminato/ridotto)

- Azione matrice-aware (Isole → Oceano): cap WIP rigoroso + attacco al bottleneck — coerente con la transizione.

- Owner: IT Service Manager — Metrica: % ticket che attraversano Step 3 → da 80% a 20%

**Intervento 2 — Aggredisce il WIP:**

- Muda target: Inventory (#6), backlog gonfio

- Intervento: WIP cap a 10 ticket per analista Tier 1

- Leva fisica: WIP

- Azione matrice-aware (Isole → Oceano): riduzione utilizzo temporanea per liberare flow, da comunicare esplicitamente al team come parte del cambio di paradigma.

- Owner: IT Service Manager, Metrica: WIP medio per analista da ~5 a ~3

**Intervento 3 — Aggredisce la variabilità:**

- Muda target: Defects (#4) e Waiting (#2) generati dalla variabilità di disponibilità del manager

- Intervento: standardizzare le finestre di approvazione (2 slot/giorno: 10:00 e 15:00) con backup automatico

- Leva fisica: variabilità (riduzione qualitativa)

- Azione matrice-aware: la riduzione della variabilità ALZA la frontiera raggiungibile. Da ~70 dopo l'intervento si può ragionevolmente stimare ~80.

- Owner: IT Service Manager + Manager approvazioni — Metrica: % approvazioni entro 24h (da molto variabile a variabile)

**Bisogni indiretti aggrediti:** tutti tre gli interventi puntano a ridurre il throughput time → il "lavoro di trazione" del 25% del team Tier 1 dovrebbe ridursi sostanzialmente. Stima delta: -10-15% di tempo dedicato a status update.

### Dopo 3 Sprint Kaizen — stima realistica

| **Dimensione DLI** | **Prima** | **Dopo** | **Delta** |
| --- | --- | --- | --- |
| Waste Score normalizzato | 48 | 70 | +22 |
| Flow Ratio | 2.5% | 35% | +32.5 |
| Complexity Score normalizzato | 46 | 64 | +18 |
| Value Alignment | 40% | 60% | +20 |
| **DLI COMPOSITO** | **32.4** | **56.3** | **+23.9** |

**Posizionamento matrice :**

- **Quadrante:** movimento da Isole alla parte bassa dell'Oceano (resource sceso, flow significativamente salito).

- **Frontiera raggiungibile aggiornata:** qualitativamente alzata da ~70 a ~80 grazie a riduzione variabilità.

- **DLI interpretato:** 56.3 su frontiera 80 → 70% della frontiera realistica. Spazio ulteriore di miglioramento c'è, ma siamo già nel quadrante target.

**Metriche di fisica del flusso:**

| **Metrica** | **Prima** | **Dopo** | **Note** |
| --- | --- | --- | --- |
| WIP totale | ~43 | ~22 | -49% grazie a WIP cap + bottleneck rimosso |
| Bottleneck | Step 3 (approvazione) | Spostato su Step 4 (Tier 2) | Atteso: il bottleneck si sposta sempre |
| Variabilità | Variabile / molto variabile | Variabile | Riduzione qualitativa |
| **Lavoro di trazione (% tempo Tier 1)** | ~25% | ~12% | -13 punti — bisogni indiretti ridotti |

# 3. I 9 Muda Digitali — Checklist Operativa

**COSA FARE:** Per ciascuno dei 9 muda: porre le domande diagnostiche, raccogliere evidenze, assegnare punteggio 0-3, identificare metriche quantitative, annotare il bisogno indiretto associato. Alla fine: Waste Score totale e top 3 muda per impatto.

| **Elemento** | **Dettaglio** |
| --- | --- |
| **CON CHI** | Owner del processo + 2-3 operatori. |
| **QUANTO TEMPO** | 60-90 minuti per tutti i 9 muda. |
| **COME SI MISURA** | Ogni punteggio > 0 ha almeno un'evidenza concreta. Almeno 1 metrica quantitativa per muda. Bisogno indiretto annotato. |

## 3.1 Scoring

| **Punteggio** | **Significato** | **Criterio** |
| --- | --- | --- |
| **0** | Assente | Nessuna evidenza di questo spreco |
| **1** | Lieve | Presente ma marginale, impatto limitato |
| **2** | Moderato | Presente e visibile, impatto significativo |
| **3** | Grave | Sistemico, impatto pesante su flow e valore |

## 3.2 I 9 muda con annotazione bisogno indiretto

| **#** | **Muda** | **Bisogno indiretto associato** | **Domande chiave** |
| --- | --- | --- | --- |
| 1 | OVERPROCESSING | **Sì** | Step a valore / totali? Tool usati al 100%? Documentazione necessaria? |
| 2 | WAITING | **Sì — principale generatore.** | Lead time vs processing? Sollecito ricorrente? Status update richiesti? |
| 3 | OVERPRODUCTION | Indirettamente | Report con 0 views? Meeting senza decisioni? |
| 4 | DEFECTS | **Sì** | Tasso di rework? Errori ricorrenti? Comunicazioni di scuse? |
| 5 | MOTION | No (tipicamente esterno) | > 5 tool aperti? > 30% tempo in meeting? |
| 6 | INVENTORY | Indirettamente | Licenze attive vs pagate? Backlog > 6 mesi? |
| 7 | TRANSPORT | **Sì** | N handoff? Info duplicata tra sistemi? |
| 8 | UNUSED TALENT | No tipicamente | % senior su task operativi? Idee proposte? |
| 9 | PERFECTION TRAP | **Sì** | Rilasci/90gg? Time-to-user > 90gg? |

**Nota di lettura:** i muda con bisogno indiretto hanno priorità di intervento perché eliminandoli si elimina anche il lavoro di trazione (status update, escalation, dashboard di tracking). Doppio dividendo.

Per il dettaglio diagnostico di ciascun muda (definizione, domande, segnali, metriche quantitative), vedi muda-checklist nelle reference del Lean Advisor.

## 3.3 Template Output — Muda Assessment Report

| **#** | **Muda** | **Score** | **Evidenze** | **Metrica** | **Bisogno indiretto** |
| --- | --- | --- | --- | --- | --- |
| 1 | OVERPROCESSING | [0-3] | [evidenza] | [misura] | Sì |
| 2 | WAITING | [0-3] | [evidenza] | [misura] | Sì (principale) |
| 3 | OVERPRODUCTION | [0-3] | [evidenza] | [misura] | Indirettamente |
| 4 | DEFECTS | [0-3] | [evidenza] | [misura] | Sì |
| 5 | MOTION | [0-3] | [evidenza] | [misura] | No |
| 6 | INVENTORY | [0-3] | [evidenza] | [misura] | Indirettamente |
| 7 | TRANSPORT | [0-3] | [evidenza] | [misura] | Sì |
| 8 | UNUSED TALENT | [0-3] | [evidenza] | [misura] | No |
| 9 | PERFECTION TRAP | [0-3] | [evidenza] | [misura] | Sì |

**WASTE SCORE TOTALE:** [somma] / 27

**TOP 3 MUDA PER IMPATTO:** [muda, score, dimensione DLI impattata, bisogno indiretto sì/no]

# 4. Sprint Kaizen — Template e Rituali

*Il miglioramento non è un progetto — è un'abitudine. 26 sprint/anno battono 2 progetti da 6 mesi.*

**COSA FARE:** Strutturare il miglioramento continuo in sprint di 2 settimane con 3 rituali: Sprint Planning (1h), Monday Stand-up (15 min), Sprint Review + Retrospettiva (1h).

| **Elemento** | **Dettaglio** |
| --- | --- |
| **CON CHI** | Team operativo (3-7 persone), owner del processo, 1 stakeholder per la review. |
| **QUANTO TEMPO** | Planning: 1h (giorno 1). Stand-up: 15 min (ogni lunedì). Review + Retro: 1h (giorno 10). |
| **COME SI MISURA** | Ogni sprint produce un delta DLI documentato + delta sulle leve fisiche del flusso + eventuale delta di posizione sulla matrice di efficienza. Ogni retro produce almeno 1 cambiamento. |

## 4.1 6 Principi dello Sprint Kaizen

- **Affettare l'elefante:** nessun intervento > 2 settimane. Se è più grande, va spezzato.

- **Misurare prima di partire:** metriche definite PRIMA dello sprint, non dopo.

- **Owner singolo:** ogni intervento ha UN owner (persona, non team).

- **Collegamento al DLI:** ogni sprint dichiara quale dimensione DLI impatta.

- **Leva fisica e matrice dichiarate :** ogni sprint dichiara quale delle tre leve fisiche aggredisce (bottleneck / WIP / variabilità) e quale movimento sulla matrice di efficienza intende produrre (anche solo "mantenimento posizione attuale").

- **Ritmo, non eroismo:** la potenza è la cadenza costante.

## 4.2 Sprint Planning (1h — Giorno 1)

### Obiettivo dello sprint

Chiedi: "Cosa vuoi ottenere in queste 2 settimane? Dillo in una frase."

Se la frase è vaga, sfida: "Migliorare cosa? Quale muda aggredisci? Quale metrica muovi? Quale leva fisica del flusso muovi? Quale movimento sulla matrice di efficienza produci ?"

### Interventi concreti (1-3 max)

Per ciascun intervento:

- Cosa fai (descrizione operativa)

- Chi è l'owner

- Done when (criterio di completamento)

- Metrica di successo (numerica, non opinione)

- Quale dimensione DLI muove

- Quale leva fisica del flusso aggredisce (bottleneck / WIP / variabilità)

- Quale movimento sulla matrice di efficienza produce

## 4.3 Monday Stand-up (15 min)

Ogni lunedì mattina:

- Cosa è stato fatto la settimana scorsa

- Cosa si farà questa settimana

- Blocchi e dipendenze

- Aggiornamento rapido delle metriche

## 4.4 Sprint Review + Retrospettiva (1h — Giorno 10)

### Review (30 min)

- Risultati vs obiettivi (con dati)

- DLI aggiornato

- Delta sulle leve fisiche del flusso

- Movimento sulla matrice di efficienza

- Demo dell'intervento al team + stakeholder

### Retrospettiva (30 min)

**4 domande standard :**

- Cosa ha funzionato bene?

- Cosa non ha funzionato?

- Cosa cambiamo nel prossimo sprint?

- 1 cambiamento concreto deciso prima di chiudere

**5ª domanda (v1.4) — Standardizzazione**

- Cosa di questo sprint diventa nuovo standard? Quale runbook/template/checklist/Definition of Done/playbook va aggiornato? Chi lo mantiene? A chi va comunicato?

*Senza standardizzazione, il miglioramento è personale e non si propaga. È il principio della capacità evolutiva (DLF v**2.4** Sez 10.5.2).*

**6ª domanda (v1.4) — Lean Test (3 check anti-teatro lean)**

A fine retrospettiva, prima di chiudere, il practitioner conduce il **Lean Test** del DLF: tre domande operative che riconoscono il teatro lean in flagranza. Le risposte non si scrivono nel report; si pensano insieme all'Owner. Se una sola risposta è "no" o "non lo so", la deriva è già iniziata e va corretta subito.

| **Test** | **Domanda** | **Se NO** |
| --- | --- | --- |
| **1. Strumento orfano** | Per ogni strumento applicato in questo sprint, sai dire in 30 secondi (a) quale principio del DLF serve e (b) quale valore concreto il cliente del processo riceve come conseguenza? | Lo strumento è orfano. Sospendi lo strumento o ricollegalo al principio. Meglio non farlo che farlo a vuoto. |
| **2. Metodo cosmetico** | Negli ultimi 3 sprint, una delle metriche di flusso si è mossa? (DLI, flow ratio, posizione sulla matrice, throughput time, lavoro di trazione) | Ferma gli sprint. Diagnostica: stai aggredendo i sintomi invece della fonte di inefficienza dominante? Gli interventi sono troppo piccoli? Il management ha cambiato priorità senza dirlo? |
| **3. Strategia in fuga** | Qualche cliente — interno o finale — ha avuto un'esperienza tangibilmente migliore? (Lead time più corto percepito, meno solleciti, meno escalation) | Torna allo Step 0A (unità di flusso, confini) e 0C (bisogni). Probabilmente hai sbagliato a definire cosa il cliente vuole davvero. |

**Verdetto del Lean Test:**

- Tre sì → framework allineato, prosegui.

- Un no → correggi subito.

- Due no → ferma e rifletti prima del prossimo sprint.

- Tre no → torna alla Legge Zero e ricomincia.

**Setting**: il Lean Test si conduce dal practitioner *con* l'Owner del processo, *senza* chi ha interesse a mantenere lo status quo. Risposte oneste richiedono setting onesto.

# 5. Matrice FLOW — Prioritizzazione interventi (bottleneck-aware)

*Nota importante : la Matrice FLOW di questa sezione è la matrice impatto/complessità per prioritizzare gli interventi sul flusso. È diversa dalla Matrice di Efficienza del Pillar 3 (DLF v**2.4** Sez 7.5), che è il quadrante strategico flow × resource. Non confondere: questa è una matrice tattica di selezione interventi, quella è una matrice strategica di posizionamento.*

**COSA FARE:** Posizionare ogni intervento candidato su una matrice 2x2 (impatto sul valore × complessità di intervento) e applicare la regola di priorità bottleneck-aware.

## 5.1 La matrice 2×2

| | **Bassa complessità** | **Alta complessità** |
| --- | --- | --- |
| **Alto impatto** | Quick win lean (priorità 1) | Investimento strategico (priorità 3) |
| **Basso impatto** | Filler — solo se c'è tempo (priorità 2) | Da evitare (priorità 4) |

## 5.2 Regola di prioritizzazione

Applicare nell'ordine:

- Tra due interventi a pari quadrante, vince quello che muove una delle tre leve fisiche del flusso (bottleneck → WIP → variabilità).

- Tra due interventi che muovono leve fisiche diverse, vince quello che aggredisce il bottleneck.

- Tra due interventi a pari leva fisica, vince quello coerente con la transizione di quadrante dichiarata in Step 0B (es. se si va da Isole a Oceano, vince l'intervento che riduce utilizzo e libera flow).

**Domanda guida:** se questo intervento riesce, di quanto si muove il throughput del sistema? Se è zero (perché agisce su uno step che non è bottleneck), riprioritizza.

# 6. Applicazione per Dominio

Guide rapide per applicare il DLF v2.4 ai 4 operational tracks specialistici (6.1-6.4) e al transversal layer di orchestrazione (6.5). I tracks sono cantieri specialistici day-to-day; il transversal layer è la dimensione applicativa quando un'iniziativa end-to-end attraversa più tracks contemporaneamente. Per il dettaglio operativo del framework su ciascun track, vedi DLF v2.4 Sezione 12.

## 6.1 IT and Digital Service Delivery

| **Elemento** | **Dettaglio** |
| --- | --- |
| **Unità di flusso** | La richiesta dell’utente |
| **Bisogno diretto** | Servizio reso entro SLA con qualità e tempo di attesa adeguati |
| **Bisogni indiretti tipici** | Solleciti utenti, riassegnazioni manuali, sync meeting per ticket complessi, escalation a management, "report di stato" generati a posteriori, validazioni manuali di dato, riconciliazion |
| **Catena interna** | L1 triage → L2 verification → L3 specialist → vendor/HQ → closure. Per i dati: ingestion → cleansing → modeling → BI → consumo |
| **Quadrante target tipico** | Oceano (servizi critici), parte bassa Oceano (servizi standard ad alto volume) |
| **Bottleneck tipico** | L2 saturo, single SME a L3, timezone del vendor; per i dati: validatore unico, pipeline che si ferma per data quality issue |
| **Primo passo** | Mappare il flusso end-to-end del servizio o della pipeline dati. Identificare rimbalzi tra livelli (segnale di catena fornitore-cliente rotta). Per data: data contracts a monte |
| **Metrica chiave** | MTTR / cycle time del ticket; per dati: freshness, accuracy, completeness misurati al consumo |

## 6.2 Cybersecurity

| **Elemento** | **Dettaglio** |
| --- | --- |
| **Unità di flusso** | Il processo di business da garantire integro, NON l'alert |
| **Bisogno diretto** | Protezione del processo di business |
| **Bisogni indiretti tipici** | Report di stato a executive, meeting di crisi, comunicazioni interne/esterne, dashboard di stato incident |
| **Catena interna** | Detection → Triage → Analysis → Containment → Eradication → Recovery |
| **Quadrante target tipico** | Oceano — il business paga la velocità di response |
| **Bottleneck tipico** | Livello di approvazione per response actions, SME singolo necessario per ogni decisione di severity |
| **Primo passo** | Mappare i processi di business critici e i rischi associati. L'unità di flusso NON è l'alert |
| **Metrica chiave** | Tempo di ripristino del processo di business, non tempo di chiusura dell'incidente |

## 6.3 Leadership & People

| **Elemento** | **Dettaglio** |
| --- | --- |
| **Unità di flusso** | Bisogno formativo / decisionale → competenza applicata o decisione presa |
| **Bisogno diretto** | Competenza applicabile nel processo reale, oppure decisione efficace presa in tempo utile |
| **Bisogni indiretti tipici** | Da training inefficace: follow-up call, sessioni di rinforzo, coaching individuale, materiale aggiuntivo. Da decision flow lento: riunioni di "allineamento", escalation, comitati ad hoc, task force su decisioni che dovrebbero essere routine |
| **Catena interna** | Per formazione: bisogno organizzativo → progettazione → erogazione → applicazione sul campo → coaching → misurazione impatto. Per decision-making: raccolta input → analisi → proposta → decisione → comunicazione → implementazione |
| **Quadrante target tipico** | Oceano (per programmi critici e per decisioni di valore competitivo) o parte bassa Oceano (per training a volumi alti) |
| **Bottleneck tipico** | Per formazione: assenza di occasioni applicative immediate post-training. Per decisioni: decision authority concentrata in un singolo ruolo, o rito (board mensile) per decisioni che servono settimanalmente |
| **Primo passo** | Audit della formazione (cosa produce valore, cosa si traduce in azione) + mappatura dei rituali decisionali (quali esistono, quali producono decisioni, quali generano solo allineamento) |
| **Metrica chiave** | % partecipanti che applicano competenze a 30 giorni; tempo medio di decisione su classi di decisione standard; cambiamento comportamentale misurato con feedback peer-to-peer |

## 6.4 AI Adoption

| **Elemento** | **Dettaglio** |
| --- | --- |
| **Unità di flusso** | Processo con lavoro ripetitivo da automatizzare |
| **Bisogno diretto** | Risparmio di tempo, qualità decisionale, riduzione carico cognitivo |
| **Bisogni indiretti tipici** | Validazione manuale degli output AI, training continuo agli utenti, gestione delle eccezioni |
| **Catena interna** | Data → Preprocessing → Modello → Output → Validazione umana → Uso operativo |
| **Quadrante target tipico** | Dipende dall'use case; tipicamente Oceano per AI critica, Isole per AI ad alto volume e basso valore unitario |
| **Bottleneck tipico** | Step cognitivo ripetibile non automatizzato — se non è sul bottleneck, l'AI non muove il throughput |
| **Primo passo** | Mappatura processi ad alto contenuto ripetitivo. Identificare se il bottleneck è cognitivo. Semplificazione PRE-AI. Pilota su 1-2 use case |
| **Metrica chiave** | Impatto reale dell'AI su metriche concrete vs aspettative |

## 6.5 Digital Transformation Programs

Transversal Layer. Strutturalmente diverso dai 4 tracks: si applica a iniziative end-to-end che attraversano più tracks. Include: lanci di piattaforme, migrazioni cloud, digitalizzazione di processi prima cartacei, ridisegno di customer journey, consolidamenti applicativi

| **Elemento** | **Dettaglio** |
| --- | --- |
| **Unità di flusso** | L'iniziativa di redesign / migrazione end-to-end di un processo di business (NON il progetto IT, NON la singola feature, NON il deliverable) |
| **Bisogno diretto** | Outcome di business del processo trasformato (cycle time -X%, conversion rate +Y%, adoption del nuovo processo a 90 giorni) |
| **Bisogni indiretti tipici** | Status meeting di programma, dashboard di programma, escalation a steering committee, comunicazioni di slittamento, "war room" su deliverable critici, sync cross-track |
| **Catena interna** | Business needs → Product → Engineering → QA → Operations → Cliente (con orchestrazione cross-track esplicita) |
| **Quadrante target tipico** | Oceano per programmi critici, parte bassa Oceano per programmi di consolidamento ad alto volume |
| **Bottleneck tipico** | Può vivere in qualsiasi dei 4 tracks toccati: code review (IT), security approval (Cyber), change management/formazione (Leadership), AI workflow non maturo (AI Adoption). Il bottleneck del programma è il bottleneck del track più lento toccato in quel momento |
| **Primo passo** | Identificare quali dei 4 operational tracks il programma attraversa. Ogni track avrà il suo sub-DLI. Il programma ha un DLI composito ponderato sul valore del business outcome. Per chi ha già digitalizzato e si trova con processo digitale ma rotto: Percorso B della Legge Zero. Per chi sta lanciando: Legge Zero rigorosa a monte, prima di scegliere la tecnologia |
| **Metrica chiave** | DLI composito del programma pre/post + outcome di business (le metriche del processo trasformato) |
| **Quando applicarlo** | Quando l'iniziativa NON è gestione di un servizio in esercizio ma redesign / migrazione / lancio di un processo di business. Spesso un programma di trasformazione, una volta concluso, lascia in eredità un servizio operativo che da quel momento vive nel suo operational track (es. nuova piattaforma lanciata via 6.5 diventa servizio gestito via 6.1) |

# 7. Lean Advisor — Guida all'uso dell'AI Operativa

Il Lean Advisor è una skill AI interattiva che guida l'applicazione operativa del DLF v2.4. Non è un chatbot che spiega la teoria lean: è uno strumento operativo che ti accompagna attraverso assessment concreti, calcoli reali, decisioni strutturate.

**QUANDO USARLO:** Quando vuoi applicare il DLF v2.4 su un processo reale e vuoi essere guidato passo-passo.

## 7.1 Le 5 Modalità Operative

Restano 5 modalità — nessuna sesta. L'estensione v2.2/v2.4 (matrice di efficienza, catena interna, frontiera raggiungibile, Pillar 5 Jidoka digitale) è codificata DENTRO la Modalità 1 (Assessment DLI), non in una modalità separata. Questa scelta protegge la coerenza del flusso operativo: la matrice e Jidoka sono strumenti dell'assessment, non assessment a sé.

| **Modalità** | **Quando usarla** | **Cosa fa** | **Output** |
| --- | --- | --- | --- |
| **1. Assessment DLI** | Vuoi misurare la salute lean di un processo | Guida Step 0 → Step 6 completo, incluso Step 0B bidimensionale matrice, Step 0C bisogni, Step 0D catena interna, Step 2 esteso con WIP/bottleneck/variabilità, Step 5 matrice-aware (transizione + frontiera) | Report DLI con baseline, metriche di fisica del flusso, posizionamento sulla matrice di efficienza, frontiera raggiungibile, piano d'intervento matrice-aware |
| **2. Muda Scan** | Vuoi analizzare gli sprechi di un processo | Guida attraverso i 9 muda con scoring e annotazione bisogno indiretto associato | Muda Assessment Report con priorità per doppio dividendo |
| **3. Sprint Kaizen** | Vuoi strutturare interventi in sprint | Definisce obiettivi, owner, metriche, leva fisica del flusso impattata, movimento atteso sulla matrice | Sprint Card + template rituali |
| **4. Legge Zero** | Stai per scegliere una tecnologia o metodologia | Guida nel workflow a 3 percorsi, con check su bisogni diretti | Decision Record strutturato |
| **5. DLI Calculator** | Hai i dati e vuoi calcolare il DLI | Raccoglie dati, calcola, interpreta. Raccoglie WIP/bottleneck/variabilità per orientare lo Step 5. Raccoglie anche quadrante attuale e target per il layer matrice | DLI Scorecard + leve fisiche + posizionamento matrice |

## 7.2 Come iniziare una sessione

Apri una conversazione nel progetto DLF e descrivi cosa vuoi fare. Esempi:

- "Voglio fare un assessment DLI sul processo di incident response" → Modalità 1

- "Voglio analizzare gli sprechi nel processo di onboarding" → Modalità 2

- "Ho identificato 3 interventi, aiutami a strutturare lo sprint" → Modalità 3

- "Stiamo per scegliere un nuovo SIEM, guidami con la Legge Zero" → Modalità 4

- "Ho i dati del value stream map, calcoliamo il DLI" → Modalità 5

## 7.3 Cosa aspettarsi

- Il Lean Advisor procede un blocco alla volta. Non ti travolge con 20 domande.

- Chiede evidenze concrete per ogni punteggio.

- Non inventa dati. Se mancano informazioni, lo segnala e suggerisce come raccoglierle.

- Produce output strutturati: report, scorecard, sprint card, decision record.

- Segue fedelmente il DLF v2.4. Non semplifica le formule e non salta step.

- Distingue chiaramente i dati qualitativi dai quantitativi — segnala esplicitamente quando una valutazione è qualitativa (variabilità, frontiera raggiungibile, posizione sulla matrice) e non rigorosa.

## 7.4 Suggerimenti per sessioni efficaci

- Prepara i dati prima della sessione: tempi del processo, numero di tool, handoff, livelli di approvazione, stima WIP per step.

- Prepara la dichiarazione del quadrante target: parla in anticipo col business owner per sapere se il modello è "prezzo" (Isole), "velocità" (Oceano), o ibrido.

- Coinvolgi le persone giuste: le risposte migliori vengono da chi vive il processo.

- Non avere fretta: un assessment fatto bene in 3 sessioni vale più di uno fatto male in 1.

- Salva gli output: il Lean Advisor può generare file Word, Excel e presentazioni dei risultati.

- Usa i risultati: il DLI non è un numero da mettere in una slide. È la baseline da cui partire per il primo Sprint Kaizen. Anche il posizionamento sulla matrice e la frontiera raggiungibile sono baseline strategiche da cui partire — vanno tracciate sprint su sprint.

## 7.5 Percorso consigliato per il primo utilizzo

| **Sessione** | **Durata** | **Cosa fare** | **Output** |
| --- | --- | --- | --- |
| **Sessione 1** | 75-105 min | Step 0 completo (0A + 0B bidimensionale + 0C bisogni + 0D catena interna) + Step 1 (Selezione) + inizio Step 2 | Unità di flusso, posizionamento matrice (attuale + target + frontiera), bisogni diretti/indiretti, matrice catena interna, confini processo, primi step mappati |
| **Sessione 2** | 75-105 min | Completare Step 2 (inclusi WIP, bottleneck, variabilità) + Step 3 (Muda Assessment) | Value Stream Map completa con metriche di fisica del flusso + Waste Score + annotazioni bisogni indiretti |
| **Sessione 3** | 60-90 min | Step 4 (Calcolo DLI) + Step 5 (Piano matrice-aware) + Sprint Planning | DLI Scorecard + interpretazione su frontiera + leve fisiche identificate + Sprint Card #1 con leva fisica e movimento atteso sulla matrice |

# Nota finale

*Meno complessità, più risultati.*

Questa guida è un documento vivo. Si aggiorna con l'esperienza dei pilota, con i feedback del team, con i risultati degli sprint. La versione che stai leggendo riflette l'evoluzione strutturale del framework con 5 pillar (Legge Zero, Catena cliente-fornitore interno, Tre Leggi del Flusso + Matrice di Efficienza, Bisogni diretti e indiretti, Visibilità del flusso e Jidoka digitale) e 4 valori culturali.

Il principio che vale per il framework vale anche per questa guida: se qualcosa non funziona, semplifica. Se qualcosa manca, aggiungi. Se qualcosa è superfluo, togli. Kaizen.

*— Digital Lean Framework, Guida Operativa v1.4*
