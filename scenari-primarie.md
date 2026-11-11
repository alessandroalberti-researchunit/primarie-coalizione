# Primarie del centrosinistra: scenari di fattibilità (Milano 2027 e candidato di coalizione)

> Documento di lavoro dell'11 novembre 2026. Le sezioni 7 e seguenti, in fondo, riportano le decisioni prese dopo la stesura e prevalgono sulle parti precedenti: gli scenari sono ora due (A e B) e non tre, il ballottaggio è escluso e le due primarie si tengono lo stesso giorno. Non è un parere legale. I punti marcati INF sono inferenze da validare con un legale.

Data di redazione: 11 novembre 2026. Bozza di lavoro, non parere legale.

## 0. Come leggere questo documento

- **Assunzione sulla data**: voto che chiude domenica 31 gennaio 2027 (81 giorni da oggi, calcolo Python). Da confermare.
- **Livelli di evidenza**: [DOC] testo ufficiale letto in estratto o per intero dall'agente di ricerca; [SEC] solo stampa o Wikipedia; [INF] inferenza mia, da validare.
- **Limite generale**: molti regolamenti esteri sono stati letti via estratti riassunti dal tool web, quindi vanno recuperati nei PDF originali prima di citarli in una proposta formale. Letti per intero dal PDF: regolamento Italia Bene Comune 2012 e regolamento Roma 2016 (copia su sito privato). Letto per intero anche il regolamento quadro dell'Unione 2005 (PDF dell'Associazione dei costituzionalisti, 4 pagine). Non sono stati letti: Charter DNC, regole DNC 2028, linee guida NEC del Labour per i sindaci, regolamento NDP 2026, statuto Labour neozelandese, i due regolamenti attuativi dell'Unione 2005 (autodisciplina e svolgimento della campagna), regolamenti di Milano 2011 e 2016 (cercati nel web e nell'archivio web: il PD risponde 403, l'archivio web è offline; di Milano 2016 ho il testo degli artt. 9 e 13 riprodotto da una testata locale e il regolamento quasi identico di Roma), Belle Alliance Populaire 2017. L'analisi di Croce (2011) sui regolamenti delle grandi città, compreso Milano 2011, è letta per intero ma è un commento, non il testo.
- **Correzioni rispetto al primo giro di ricerca**: nel testo 2012 non compaiono né la clausola sulle "procedure distinte" tra registrazione e voto né le 20.000 firme dei candidati, che l'agente aveva riportato da una fonte secondaria. Vanno considerate non verificate.
- Tutti i numeri di giorni sono calcolati con script Python (`scratchpad/dates.py`).

## 1. Cosa dicono i casi (sintesi comparata)

