---
asset: muda-checklist
version: 2.3
compatible-with: DLF v2.4
author: Alessio Setaro
license: CC BY-NC-ND 4.0
---

# Muda Checklist — I 9 Muda Digitali (v2.3)

Guida operativa per l'assessment dei 9 Muda Digitali del DLF.
Per ciascun muda: definizione, domande diagnostiche, segnali, scoring 0-3,
metriche quantitative, **bisogno indiretto associato (v2.1)**, **fonte di
inefficienza tipica (v2.2)**.

**Cosa cambia in v2.3** (questa versione): allineamento al **DLF v2.4**
(master modificato), fix ordinamento muda 8 (Unused Talent) e 9 (Perfection
Trap) per coerenza con master v2.4 Sez 10.3. Nessuna modifica concettuale
allo scoring, alle domande diagnostiche, alla mappatura fonti.

**Cosa è stato aggiunto in v2.2** (riferimento storico): per ciascun muda è
aggiunta l'indicazione della **fonte di inefficienza tipica** secondo la
lettura causale del DLF (Sez 8.1 master) — lungo throughput time / WIP alto /
molti riavvii. Questa annotazione supporta lo Step 3 fonte-aware dell'assessment
DLI: dopo aver scorato i muda, si identifica la fonte di inefficienza dominante —
quella che genera la maggioranza dei muda gravi osservati — e si aggrediscono
in via prioritaria le cause, non i sintomi singoli.

**Mappatura sintetica muda → fonte:**

| Muda | Fonte di inefficienza tipica |
|---|---|
| 1. Overprocessing | WIP alto (sovrabbondanza di gestione concorrente) |
| 2. Waiting | Lungo throughput time |
| 3. Overproduction | Molti riavvii (e/o assenza di pull) |
| 4. Defects | Molti riavvii (perdita di contesto a ogni handoff) |
| 5. Transport | Molti riavvii (handoff strutturale) |
| 6. Inventory | Lungo throughput time + WIP alto |
| 7. Motion | Molti riavvii (context switch tra tool e contesti) |
| 8. Unused Talent | WIP alto (impossibilità di applicare competenze sotto sovraccarico) |
| 9. Perfection Trap | WIP alto (sovrabbondanza di iterazione concorrente) |

**Cosa cambia in v2.1** (riferimento storico): per ciascun muda è aggiunta
l'annotazione del bisogno indiretto tipicamente generato. I muda con bisogno
indiretto SÌ hanno priorità di intervento perché eliminandoli si elimina
anche il "lavoro di trazione" conseguente — doppio dividendo.

**Collegamento al framework v2.4**: questa checklist opera dentro il contesto
dei **5 Pillar** (Legge Zero, Catena interna, Tre Leggi + Matrice, Bisogni
diretti/indiretti + Tre fonti di inefficienza, Visibilità del flusso Jidoka)
del DLF v2.4. Chi entra dalla checklist senza essere passato dal framework
dovrebbe prima leggere le Sezioni 5-9 del DLF: l'identificazione dei muda è
più precisa quando si sa dove sta il bottleneck del processo, quale lavoro
di trazione i muda stanno generando, e su quale fonte di inefficienza
risalgono.

