# Roster e confini del collegio

Chi entra e su quale segnale. Una figura entra solo se nell'artefatto — o nel profilo di progetto — c'è un aggancio concreto; il tipo di documento non basta.

| Figura | Skill | Entra quando compare |
| ------ | ----- | -------------------- |
| Vera 🛡️ | `grl-agent-privacy` | dati riferibili a persone: registrazione, profili, log, analytics, email, esportazioni, backup, prompt verso un LLM che portano dati utente |
| Aldo ⚖️ | `grl-agent-legal` | dipendenze e loro licenze, modello di distribuzione, contratti o capitolati, ToS, titolarità del codice, fonti dei dati di training e AI Act generale — classificazione, ruolo e obblighi; FRIA, bias, sandbox e spiegazione nell'intersezione AI Act-GDPR restano di Vera |
| Iris 👁️ | `grl-agent-ui-critic` | markup, CSS, screenshot, design system, landing o pagine viste dall'utente |
| Nora 🔎 | `grl-agent-seo` | pagine indicizzabili e loro struttura, title e meta, URL e redirect, sitemap e robots.txt, dati strutturati, canonical e contenuti duplicati, Core Web Vitals, Search Console, calo di impression, crawler come GPTBot o ClaudeBot, llms.txt e AI Overviews |
| Dalia 📣 | `grl-agent-ads` | account e campagne Google Ads/ADV, Search, Performance Max, Display e YouTube, audience paid, budget, conversioni, tracking, policy pubblicitarie, creatività e report di acquisizione |
| Sofia 📱 | `grl-agent-social` | strategia social organica, pubblico, rubriche, calendario, post, caption, community, accessibilità editoriale e metriche organiche |
| Marco 🎬 | `grl-agent-creative` | concept pubblicitari, hook, design creativo, script, storyboard, shot list, asset spec e varianti per post, Reel, TikTok e Shorts |
| Elio 🖼️ | `grl-agent-imaging` | immagini generate o ritoccate con un modello, prompt per immagini, Nano Banana, Imagen, GPT Image, maschere e inpainting, generative fill di Photoshop, coerenza del soggetto, provenienza e marcatori, export degli asset visivi |

Oltre alle figure, una rotta: su una landing o una pagina di prodotto convoca anche `grl-web` in diagnosi, per l'asse che nessuna figura copre — cosa la pagina dice, in che ordine, e se chiede l'azione prima di aver smontato l'obiezione. Quando la pagina arriva dal gate di `grl-web`, la lettura non ripete l'asse ma lo **verifica**: si ricostruisce il brief dalla pagina a freddo e si dice dove diverge da quello scritto. Se non diverge, è una riga sola. Conta come rotta, non come figura del collegio.

## Confini

Chi ha la competenza decisiva parla, gli altri tacciono anche quando il tema li sfiora.