| Caso | Chi vota | Registrazione e quota | Chiusura registrazione, giorni prima della chiusura del voto | Canali | Verifica identità | Evidenza |
|---|---|---|---|---|---|---|
| Labour 2020 | Iscritti, affiliati, sostenitori | Sostenitori: 3 giorni di finestra (14 16 gen), 25 sterline, freeze dell'elettorato il 20 gen | 77 | Email, posta se manca email (Civica) | Iscrizione alle liste elettorali; esclusi sostenitori di altri partiti negli ultimi 2 anni | DOC |
| Labour 2016 | Come sopra, freeze degli iscritti a 6 mesi | 25 sterline, 3 giorni | 63 | Posta con reinvio elettronico | Liste elettorali; ricorso Evangelou, appello a favore del partito | DOC |
| Labour 2015 | Come sopra | 3 sterline, finestra fino al giorno 12 agosto | 29 | Email o posta | Verifica da 6 membri NEC; respinti 3.138 a fine agosto, circa 56.000 a consuntivo secondo Wikipedia (non conciliabili, nessun dato ufficiale) | DOC e SEC |
| Labour regole 2025 | Solo iscritti e affiliati, 6 mesi di iscrizione | Sostenitori registrati assenti dal testo | Decide il NEC | Preferenziale | Lo scrutineer approva la lista | DOC |
| Liberali canadesi 2025 | Registered Liberals, 14+ | Gratuita | 41 | Online, telefono su autorizzazione, anticipato 11 giorni | Identity+ di Canada Post o ufficio postale, patente o ID provinciale; verifica tra il 20 feb e il 7 mar | DOC |
| NDP 2026 | Iscritti | n.d. | circa 59 | Online, telefono, posta, congresso | Non trovata | SEC |
| ALP (Australia), cl. 42 community preselections | Soci con quota, oppure elettori iscritti alle liste elettorali del collegio | Non iscritti: dichiarazione firmata di essere sostenitori Labor e di non appartenere ad altri partiti | n.d. | n.d. | Iscrizione alla commissione elettorale (AEC) | DOC |
| Democrats Abroad 2024 | Cittadini USA all'estero che votano come Democratici | L'iscrizione è la registrazione, anche il giorno stesso | 0 | Presenza, posta, fax, email firmata, nessuna piattaforma web | Dichiarazione firmata contro database interno; in centro documento o giuramento | DOC |
| Regole DNC 2024, Rule 2.G | Dichiarazione pubblica di preferenza | Nessuna quota | n.d. | Internet solo come alternativa a presenza o posta, con piano di sicurezza e traccia cartacea | Da piano approvato | DOC |
| Iowa 2024 | Registrati come Democratici | Entro il 19 febbraio | 15 | Solo posta | Confronto con il voter file, nessun ID | DOC |
| SPD 2019 | Iscritti, ospiti esclusi | Nessuna quota | 36 (registrazione online per scegliere il canale) | Online e posta | Link monouso, PIN, dichiarazione giurata per la posta | DOC |
| PSOE 2027 | Solo militanti, censo chiuso 48 giorni prima | Quote regolarizzabili fino a 3 giorni prima | 48 | Solo presenza | DNI, passaporto, patente, NIE | DOC (copia giornalistica) |
| PS Portogallo 2026 | Militanti e simpatizzanti con 6 mesi | Contributo unico | 22 | Solo urna | Documento oppure due militanti; piattaforma con doppia identificazione | DOC |
| Italia Bene Comune 2012 (regolamento 19 ott 2012, letto per intero) | Maggiorenni che sottoscrivono l'Appello e dichiarano di riconoscersi nella Carta d'intenti; cittadini UE residenti e stranieri con permesso e carta d'identità (art. 3.1 3.2) | Iscrizione all'albo dal 4 al 25 novembre, almeno 2 euro, presso sedi decise dal Coordinamento provinciale (art. 3.3). Il certificato di elettore ha un cedolino per ogni giornata di voto, trattenuto al seggio contro il doppio voto (art. 10.2 10.3) | 0 (la finestra comprende il giorno del voto, 21 giorni di durata) | Solo seggi, nel seggio della propria sezione elettorale (art. 3.6). Nessun voto online nel regolamento | Documento, tessera elettorale e certificato di elettore (art. 10.1) | DOC |
| Roma 2016, sindaco (regolamento del Comitato Promotore, letto per intero) | Titolari dell'elettorato attivo a Roma; stranieri residenti e 16 enni con iscrizione preventiva entro il 3 marzo, cioè 3 giorni prima del voto del 6 marzo (art. 9) | Per gli altri nessuna registrazione anticipata: firma delle Linee guida, almeno 2 euro e consenso all'inserimento nell'albo al seggio il giorno stesso (art. 13) | 0 per la maggior parte degli elettori, 3 per le categorie con iscrizione preventiva | Solo seggi. Registro al seggio dei votanti | Documento con foto che indichi la residenza e/o il certificato elettorale (art. 13.a.1) | DOC (copia ospitata su un sito privato, non sul sito ufficiale) |
| Milano 2016 (6 7 febbraio) | Residenti a Milano (non basta il domicilio), 16+, stranieri residenti. Firma delle Linee guida del centrosinistra per Milano | Iscrizione all'Albo "entro il 7° giorno antecedente" il voto presso le sedi dei partiti del Comitato promotore, con documento con foto e residenza, almeno 2 euro, consenso al trattamento. Dal 18 gen al 2 feb si potevano compilare online i moduli da compilare ai seggi, che non è un voto online | 7 giorni (come scritto nel testo) per l'iscrizione all'Albo | Seggi (150) | Documento con foto che indichi la residenza e/o il certificato elettorale | SEC (la guida di MilanoToday dell'8 gennaio 2016 riproduce quasi alla lettera gli artt. 9 e 13, e coincidono con il regolamento di Roma. Il PDF ufficiale non è stato trovato) |
| Milano 2011 (voto 14 nov 2010) | Come sopra, giovani che compiono 16 anni entro le comunali (art. 7) | Registrazione negli elenchi di norma al momento del voto, contributo di 1 2 euro nei regolamenti analizzati | 0 (di norma al seggio) | Seggi | Documento e, ove previsto, certificato | SEC (analisi accademica di Croce 2011, 21 articoli, 4.369 parole; regolamento non letto) |
| Unione 2005, regolamento quadro (11 luglio 2005, letto per intero) | Cittadini con elettorato attivo per la Camera che sottoscrivono il Progetto dell'Unione e versano un contributo; stranieri residenti a discrezione dell'Ufficio di Presidenza (art. 6.1 6.3) | Contributo non quantificato nel quadro (1 euro minimo secondo Rubechi, SEC); consenso all'inserimento in un elenco dei partecipanti consultabile da chiunque abbia interesse (art. 6.2) | Non fissata nel quadro | Seggi. L'Ufficio tecnico predispone "strumenti informatici per l'eventuale svolgimento per via telematica" (art. 4.1) e le schede possono essere "in formato cartaceo o informatico" (art. 7.5) | Documento e tessera elettorale (art. 6.2) | DOC |
| PD 2023 | Iscritti esenti, non iscritti con albo | 2 euro per i non iscritti | n.d. | Gazebo, online solo per categorie limitate | Documento e tessera elettorale | SEC |
| Primaire populaire 2022 | Chiunque 16+ | Gratuita, chiusa 23 gen | 7 (voto fino al 30 gen) | Solo online | Email, telefono, carta di pagamento (Neovote); 120.000 verificati su 300.000 al 10 gen | SEC |

