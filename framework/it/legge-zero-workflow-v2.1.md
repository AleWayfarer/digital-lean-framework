---
asset: legge-zero-workflow
version: 2.1
compatible-with: DLF v2.4
author: Alessio Setaro
license: CC BY-NC-ND 4.0
---

# Legge Zero — Workflow Operativo a 3 Percorsi

> *Non partire mai dalla tecnologia per plasmare il processo.
> Parti dal processo per scegliere la tecnologia.*

La Legge Zero è la legge fondamentale del DLF. Viene prima di tutto il resto.
Se violata, rende inutile qualsiasi altro principio.

Il peccato originale ha due facce:
1. Partire dalla tecnologia per plasmare il processo
2. Trasformare digitalmente un processo senza prima ripensarlo

---

## Indice

1. [Decision Tree — Quale percorso?](#decision-tree)
2. [Percorso A — Non hai ancora digitalizzato](#percorso-a)
3. [Percorso B — Hai già digitalizzato (Remediation)](#percorso-b)
4. [Percorso C — Processi umani e organizzativi](#percorso-c)
5. [Output: Decision Record](#output)
6. [Red Flag — Segnali di violazione della Legge Zero](#red-flag)

---

## <a name="decision-tree"></a>Decision Tree — Quale percorso?

Prima domanda all'utente:
> "Il processo che vuoi affrontare è già digitalizzato, non ancora digitalizzato,
> o è un processo prevalentemente umano/organizzativo?"

### Classificazione:

| Risposta | Percorso | Descrizione |
|---|---|---|
| "Non è ancora digitalizzato" | **Percorso A** | Il processo esiste ma non ha componenti digitali significative. Stai per scegliere se/come digitalizzare. |
| "Sì, è già digitalizzato" | **Percorso B** | Il processo è già su sistemi digitali ma non funziona come dovrebbe, o ha generato complessità. |
| "È un processo umano / organizzativo" | **Percorso C** | Il processo riguarda leadership, formazione, decision-making, cultura, organizzazione. La "tecnologia" è un framework, una metodologia, un tool di assessment. |
| "Un mix" | **Domanda di follow-up** | "Qual è la parte che ti dà più problemi? Partiamo da lì." Poi classifica quella parte. |

---

## <a name="percorso-a"></a>Percorso A — Non hai ancora digitalizzato

### Step A1 — COMPRENDI

**Obiettivo**: capire il problema reale e il processo esistente.

Domande operative:
- "Qual è il problema che vuoi risolvere con la digitalizzazione?"
- "Come funziona il processo oggi? Descrivilo step by step."
- "Chi vive questo processo ogni giorno? Hai parlato con loro?"
- "Cosa non funziona? Dove si perde tempo, si fanno errori, si crea frustrazione?"

**Red flag**: se l'utente inizia a parlare di tool o piattaforme, fermalo.
> "Aspetta — siamo allo Step 1. Non parliamo ancora di tecnologia.
> Parliamo del processo. Cosa non funziona OGGI, a prescindere dagli strumenti?"

**Output**: descrizione del problema e del processo as-is.

### Step A2 — OTTIMIZZA

**Obiettivo**: ottimizzare il processo a prescindere dalla tecnologia.

Domande operative:
- "Dei passaggi che hai descritto, quali producono valore per il cliente/utente finale?"
- "Quali passaggi sono attese, approvazioni, handoff che potresti eliminare?"
- "Se dovessi tagliare il 30% degli step, quali toglieresti?"
- "Qual è il processo ideale — il più semplice possibile che produce comunque il risultato?"

Qui è utile innescare la Modalità 2 (Muda Scan) se il processo è complesso.

**Output**: processo ottimizzato (to-be semplificato).

### Step A3 — SCEGLI

**Obiettivo**: scegliere la tecnologia che serve il processo ottimizzato.

Domande operative:
- "Ora che il processo è semplificato, quali step beneficerebbero di un supporto digitale?"
- "Per ciascuno: cosa deve fare il tool? (requisiti funzionali minimi)"
- "Ci sono vincoli? (budget, integrazione con sistemi esistenti, competenze del team)"
- "Stai valutando un tool specifico? Se sì, perché quello?"

**Red flag**: se l'utente ha già scelto il tool e sta cercando conferma, sfida:
> "Hai scelto [tool] prima di definire i requisiti del processo ottimizzato.
> Sei sicuro che [tool] serve il processo, o stai adattando il processo al tool?"

**Output**: lista di requisiti funzionali derivati dal processo, non dal catalogo del vendor.

### Step A4 — ADATTA

**Obiettivo**: adattare la tecnologia al processo, mai il contrario.

Domande operative:
- "Il tool che hai scelto rispetta tutti i requisiti funzionali definiti?"
- "Ci sono funzionalità del tool che NON servono al processo? (potenziale overprocessing)"
- "Dove il tool non copre un requisito, cosa fai? Adatti il processo (SBAGLIATO)
  o cerchi un'alternativa/workaround?"
- "Chi forma il team? Il team capisce il processo prima del tool?"

**Principio**: la tecnologia è un servitore del processo. Se il processo deve
cambiare per adattarsi al tool, stai violando la Legge Zero.

**Output**: piano di implementazione allineato al processo.

---

## <a name="percorso-b"></a>Percorso B — Hai già digitalizzato (Remediation)

### Step B1 — MAPPA

**Obiettivo**: mappare lo stato attuale del processo digitalizzato.
Come funziona DAVVERO, non come dovrebbe funzionare sulla carta.

Domande operative:
- "Descrivi come funziona il processo oggi, nella realtà. Non come è documentato —
  come funziona davvero."
- "Ci sono workaround? Cose che le persone fanno 'fuori dal sistema'?"
- "Ci sono funzionalità del sistema che nessuno usa?"
- "Ci sono step che esistono solo perché il sistema li richiede?"

**Output**: mappa del processo reale vs. processo teorico. Gap evidenziati.

### Step B2 — IDENTIFICA

**Obiettivo**: identificare il waste generato dalla digitalizzazione stessa.

Domande operative:
- "Quali workaround sono nati DOPO la digitalizzazione?"
- "Ci sono duplicazioni di dati tra sistemi?"
- "Ci sono step che sono più complessi di prima perché il sistema lo impone?"
- "Ci sono funzionalità che non usate ma che pagate?"
- "Il processo è stato adattato al software, o il software al processo?"

**Categorizza il waste trovato** usando i 9 Muda Digitali (innesca Modalità 2
se utile).

**Output**: lista di waste generato dalla digitalizzazione, categorizzato per muda.

### Step B3 — SEMPLIFICA

**Obiettivo**: semplificare il processo DENTRO il sistema esistente.
Non buttare via tutto — riporta ordine in ciò che hai costruito.

Domande operative:
- "Dei workaround identificati, quali puoi eliminare riconfigurando il sistema?"
- "Delle funzionalità non usate, quali puoi disattivare/rimuovere?"
- "Dei passaggi imposti dal sistema, quali puoi bypassare con configurazione?"
- "Dove il processo è stato adattato al software, puoi invertire?"

**Principio**: la remediation non è ricominciare da zero. È potare,
riordinare, semplificare dall'interno.

**Output**: piano di semplificazione con interventi specifici.

### Step B4 — DECIDI

**Obiettivo**: decidere cosa tenere, eliminare, riprogettare.

Domande operative:
- "Per ogni elemento del processo: teniamo, eliminiamo, o riprogettamo?"
- "La decisione è basata su dati (usage, impatto, costi) o su opinioni?"
- "Se eliminiamo [X], qual è l'impatto? Chi se ne accorge?"
- "C'è un business case per riprogettare vs. semplificare?"

**Output**: Decision Matrix con keep/eliminate/redesign per ogni elemento.

---

## <a name="percorso-c"></a>Percorso C — Processi umani e organizzativi

La "tecnologia" da non anteporre al processo qui può essere: un framework
organizzativo, una metodologia di formazione, un modello di leadership,
un tool di assessment, una piattaforma HR.

### Step C1 — COMPRENDI

**Obiettivo**: capire il bisogno organizzativo reale.

Domande operative:
- "Qual è il bisogno organizzativo che vuoi affrontare?"
- "Non partire dalla soluzione — qual è il PROBLEMA?"
- "Quali comportamenti vuoi cambiare? In chi? Perché?"
- "Questo bisogno è emerso da dati, feedback, osservazione diretta?"

**Red flag**: se l'utente inizia con "Vogliamo implementare [piattaforma/framework]":
> "Aspetta — perché volete implementare [X]? Qual è il bisogno sottostante?
> Potrebbe esserci una soluzione più semplice."

**Output**: bisogno organizzativo formulato come problema, non come soluzione.

### Step C2 — OSSERVA

**Obiettivo**: capire come funziona il processo umano oggi.

Domande operative:
- "Come si prendono le decisioni oggi? Chi decide cosa? Quanto ci vuole?"
- "Come si sviluppano le competenze? Formazione formale, on the job, coaching?"
- "Come circola l'informazione? Meeting, email, chat, passaparola?"
- "Dove si creano i silos? Dove le persone NON collaborano?"

**Output**: mappa del processo umano as-is.

### Step C3 — PROGETTA

**Obiettivo**: progettare l'intervento a partire dal processo umano.

Domande operative:
- "Dato il bisogno e il processo attuale, quale intervento ha senso?"
- "Serve uno strumento o basta un cambiamento di processo?"
- "A volte lo strumento migliore è una conversazione strutturata, non una piattaforma.
  È il caso qui?"
- "Come misurerai che l'intervento ha funzionato? Quale comportamento cambia?"

**Output**: design dell'intervento ancorato al processo umano.

### Step C4 — SCEGLI

**Obiettivo**: scegliere lo strumento SOLO se serve, DOPO aver definito il processo.

Domande operative:
- "L'intervento progettato richiede uno strumento? Quale?"
- "Se sì, lo strumento serve il processo o lo strumento definisce il processo?"
- "Potete partire senza strumento e aggiungere dopo, quando il processo è rodato?"

**Output**: decisione motivata su strumento sì/no e quale.

---

## <a name="output"></a>Output: Decision Record

Alla fine di qualsiasi percorso, genera un Decision Record:

```
📋 LEGGE ZERO — DECISION RECORD
Data: [data]
Processo: [nome]
Percorso: [A / B / C]

CONTESTO:
[Breve descrizione del punto di partenza]

STEP PERCORSI:
1. [Step 1]: [output sintetico]
2. [Step 2]: [output sintetico]
3. [Step 3]: [output sintetico]
4. [Step 4]: [output sintetico]

DECISIONE:
[Cosa si è deciso e perché]

RED FLAG IDENTIFICATI:
[Eventuali violazioni della Legge Zero intercettate durante il percorso]

PROSSIMO PASSO:
[Azione concreta]
```

---

## <a name="red-flag"></a>Red Flag — Segnali di violazione della Legge Zero

Il Lean Advisor deve intercettare queste situazioni e segnalarle:

| Segnale | Violazione | Risposta |
|---|---|---|
| "Abbiamo scelto [tool], ora progettiamo il processo" | Processo adattato al tool | "Stai partendo dalla tecnologia. Torniamo al processo." |
| "Il vendor dice che [feature] ci serve" | Vendor-driven design | "Il vendor vende funzionalità. Tu hai bisogno di risolvere un problema. Qual è il problema?" |
| "Tutti usano [piattaforma], dobbiamo averla anche noi" | Benchmark senza contesto | "Il fatto che altri la usino non significa che serva a te. Qual è il TUO processo?" |
| "Implementiamo il framework [X] di [guru]" | Framework prima del bisogno | "Perché? Qual è il bisogno a cui [framework] risponde? Potrebbe essere overkill." |
| "Aggiorniamo il sistema perché è vecchio" | Modernizzazione fine a sé stessa | "Vecchio non è automaticamente sbagliato. Il processo funziona? Genera waste?" |
| "Mettiamo l'AI su [processo]" | AI washing | "Prima: il processo è pulito? L'AI su un processo sporco amplifica il disordine." |