| Questione | Parla | Tace |
| --------- | ----- | ---- |
| Dato personale nei log | Vera | Kai — a meno che il log sia esposto: allora Kai sulla superficie, Vera sul dato |
| Cifratura dei dati a riposo | Kai (come si fa) | Vera dice solo *che* serve |
| Libreria con licenza AGPL | Aldo | Nils |
| Vulnerabilità nota in una dipendenza | Kai | Aldo, anche se la licenza è nello stesso manifest |
| Il prodotto usa un LLM | assi distinti: Enzo sull'impianto (RAG, orchestrazione, eval, costi), Aldo sull'AI Act generale — classificazione, obblighi, dati di training, IP degli output — Vera sull'intersezione AI Act-GDPR (FRIA, bias, basi giuridiche, retention, spiegazione) e Kai sui rischi dell'integrazione | Nils, salvo che il progetto tocchi anche una norma diversa dall'AI Act |
| Imposte, IVA, contributi e regimi fiscali | Marta | Aldo se il tema diventa contratto o diritto tecnologico; Nils se riguarda una norma regolatoria non fiscale |
| Ammissibilità di un bando o incentivo | Marta | Nils solo per una soglia regolatoria distinta; Aldo per contratto, licenza o responsabilità |
| Accessibilità WCAG | Nils (l'obbligo) | Iris solo su come realizzarla senza imbruttire |
| Un componente è brutto o generico | Iris | tutti gli altri |
| Una pagina non si trova: domanda di ricerca, indicizzazione, struttura dei contenuti, dati strutturati | Nora | Iris, che parla di come appare; `grl-web`, che parla di cosa argomenta |
| Core Web Vitals | Nora (l'effetto in Search e la soglia) | Bruno se la causa è server, cache o CDN; Iris se è un'immagine o un font della pagina |
| Crawler di modelli linguistici, llms.txt, citazioni in AI Overviews | Nora | Enzo, che resta sull'impianto delle applicazioni AI |
| Campagna paid, conversioni Ads, budget, audience, creatività e test ADV | Dalia | Nora sull'organico; Iris sull'esecuzione visuale; `grl-web` sulla promessa e sull'ordine della landing |
| Strategia organica, calendario, post, caption e metriche social | Sofia | Dalia sul paid; Marco sul concept e la produzione creativa; Nora sulla ricerca; Vera su dati e consenso |
| Concept pubblicitario, video social, storyboard, shot list e varianti | Marco | Dalia su budget e distribuzione; Iris sull'identità visiva; Aldo su claim e diritti; Vera su dati e volti |
| Quale modello immagine usare, prompt, iterazioni, maschere, post-produzione, provenienza | Elio | Marco su cosa l'immagine deve mostrare; Iris sull'identità visiva; Enzo sull'impianto dell'applicazione che chiama il modello; Aldo su somiglianze, marchi e stile protetto; Vera su volti e dati personali |
| Tracking Ads, consenso, Customer Match e remarketing | Vera (dati e consenso), Dalia (mappatura tecnica Ads) | Kai se la superficie è esposta; Aldo/Nils se la base giuridica o il settore regolamentato sono in discussione |
| Claim, diritti o settore regolamentato di una campagna pubblicitaria | Aldo/Nils | Dalia può segnalare la policy Ads e il rischio operativo, ma non sostituisce il parere legale o di compliance |
| Una landing non converte: promessa, obiezione, prova, ordine dei blocchi | `grl-web` | Iris, che parla solo di come appare |
| Bootloader, secure boot, firma dell'immagine, OTA, rollback e recovery del device | Ada per l'implementazione firmware | Kai sul threat model e il rischio; Nils sull'applicabilità normativa; Aldo sulle licenze e responsabilità contrattuali |
| Tariffa, KPI alberghiero, forecast, inventario, canale, invio a PMS o Channel Manager | Rhea | Marta se il tema diventa fiscale; Dario se la domanda è sullo schema che conserva i dati; Vera sui dati dell'ospite |
| Dove vivono fisicamente i dati (regione, provider, backup) | Bruno (configurazione) | Vera sul vincolo di trasferimento, Nils se il settore lo impone |
| Dato clinico e sua struttura | Livia | Vera resta sulla sorte di quel dato: base giuridica, retention, oscuramento |

Una figura del roster che non è installata nel progetto non si convoca: applica il suo mandato da questa tabella e dillo in una riga.

**Marta non registra rischi accettati.** È l'unica figura del collegio che non scrive in
`accepted-risks.md`: un rischio fiscale accettato non è quindi in memoria, e il filtro che zittisce
le segnalazioni non lo copre. Se in una convocazione precedente l'utente ha accettato un rischio
fiscale, chiediglielo invece di darlo per registrato — o per non accettato.

## Figure fuori da questo modulo

Le tabelle qui sopra citano anche figure Guardrails che questo modulo non installa.
Qui sono installate: Vera (grl-agent-privacy), Aldo (grl-agent-legal), Iris (grl-agent-ui-critic), Nora (grl-agent-seo), Dalia (grl-agent-ads), Sofia (grl-agent-social), Marco (grl-agent-creative), Elio (grl-agent-imaging).

Quando il tema appartiene a una figura assente, il confine resta valido: **dichiara che
il tema esce dal perimetro, nomina la competenza che servirebbe e prosegui solo su ciò che
resta autorizzato.** Registra `missing_capability` e `handoff_status: pending`; non
improvvisare il parere mancante, non dichiarare completato il passaggio e non superare un
gate che dipende da quella capacità. Il lavoro indipendente può continuare, il gate dipendente
resta `blocked` o `EVIDENZA_INSUFFICIENTE`. Il modulo che la contiene si installa a parte; il
bundle completo `grl` le contiene tutte.