Lezioni che ricorrono:
1. Il collo di bottiglia è la verifica di massa, non il voto (Labour 2015, Canada, Francia) [DOC e SEC].
2. Un congelamento retroattivo dell'elettorato è stato ritenuto legittimo in UK, e resta un rischio di contenzioso [DOC].
3. Il voto online si regge solo con un canale alternativo e una traccia verificabile (regola DNC 2.G, Iowa 2020, Rousseau 2019) [DOC].
4. Nelle primarie di coalizione l'albo con firma di un testo politico è lo strumento di legittimazione (Unione 2005, 2012, Milano 2016) [SEC].
5. La registrazione tardiva e il ballottaggio sono stati la parte più contestata nel 2012 [SEC].

### Governance dei comitati promotori (dai testi italiani letti)

Il regolamento di Roma 2016 è l'unico testo letto per intero costruito attorno a un Comitato Promotore di più forze politiche, come nel tuo caso [DOC].
- **Organi**: Comitato Promotore (responsabili designati dalle forze politiche, coordinato dal segretario regionale del PD), che nomina un Coordinamento Organizzativo (fino a 10 persone) e il Tesoriere. Il Coordinamento nomina il Collegio dei Garanti (5 persone "di comprovata autorevolezza") e un Comitato per il programma (art. 1). Nel 2012 era il Collegio dei garanti a nominare un Coordinamento di quattro persone indicate dai partiti, con coordinamenti regionali e provinciali che includono un componente per partito (art. 1.d, 4, 5). Nel 2005 il Comitato dei responsabili dei partiti nomina un Ufficio di Presidenza (un rappresentante per partito), che nomina 5 garanti e un Ufficio tecnico-amministrativo con tanti membri quanti i partiti (art. 2) [DOC]. Per Milano 2011 un'analisi accademica descrive quattro organi: Comitato Promotore (segretari delle forze che sottoscrivono), Comitato Organizzativo (fino a 27 componenti, con tutte le forze rappresentate), Comitato Esecutivo (9 membri) e Collegio di Garanzia (3 5 membri nominati dal Promotore, senza intervento dell'Organizzativo) [SEC].
- **Incompatibilità**: le cariche di Comitato Promotore, Coordinamento e Garanti sono incompatibili tra loro e con la candidatura (Roma, art. 5).
- **Candidature**: a Roma 2.000 2.500 firme di elettori, raccolta dal 30 gennaio, deposito entro il 10 febbraio, ammissione entro 24 ore, ricorso in 2 giorni, decisione in 2 giorni (art. 7 8). Nel 2005 servivano almeno 10.000 firme, in almeno 10 regioni con almeno 1.000 firme ciascuna (500 nelle regioni sotto il milione di abitanti) [DOC, art. 5.2]. Il tetto di 20.000 compare solo in fonti secondarie. Per il 2012 le firme erano in un atto separato che non ho letto. I candidati firmano adesione alle linee guida, codice di comportamento e impegno a sostenere il vincitore (Roma, art. 7.c, clausola compromissoria art. 18; 2012 art. 15).
- **Tempi dei ricorsi**: 24 ore per i reclami sul voto, 24 ore di decisione, 48 ore per il risultato (Roma, art. 19); nel 2012 48 ore in prima istanza e 24 più 24 ore per i risultati (art. 2.c, 13.7).
- **Tetti di spesa**: 30.000 euro per candidato (Roma 2016), 300.000 euro con tetto di 10.000 per singolo contributore (2005 [SEC]).
- **Doppio voto**: nel 2012 il cedolino di giornata staccabile dal certificato di elettore. Roma usa un registro al seggio. Nessuno dei due testi prevede il voto online, quindi la gestione del doppio voto tra online e presenza resta da progettare [INF].
- **Privacy**: il 2005 prevedeva un elenco dei partecipanti consultabile su richiesta, il 2012 un albo con modulo di autorizzazione al trattamento dati (art. 6.2), Roma il consenso alla consultazione dell'albo da parte del Comitato (art. 13.a.3). L'albo è informatizzato dopo il voto, per decisione del Comitato (Roma, art. 22.3). Il Garante nel 2012 ha escluso la diffusione online [SEC].
- **Esclusioni**: nel 2012 chi svolge attività politica in contrasto con la Coalizione (art. 3.7), a Roma gli eletti di coalizioni avverse (art. 9.c).

