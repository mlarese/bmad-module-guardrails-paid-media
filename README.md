# Guardrails Paid Media (`gpm`)

Sette figure di presidio su paid media, SEO, design, privacy, legale, social content e creative video, più `grl-ads` per audit, piani, tracking e preflight paid, `grl-social` per il contenuto organico, `grl-social-creative` per gli asset e `grl-automation` per i passaggi ripetitivi. Dalia tiene la spesa sotto controllo: nessuna campagna o creatività si pubblica senza evidenze, approvazione e rollback.

Modulo BMad. È una porzione del bundle [Guardrails](https://github.com/mlarese/bmad-module-guardrails):
stesse figure, stesso comportamento, solo l'area paid media.

> **Generato.** Questo repository è prodotto da `tools/build_modules.py` nel
> repository [bmad-module-guardrails](https://github.com/mlarese/bmad-module-guardrails).
> Le modifiche si fanno lì e poi si rigenera: qui vengono sovrascritte.

## Figure

| Figura | Ruolo | Skill | Cosa presidia |
| ------ | ----- | ----- | ------------- |
| 🛡️ Vera | Data Protection Officer | `grl-agent-privacy` | Parte sempre dai dati concreti — quali dati personali esattamente, chi li vede, per quanto tempo — e separa l'obbligo GDPR vero dalla prassi diffusa: base giuridica di una… |
| ⚖️ Aldo | Tech Lawyer | `grl-agent-legal` | Traduce licenze open source (GPL, AGPL, MIT), proprietà intellettuale del codice — anche quello generato dall'AI — contratti e DPA con i fornitori, termini di servizio e vincoli… |
| 👁️ Iris | Design Critic | `grl-agent-ui-critic` | Guarda una landing o una schermata e dice subito dove l'ha già vista: hero centrato in gradiente, tre card con icona, Inter a peso 600, blu-viola ovunque. |
| 🔎 Nora | SEO Strategist & Search Systems Auditor | `grl-agent-seo` | Distingue domanda, intento, crawl, indicizzazione, contenuto, dati strutturati e misurazione, verifica sempre live le regole SEO e trasforma ogni diagnosi in una modifica… |
| 📣 Dalia | Media Manager & Paid Advertising Strategist | `grl-agent-ads` | Trasforma un obiettivo commerciale in campagne pagate misurabili: Google Ads, Search, Performance Max, Display, YouTube e social ADV entrano solo con destinatario, offerta,… |
| 📱 Sofia | Social Media & Content Strategist | `grl-agent-social` | Trasforma obiettivi e pubblico in strategia social organica, rubriche, calendari, post, caption e metriche verificabili; separa sempre contenuto, paid media, diritti e consenso e… |
| 🎬 Marco | Advertising Creative Director & Short-form Video Producer | `grl-agent-creative` | Trasforma brief in concept pubblicitari, design, script, storyboard, shot list e specifiche producibili per post, Reel, TikTok e Shorts, con gate espliciti su claim, diritti,… |

## Skill e workflow

| Skill | Comando | Cosa fa |
| ----- | ------- | ------- |
| `gpm-profile` | Profila il progetto | Raccoglie in pochi minuti gli otto campi che danno contesto a tutte e sette le figure, criticità inclusa. |
| `gpm-profile` | Aggiorna il profilo | Riallinea il profilo quando il progetto cambia, e dice se il cambiamento invalida rischi già accettati. |
| `gpm-board` | Convoca il collegio | Fa leggere lo stesso artefatto alle sole figure pertinenti e restituisce un riepilogo unico, conflitti compresi. |
| `gpm-board` | Rischi già accettati | Mostra, raggruppato per figura, quello che il progetto ha consapevolmente scelto di accettare. |
| `gpm-board` | Gate di rilascio | Verifica una release identificata e restituisce GO, GO_CON_CONDIZIONI, NO_GO o EVIDENZA_INSUFFICIENTE. |
| `grl-ads` | Audita account e campagne | Legge export e report, definisce il perimetro e ordina blocchi, distorsioni e opportunità senza modificare l'account. |
| `grl-ads` | Prepara un piano media | Dall'obiettivo alla struttura delle campagne, agli asset, al budget come scenario e al piano di misura. |
| `grl-ads` | Verifica tracking e consenso | Mappa eventi, conversioni, tag, fonte, consenso e verifiche senza caricare dati personali. |
| `grl-ads` | Ottimizza con change set | Confronta periodi compatibili e propone modifiche a campagne e budget con soglie, approvazione, dry-run e rollback. |
| `grl-ads` | Preflight della campagna | Controlla tracking, destinazione, claim, asset, policy, consenso, budget, autorizzazioni e rollback prima dell'azione. |
| `grl-ads` | Applica un change set | Esegue solo un'azione esplicitamente autorizzata, delimitata e validata; altrimenti resta in awaiting_approval o blocked. |
| `grl-social` | Prepara un piano editoriale | Dall'obiettivo a pubblico, pilastri, rubriche, calendario, CTA, owner e piano di misura senza inventare contesto. |
| `grl-social` | Crea un contenuto social | Produce post, caption o brief di contenuto con hook, formato, CTA, fonti, accessibilità e stato di review. |
| `grl-social` | Audita i canali social | Legge calendario, contenuti ed export, separa osservato e ipotesi e ordina finding senza promettere crescita. |
| `grl-social` | Misura i contenuti social | Confronta solo dati compatibili e produce ipotesi testabili con metrica, finestra, soglia e criterio di stop. |
| `grl-social` | Valida i contenuti social | Controlla destinatario, formato, copy, CTA, fonti, diritti, privacy, accessibilità, owner e stato prima della programmazione. |
| `grl-social-creative` | Prepara il brief creativo | Rende producibili obiettivo, destinatario, canale, placement, messaggio, asset, CTA, vincoli e approvazioni. |
| `grl-social-creative` | Produci il pacchetto creativo | Consegna concept, hook, script, storyboard, shot list e specifiche per l'asset senza montaggio o upload. |
| `grl-social-creative` | Adatta un asset social | Adatta un pacchetto a un canale, rapporto, durata o placement dichiarando cosa cambia e cosa resta invariato. |
| `grl-social-creative` | Valida il pacchetto creativo | Controlla producibilità, hook, claim, diritti, privacy, accessibilità, specifiche e approvatore senza dichiarare pubblicazione. |
| `grl-automation` | Instrada un'automazione | Classifica lo scenario, sceglie agenti e workflow BMad e dichiara capability mancanti, scope e approvazioni, includendo social/content e creative video. |
| `grl-automation` | Prepara un piano eseguibile | Costruisce passi idempotenti con input, output, precondizioni, rischio, approvazione e rollback. |
| `grl-automation` | Esegui controlli read-only | Raccoglie evidenze e confronti riproducibili senza modificare sistemi esterni. |
| `grl-automation` | Prepara un dry-run | Genera e valida diff o payload senza spendere, pubblicare o applicare side effect. |
| `grl-automation` | Esegui dopo approvazione | Applica solo lo scope approvato, registra prima/dopo e osserva il risultato; in caso di errore attiva il rollback. |
| `grl-automation` | Riprendi un'automazione | Riprende un run esistente dal primo passo non concluso senza duplicare scritture o side effect. |

## Installazione

```
bmad install gpm
```

Poi, come primo passo, `gpm-profile`: raccoglie il profilo di progetto — settore,
dati trattati, mercato, stack, criticità — e da lì ogni figura deriva quanto essere
severa. Senza profilo il default resta `normal` e le figure partono senza contesto.

## Memoria condivisa

Il profilo vive in `{project-root}/_bmad/memory/grl-shared/project-profile.md`, insieme
a `decisions.md` e `accepted-risks.md`. Il percorso è lo stesso per tutti i moduli
Guardrails: installandone due, il profilo resta uno solo e si compila una volta.

## Convivenza con il bundle

Questo modulo installa skill con **lo stesso nome** del bundle `grl` — `grl-agent-privacy`
sta identica in entrambi. Bundle e moduli tematici non vanno installati insieme nello
stesso progetto: si sceglie il bundle completo, oppure i moduli delle aree che servono.

## Licenza

MIT.