**Come usare questa checklist:**
Procedi muda per muda, in ordine. Per ciascuno:
1. Leggi la definizione (per te, non serve ripeterla tutta all'utente)
2. Poni le domande diagnostiche (2-3 alla volta, non tutte insieme)
3. Ascolta le risposte e cerca i segnali
4. Chiedi il punteggio 0-3 O suggeriscilo sulla base delle evidenze
5. Per ogni punteggio > 0, chiedi: "Quale evidenza concreta lo supporta?"
6. Raccogli la metrica quantitativa se disponibile

**Scoring:**
- 0 = Assente: nessuna evidenza di questo spreco
- 1 = Lieve: presente ma marginale, impatto limitato
- 2 = Moderato: presente e visibile, impatto significativo
- 3 = Grave: sistemico, impatto pesante su flow e valore

---

## Muda 1 — OVERPROCESSING (Sovra-elaborazione)

**Definizione**: tool e processi più complessi del necessario. Architetture
overengineered. Report con 50 KPI quando ne servono 5.

**Domande diagnostiche:**
- "Quanti step ha il processo? Quanti di questi producono direttamente valore
  per il cliente/utente finale?"
- "Ci sono tool o funzionalità che il team usa al 20% delle capacità?"
- "Esiste documentazione di processo che nessuno legge o segue?"
- "C'è qualcosa nel processo che esiste solo perché 'abbiamo sempre fatto così'?"
- "Se dovessi spiegare il processo a un nuovo arrivato, in quanti minuti ci riusciresti?"

**Segnali tipici:**
- Tool che nessuno sa usare al 100%
- Processi che richiedono un manuale per essere seguiti
- Report con decine di KPI di cui se ne guardano 3
- Step che esistono "per sicurezza" senza un rischio reale da mitigare

**Metrica quantitativa**: numero di step nel processo vs. step a valore diretto.
Formula: step a valore / step totali. Se < 50%, hai overprocessing significativo.

**Bisogno indiretto associato (v2.1)**: **Sì.** Tool complessi e processi
ridondanti generano richieste di chiarimento, training continuo per l'uso,
documentazione di processo che a sua volta richiede manutenzione. Il muda
primario genera lavoro di trazione (knowledge management, support, training)
che non esisterebbe se il processo fosse semplice.

---

## Muda 2 — WAITING (Attesa)

**Definizione**: tempi morti tra decisione e azione. Approvazioni multiple.
Silos organizzativi. Dipendenze non gestite.

**Domande diagnostiche:**
- "Quando [unità di flusso] entra nel processo, quanto tempo passa prima che
  qualcuno ci lavori effettivamente?"
- "Quanti livelli di approvazione ci sono? Quali sono davvero necessari?"
- "Capita di dover sollecitare qualcuno per far avanzare il processo? Quanto spesso?"
- "Ci sono momenti in cui il lavoro si ferma perché si aspetta un'altra funzione/team?"

**Segnali tipici:**
- Lead time >> processing time
- Email di sollecito ricorrenti
- "Sto aspettando che mi rispondano..."
- Code di lavoro che crescono

**Metrica quantitativa**: % del lead time in attesa vs. in lavorazione.
Formula: tempo di attesa / throughput time × 100.
Se > 70%, il processo è dominato dall'attesa.

**Bisogno indiretto associato (v2.1)**: **Sì — è il principale generatore
di bisogni indiretti.** L'attesa è la condizione che attiva tutti i tipici
"lavori di trazione": solleciti, richieste di status update, dashboard di
tracking, escalation, riunioni di review backlog. Eliminare Waiting elimina
direttamente tutta la macchina del "servizio dello stato" — che spesso vale
più del muda primario in termini di tempo del team. Doppio dividendo
massimo.

---

## Muda 3 — OVERPRODUCTION (Sovrapproduzione)

**Definizione**: output che nessuno usa. Report automatici, dashboard con 0 views,
meeting che producono nulla, documentazione che nessuno legge.

**Domande diagnostiche:**
- "Ci sono report o dashboard che vengono generati automaticamente? Chi li guarda?"
- "Quanti meeting ricorrenti ci sono? Quanti hanno un'agenda e producono decisioni?"
- "C'è documentazione che viene prodotta per processo ma mai consultata?"
- "Se smettessi di generare [output X] domani, chi se ne accorgerebbe?"

**Segnali tipici:**
- Report automatici in archivio senza lettori
- Dashboard con 0 views nelle ultime 4 settimane
- Meeting ricorrenti senza agenda e senza decisioni
- Documentazione prodotta "perché il processo lo richiede"

**Metrica quantitativa**: % di report/dashboard con zero visualizzazioni in 30 giorni.
Per i meeting: % meeting senza decisioni documentate nell'ultimo mese.

**Bisogno indiretto associato (v2.1)**: **Indirettamente.** L'overproduction
non genera direttamente "lavoro di trazione" sul cliente esterno — è waste
auto-prodotto. Ma genera un effetto secondario: gli output sovraprodotti
vengono "ignorati" sistematicamente, e questo porta a richieste tipo
"servirebbe un report più semplice" o "questo dashboard non lo guarda
nessuno, possiamo averne uno utile?". Lavoro di rimedio che si attiverebbe
meno se si producesse meno e meglio dall'inizio.

---

## Muda 4 — DEFECTS (Difetti)

**Definizione**: rework causato da processi mal disegnati. Errori ripetitivi.
Incidenti di sicurezza da configurazioni errate. Formazione senza impatto.

**Domande diagnostiche:**
- "Quante volte capita di dover rifare un lavoro già fatto? Con quale frequenza?"
- "Ci sono errori che si ripetono ciclicamente (ogni settimana/mese)?"
- "Qual è il tasso di rework nel processo? (task riaperti, bug ritornanti, incidenti ricorrenti)"
- "La formazione fatta nell'ultimo anno ha prodotto un cambiamento visibile nei comportamenti?"

**Segnali tipici:**
- "L'abbiamo già corretto la settimana scorsa" (e torna)
- Stessi errori, stesse root cause
- Incidenti ricorrenti con la stessa categoria
- Formazione erogata senza follow-up comportamentale

**Metrica quantitativa**: tasso di rework = % task riaperti entro 7 giorni.
Per cybersecurity: % incidenti con root cause ricorrente.
Per formazione: % partecipanti che applicano dopo 30 giorni (se misurabile).

**Bisogno indiretto associato (v2.1)**: **Sì.** Ogni difetto genera lavoro
di comunicazione attorno alla correzione: richieste di status sulla
riparazione, comunicazioni di scuse al cliente, post-mortem, follow-up,
report di affidabilità verso il management. È meno visibile del muda
primario (il rework) ma cumulativamente significativo. Particolarmente
costoso quando i difetti sono ricorrenti — il lavoro di trazione diventa
una routine permanente.

---

## Muda 5 — MOTION (Movimento inutile)

**Definizione**: context switching. Meeting inutili. Complessità organizzativa.
Tempo speso a cercare informazioni invece che a usarle.

**Domande diagnostiche:**
- "Quanti tool diversi usa il team quotidianamente? Più di 5?"
- "Che percentuale del tempo è in meeting vs. in lavoro produttivo?"
- "Quanto tempo si perde a cercare informazioni (file, dati, persone giuste)?"
- "Quante volte al giorno il team deve cambiare contesto tra attività diverse?"

**Segnali tipici:**
- Più di 5 tool aperti contemporaneamente
- Più del 30% del tempo in meeting
- "Non so dove trovare..." ricorrente
- Context switching continuo tra progetti/tool/priorità

**Metrica quantitativa**: ore/settimana in meeting vs. ore in lavoro produttivo.
Secondaria: numero di tool attivi per utente/giorno.

**Bisogno indiretto associato (v2.1)**: **Tipicamente no.** Motion è waste
interno al team che vive il processo — il cliente esterno non lo percepisce
direttamente. Non genera quindi richieste esterne di "trazione". Però attenzione:
l'effetto secondario è il **burnout dei team**, che a sua volta genera turnover,
onboarding ripetuto, knowledge loss. È un costo indiretto che si vede sul
medio periodo, non come "lavoro di trazione" immediato.

---

## Muda 6 — INVENTORY (Scorte)

**Definizione**: licenze software inutilizzate. Tech debt accumulato.
Backlog infiniti. Progetti zombie.

**Domande diagnostiche:**
- "Quante licenze software sono attive? Quante effettivamente usate?"
- "Com'è il backlog? Ci sono item più vecchi di 6 mesi che non si muovono?"
- "Ci sono progetti che sono 'in corso' da mesi senza progressi visibili?"
- "Quanto tech debt c'è? Viene mai affrontato o solo accumulato?"

**Segnali tipici:**
- Licenze pagate e non attivate/usate
- Backlog > 6 mesi senza pulizia
- Progetti zombie: nessun progresso da mesi ma non cancellati
- Tech debt che cresce senza piano di rientro

**Metrica quantitativa**: % licenze software attive vs. pagate.
Secondaria: età media del backlog (in giorni). Numero di progetti senza
progressi documentati negli ultimi 90 giorni.

**Bisogno indiretto associato (v2.1)**: **Indirettamente.** Il backlog gonfio
genera richieste ricorrenti da parte di chi ha cose in coda: "a che punto è
la mia richiesta X?", "questa feature è ancora in pipeline?", "il mio
progetto è abbandonato?". Più il backlog è vecchio e illeggibile, più lavoro
di "scavo nel backlog" si genera per rispondere a queste richieste. Le
licenze inutilizzate non generano trazione diretta — ma costano e occupano
attenzione amministrativa (audit, rinnovi, valutazione di valore).

---

## Muda 7 — TRANSPORT (Trasporto inutile)

**Definizione**: passaggi di consegna non necessari. Duplicazione di informazioni
tra sistemi. Dati copiati manualmente.

**Domande diagnostiche:**
- "Quanti handoff ci sono nel processo end-to-end?"
- "Le stesse informazioni esistono in più sistemi? Quanti?"
- "C'è copia-incolla manuale di dati tra sistemi?"
- "Quante persone/team toccano [unità di flusso] dall'inizio alla fine?"

**Segnali tipici:**
- Copia-incolla tra sistemi (il classico "export Excel → import nell'altro tool")
- Più di 3 handoff per processo end-to-end
- Stessa informazione in 4 posti diversi
- Email come sistema di trasporto dati

**Metrica quantitativa**: numero di handoff per processo end-to-end.
Secondaria: numero di sistemi in cui la stessa informazione è duplicata.

**Bisogno indiretto associato (v2.1)**: **Sì.** Ogni handoff genera un punto
di potenziale richiesta di status: "ho passato la richiesta a X, a che punto
è?". Le duplicazioni di dati tra sistemi generano richieste di
riconciliazione ("ma allora qual è il dato giusto?"). Con N handoff in
sequenza, l'unità di flusso può essere oggetto di N×K richieste di status
durante il suo attraversamento, dove K è la frequenza con cui chi ha
consegnato vuole sapere a che punto è. Riducendo gli handoff si elimina
proporzionalmente questo lavoro.

---

## Muda 8 — UNUSED TALENT (Talento inutilizzato)

**Definizione**: persone senior su lavoro operativo ripetitivo. Competenze bloccate
nei silos. Idee che muoiono perché "non è nel mio perimetro." Team che eseguono
senza capire il perché.

**Nota**: questo è il classico 8° muda della scuola lean occidentale, qui adattato
al contesto digitale. L'AI rischia di amplificarlo: se non liberi le persone per
il pensiero di alto livello, l'automazione produce spreco più veloce.

**Domande diagnostiche:**
- "Le persone senior del team quanto tempo passano su task operativi vs. strategici?"
- "Ci sono competenze nel team che non vengono sfruttate perché 'non è il loro ruolo'?"
- "Il team sa PERCHÉ fa quello che fa, o esegue senza contesto?"
- "Quando qualcuno ha un'idea di miglioramento, c'è un canale per proporla?
  Viene ascoltata?"

**Segnali tipici:**
- Senior su task da junior
- "Non è di mia competenza" come risposta abituale
- Nessuno chiede "perché lo facciamo?"
- Idee che non trovano spazio perché non rientrano nel perimetro formale
- Automazione di task che avrebbe potuto liberare tempo per pensiero strategico,
  ma che invece ha solo spostato le persone su altri task operativi

**Metrica quantitativa**: % tempo senior su task operativi vs. strategici.
Secondaria: numero di idee di miglioramento proposte dal team negli ultimi 90 giorni.

**Bisogno indiretto associato (v2.1)**: **Tipicamente no.** È un muda interno
organizzativo: il "danno" sta nella persona/talento non valorizzato, non in
un flusso che genera richieste esterne di trazione. Però gli effetti
collaterali sono significativi sul medio termine: disengagement, perdita di
talento (turnover), declino della cultura organizzativa, fuga delle persone
più capaci verso contesti più stimolanti. Non lavoro di trazione, ma costo
strategico.

---

## Muda 9 — PERFECTION TRAP (Trappola della perfezione)

**Definizione**: cercare il prodotto perfetto invece del MVP. Feature che mancano
sempre. Iterazioni infinite senza utenti reali. Sunk cost fallacy.

**Nota**: questo è un muda ORIGINALE del DLF, nato dall'osservazione che nel digitale
il ciclo di feedback non è fisico come nel manufacturing — si può iterare all'infinito
senza mai toccare la realtà.

**Domande diagnostiche:**
- "C'è qualche progetto o iniziativa che è 'quasi pronto' da più di 3 mesi?"
- "Quanti rilasci ci sono stati negli ultimi 90 giorni?"
- "Quanto tempo passa dal primo commit/draft al primo utente reale?"
- "Ci sono specifiche o requisiti in continuo cambiamento senza mai arrivare a 'done'?"
- "Qualcuno ha mai detto 'manca solo questa feature'... più di una volta?"

**Segnali tipici:**
- "Manca solo questa feature" (ricorrente)
- Progetti > 6 mesi senza un utente reale
- Specifiche in continuo cambiamento
- Sunk cost: "Abbiamo investito troppo per mollare"
- Perfezione come scusa per non rilasciare

**Metrica quantitativa**: numero di rilasci negli ultimi 90 giorni.
Secondaria: tempo medio dal primo commit/draft al primo utente reale.
Se il rapporto rilasci/90 giorni è < 1 e il time-to-user è > 90 giorni,
la Perfection Trap è probabile.

**Bisogno indiretto associato (v2.1)**: **Sì.** Rilasci lenti o assenti
generano un flusso continuo di richieste tipo "quando arriva X?", "siete
ancora in tempo?", "ce la facciamo per la deadline?". Genera review di
stato infinite, riunioni di "allineamento sulla data", comunicazioni di
slippage. Il muda primario (perfezionismo che non rilascia) genera
quindi un muda secondario potente: la macchina della comunicazione di
slittamento, che cresce esponenzialmente con il ritardo accumulato.

---

## Output Finale — Muda Assessment Report

```
📊 MUDA ASSESSMENT REPORT
Processo: [nome]
Data: [data]

| # | Muda | Score (0-3) | Evidenze | Metrica quantitativa | Bisogno indiretto |
|---|---|---|---|---|---|
| 1 | Overprocessing | [X] | [evidenza] | [step a valore / totali = X%] | Sì |
| 2 | Waiting | [X] | [evidenza] | [% tempo in attesa = X%] | Sì (principale) |
| 3 | Overproduction | [X] | [evidenza] | [% report 0 views = X%] | Indirettamente |
| 4 | Defects | [X] | [evidenza] | [rework rate = X%] | Sì |
| 5 | Motion | [X] | [evidenza] | [% tempo meeting = X%] | No |
| 6 | Inventory | [X] | [evidenza] | [% licenze inutilizzate = X%] | Indirettamente |
| 7 | Transport | [X] | [evidenza] | [N handoff end-to-end] | Sì |
| 8 | Unused Talent | [X] | [evidenza] | [% senior su operativo = X%] | No |
| 9 | Perfection Trap | [X] | [evidenza] | [rilasci/90gg = N] | Sì |

WASTE SCORE TOTALE: [somma]/27

TOP 3 MUDA PER IMPATTO:
1. [Muda X] (score [N]) — impatto su: [quale dimensione DLI] — bisogno indiretto: [sì/no]
2. [Muda Y] (score [N]) — impatto su: [quale dimensione DLI] — bisogno indiretto: [sì/no]
3. [Muda Z] (score [N]) — impatto su: [quale dimensione DLI] — bisogno indiretto: [sì/no]

NOTA DI LETTURA (v2.1):
I muda con bisogno indiretto "Sì" hanno PRIORITÀ DI INTERVENTO perché
eliminandoli si elimina anche il lavoro di trazione (status update,
escalation, dashboard di tracking, ecc.). Doppio dividendo.
```

Dopo il Muda Assessment, prosegui con Step 4 (Calcolo DLI) nel file
`references/assessment-dli.md`.