## 2. Canale ibrido comune a tutti gli scenari

- **Online**: autenticazione con SPID e CIE tramite aggregatore privato (AgID, determina 71/2022 [SEC]). Tempi e tariffe vigenti non verificati. Se l'aggregatore non è attivo entro il 7 dicembre, la finestra di registrazione slitta [INF].
- **Presenza**: seggi nel weekend finale (sabato 30 e domenica 31 gennaio).
- **Registro unico dei votanti** con stato "ha già votato" aggiornato in tempo reale tra online e seggi. Il registro contiene lo stato, mai il voto [INF, coerente con Rousseau 2019]. In alternativa, scelta del canale in fase di registrazione (modello SPD 2019).
- **Documenti ai seggi**: la carta d'identità cartacea è prorogata solo fino al 31 gennaio 2027 dal D.L. 108/2026, art. 11, per i rapporti con la PA e simili. Le iniziative private non sono citate [DOC sulla notizia, testo di legge non letto]. Il voto cade proprio sulla scadenza, quindi il regolamento deve fissare un elenco chiuso di documenti ammessi (CIE, passaporto, patente) [INF].
- **Sicurezza**: audit indipendente prima dell'apertura, DPIA, fornitore nominato responsabile del trattamento, separazione tra identità e voto, credenziali nominative [DOC, provvedimento Garante 2019 su Rousseau].
- **Base giuridica**: l'art. 9.2.d del GDPR copre membri e persone in contatto regolare, quindi un comitato aperto ha più probabilità di dover raccogliere consenso esplicito [INF, da verificare con un legale].
- **Quota**: i precedenti sono 2 euro (2012, Milano 2016, PD 2023). Applicabilità della L. 3/2019 a un comitato non verificata.
- **Carta dei valori firmata** e riconoscimento dei risultati da parte dei candidati (art. 15 del regolamento 2012) [SEC].

## 3. Scenari sull'elettorato e le tempistiche

Calendario comune di partenza (giorni calcolati): regolamento approvato lunedì 30 novembre (19 giorni da oggi, 62 giorni dal voto). Voto online da venerdì 22 gennaio (9 giorni). Seggi sabato 30 e domenica 31 gennaio. Audit concluso entro il 15 gennaio (16 giorni dal voto).

### Scenario A: basta l'iscrizione a uno dei partiti della coalizione

- **Elettorato**: iscritti ai partiti aderenti al 30 novembre. Nessuna registrazione al comitato, solo la conferma del canale e dell'identità.
- **Calendario**: freeze 30 nov (62 giorni prima del voto). Liste certificate dai partiti entro il 15 dic. Controllo dei doppi iscritti e conferma del canale entro il 10 gen. Voto online 22 31 gen, seggi 30 31 gen.
- **Precedenti**: SPD 2019, PSOE 2027, Labour 2025, leader ALP [DOC].
- **Punti di forza**: è lo scenario più rapido, con tempi ampiamente sufficienti. Il freeze è già stabilito e riduce il rischio di infiltrazione.
- **Criticità**:
  - È una primaria chiusa. Se l'obiettivo è l'apertura alla società civile, non serve allo scopo [INF].
  - I partiti devono fornire liste affidabili. Non ho trovato dati sulla qualità dei registri degli iscritti dei partiti italiani, quindi resta da verificare [INF].
  - La comunicazione delle liste a terzi richiede consenso scritto secondo il Garante del 2014 [DOC, estratto].
  - Il peso dei partiti dipende dal numero di iscritti, non dal consenso. Rischio di contestazione dai partiti più piccoli [INF].
  - Il congelamento retroattivo è stato contestato in Evangelou e poi confermato in appello [DOC].

### Scenario B: serve iscriversi al comitato, anche per gli iscritti ai partiti

- **Elettorato**: chiunque si registri all'albo del comitato, firmando la Carta dei valori, con quota di 2 euro. Gli iscritti ai partiti non hanno corsia preferenziale.
- **Calendario**: apertura registrazione lunedì 7 dic (26 giorni da oggi), chiusura domenica 10 gen (21 giorni prima della fine del voto, registrazione di 34 giorni). Verifica dal 10 al 22 gen (12 giorni). Voto online dal 22 gen (9 giorni). Seggi 30 31 gen.
- **Confronto con i casi**: 21 giorni di anticipo di chiusura sono meno dei 41 canadesi e dei 63 77 del Labour, più dei 5 di Milano 2016. Con 14 giorni (chiusura il 17 gen) restano solo 5 giorni di verifica prima dell'online. Con 28 giorni (chiusura il 3 gen) la registrazione dura 27 giorni.
- **Precedenti**: Italia Bene Comune 2012 e Roma 2016 [DOC], Milano 2016, Registered Liberals, Democrats Abroad. Nei testi italiani l'albo si compila di persona, fino al giorno del voto (2012) o al seggio (Roma). A Milano 2016 era prevista l'iscrizione all'Albo entro il 7° giorno prima del voto presso le sedi dei partiti, e a Bologna 2011 l'iscrizione negli "elenchi degli elettori" nei tempi decisi dal Comitato organizzatore [SEC, Croce]. Nessun testo letto prevede il voto online, quindi non esiste un precedente italiano di albo chiuso prima di un voto ibrido. Il quadro del 2005 contemplava però lo strumento telematico (art. 4.1 e 7.5).
- **Punti di forza**: è il modello più coerente con primarie di coalizione, perché mette tutti sullo stesso piano e ha già un precedente italiano. Produce un albo unico, utile contro i doppi voti.
- **Criticità**:
  - La verifica di massa è il punto debole (Canada: problemi con l'app; Francia: 120.000 verificati su 300.000 a pochi giorni dal voto) [SEC].
  - L'aggregatore SPID deve essere operativo entro il 7 dicembre. Non ho fonti sui tempi reali [INF].
  - Gli iscritti ai partiti devono accettare di registrarsi, e questo può abbassare la partecipazione [INF].
  - Chi si registra in loco ai seggi (variante come DA e 2012) può votare solo in presenza, e le carte cartacee sono a rischio [INF].
  - Albo da trattare come dato particolare (opinione politica), non pubblico (Garante, 2012 [SEC]).

### Scenario C: ibrido, iscritti con corsia veloce e non iscritti con registrazione

- **Elettorato**: gli iscritti ai partiti (liste al 30 nov) confermano solo l'identità e il canale. I non iscritti si registrano all'albo, con Carta dei valori e quota.
- **Calendario**: freeze iscritti 30 nov, liste certificate 15 dic. Registrazione non iscritti dal 7 dic al 10 gen. Verifica unica fino al 22 gen. Voto come negli altri scenari.
- **Precedenti**: PD 2023 (iscritti esenti, albo per i non iscritti), PS Portogallo (militanti e simpatizzanti con registrazione separata), Labour 2015 2020 (tre categorie con voto di pari peso), ALP clausola 42 (i non iscritti votano se iscritti alle liste elettorali del collegio e firmano una dichiarazione di sostegno e di non appartenenza ad altri partiti, modello vicino alla Carta dei valori) [DOC e SEC].
- **Punti di forza**: unisce la legittimazione dei partiti e l'apertura. Alleggerisce la verifica di massa, perché gli iscritti arrivano già censiti.
- **Criticità**:
  - Due flussi di dati da fondere e deduplicare (iscritto a due partiti, iscritto che si registra anche come non iscritto) [INF].
  - Regola di pari peso o pesi diversi tra le categorie da stabilire. Il Labour usa un'unica sezione con pari peso [DOC].
  - Dipende dalla qualità delle liste dei partiti, come lo scenario A.
  - Rischio politico: una categoria di non iscritti molto numerosa decide l'esito, come a Londra 2015, dove tra gli iscritti il margine era di 964 voti e i sostenitori hanno deciso [SEC].

### Valutazione di fattibilità (giudizio mio, non misurato)

| Criterio | A | B | C |
|---|---|---|---|
| Tempi (81 giorni) | alta | media | media |
| Verifica di massa | bassa pressione | alta pressione | media pressione |
| Apertura e legittimazione | bassa | alta | alta |
| Dipendenza dalle liste dei partiti | alta | nulla | alta |
| Rischio infiltrazione | basso | medio, mitigabile con Carta dei valori | medio |
| Rischio privacy | medio | alto (albo ampio) | alto |
| Rischio di contestazione sul freeze | medio | basso | medio |

## 4. Espressione del voto

Interpreto "a capo del comitato o simili" così: il voto designa una persona che guida il comitato di coalizione. Da confermare.

- **V1, persona unica con voto preferenziale e un solo turno** (Labour, Liberali canadesi, NYC). È l'unica forma che regge con 81 giorni, perché non richiede un secondo appuntamento. Su carta il conteggio è più lento. [DOC e SEC]
- **V2, persona con soglia del 50% più uno e ballottaggio** (Italia Bene Comune 2012, PSOE). Richiederebbe di anticipare il primo turno di una settimana o due, e quindi anche le registrazioni. Nel 2012 la riapertura della registrazione al secondo turno è stata contestata [SEC]. Realistica solo con primo turno a metà gennaio [INF].
- **V3, maggioranza semplice** (Milano 2016). È la più rapida e semplice, con il rischio di un vincitore con una quota bassa [SEC, INF].
- **Variante di ponderazione territoriale**: i liberali canadesi assegnano 100 punti a ogni circoscrizione, indipendentemente dai votanti [DOC]. Per Milano si potrebbe pesare per Municipio (9 zone), come ipotesi da valutare e non come raccomandazione [INF].
- **Doppio ruolo** (sindaco di Milano e candidato nazionale): vedi domanda aperta 1.

Abbinamento che reggerebbe meglio i vincoli di tempo: V1 con A, B o C. È una proposta di lavoro e non una conclusione.

## 5. Domande aperte per te

1. **Doppio ruolo**: una sola primaria designa sia il candidato a Milano sia quello nazionale, o sono due schede? L'elettorato sarebbe milanese per la scheda locale, ma non è chiaro chi voterebbe la scheda nazionale.
2. **Data**: 31 gennaio è domenica, giorno di scadenza della proroga della carta cartacea. Si può anticipare il voto di una settimana?
3. **Chi decide il regolamento** e chi sono i garanti del comitato.
4. **Candidati**: soglie di firme o di sostegno dai partiti per candidarsi (Roma 2016: 2.000 2.500 firme di elettori; Unione 2005: 10.000 20.000 [SEC]).
5. **Quota**: gratuita o 2 euro, con le conseguenze fiscali e di trasparenza da verificare.

## 6. Lacune e verifiche da fare

- Leggere i PDF originali: regolamento Italia Bene Comune 2012, regole Milano 2016, Carta d'intenti, statuto del Labour neozelandese, regolamento NDP 2026, linee guida NEC.
- Testo del D.L. 108/2026 art. 11 e circolare DAIT 76/2025.
- Tariffe e tempi SPID e CIE per un privato tramite aggregatore (preventivo scritto).
- Verifica con un legale su: art. 9 GDPR, L. 3/2019, ammissibilità dei documenti.
- Qualità dei registri degli iscritti dei partiti coinvolti.
- Dati sui votanti per canale (online contro presenza) nei casi Labour: non trovati.

## 7. Decisioni dell'11 novembre 2026

1. Due schede nello stesso voto: candidato sindaco di Milano e candidato di coalizione nazionale.
2. Il voto chiude domenica 31 gennaio 2027.
3. Il comitato promotore dei partiti scrive il regolamento e nomina coordinamento organizzativo e garanti (modello Roma 2016).
4. Firme per candidarsi: 2.500 per la scheda di Milano, 10.000 per quella nazionale.

Domande aperte che ne derivano (formulate da me, ipotesi): chi può votare la scheda nazionale, la forma di voto per ciascuna scheda, quota di 2 euro o voto gratuito, orari dei seggi.
Calendario candidature (ipotesi mia): raccolta firme dal 1 dicembre al 5 gennaio (35 giorni), deposito il 5 gennaio (26 giorni prima del voto, Roma 2016: 25), ammissione e ricorsi entro il 12 gennaio.

## 8. Correzione dell'11 novembre 2026: due primarie distinte

Le primarie sono due, nello stesso giorno (31 gennaio 2027): una solo a Milano per scegliere il sindaco (elettori: residenti a Milano, 2.500 firme per candidarsi) e una in tutta Italia per scegliere il candidato di coalizione (elettori: tutta Italia, 10.000 firme). Un milanese compila due schede, chi vive altrove una. Questo sostituisce la formula "due schede nello stesso voto" della sezione 7 e chiude la domanda su chi vota la scheda nazionale.
Scala dei precedenti (stampa): Milano 2016, 60.900 votanti; Italia Bene Comune 2012, 3.107.568 al primo turno (circa 51 volte); Unione 2005, 4.290.388 (circa 70 volte). Rapporti calcolati con Python.
Nuove domande aperte (ipotesi mia): numero e gestione dei seggi fuori Milano; un solo comitato promotore o uno nazionale e uno milanese.

## 9. Scenario A rivisto (11 novembre 2026)

Il conteggio degli iscritti dei partiti è al 31 dicembre (non più al 30 novembre). Entro il 15 gennaio gli iscritti confermano che votano. Voto online dal 22 gennaio con SPID o CIE, seggi sabato 30 e domenica 31 gennaio. Distanze dal voto, calcolate con Python: 31 giorni dal conteggio, 16 dalla conferma. Lo scenario C resta con il blocco degli iscritti al 30 novembre, da allineare se serve.

Aggiornamento: anche lo scenario C usa il conteggio degli iscritti al 31 dicembre e la conferma del voto entro il 15 gennaio. L'albo dei non iscritti resta aperto dal 7 dicembre al 10 gennaio, con verifica fino al 22 gennaio.

Decisione: niente ballottaggio per i tempi. La forma di voto è tra preferenze in ordine e un solo nome.

## 10. Scenari B e C unificati (11 novembre 2026)

Lo scenario B assorbe l'ex C: gli iscritti ai partiti (contati al 31 dicembre) entrano automaticamente nell'albo degli elettori e entro il 15 gennaio confermano che votano, senza quota. Chi non ha tessere può iscriversi direttamente all'albo come indipendente dal 7 dicembre al 10 gennaio, con Carta dei valori, 2 euro e verifica. Restano due scenari: A (solo iscritti ai partiti) e B (albo unico). Ex scenario B (tutti si registrano, iscritti compresi) eliminato.

Precisazione: nello scenario B gli iscritti ai partiti sono automaticamente iscritti all'albo e non devono confermare nulla (nessuna conferma al 15 gennaio, nessuna quota). La conferma del voto entro il 15 gennaio resta solo nello scenario A.

## 11. Percorso ristrutturato (11 novembre 2026)

Le 8 tappe sono accorpate in 5 fasi: informazione e requisiti, iscrizione e consenso, identità e accesso, voto, risultato e ricorsi. Ogni fase ha due corsie: voter journey (cosa fa l'elettore) e system journey (cosa fanno comitato, partiti, piattaforma e seggi, con l'indicazione di chi fa che cosa).

## 12. Decisioni sui sette punti (11 novembre 2026)

1. Elenco chiuso di documenti ammessi ai seggi: deciso (quali documenti, da fissare).
2. SPID e CIE tramite aggregatore, attivo entro il 7 dicembre: confermato.
3. Residenza: CIE usata online potrebbe restituire la residenza anagrafica da ANPR (decreto 8 settembre 2022, da verificare nel manuale tecnico), SPID no (domicilio fisico attributo secondario), tessera sanitaria no. Da verificare con l'aggregatore.
4. Privacy e sicurezza: sezione dedicata nella pagina (consenso esplicito, valutazione d'impatto, audit, caso Rousseau, consensi dei partiti per gli elenchi dello scenario B).
5. Quota di 2 euro versata al tesoriere: deciso.
6. Punto sul PDF di Milano 2016: eliminato, non interessa.
7. Scala: sezione dedicata nella pagina (partecipazione dei precedenti, verifica, SPID, seggi, piattaforma). Calcoli: 406 voti per seggio a Milano 2016, circa 7.654 seggi equivalenti per 3.107.568 voti.
