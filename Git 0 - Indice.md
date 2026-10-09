# Guida Git – Indice

Una guida completa da consultare e stampare, ideata per affiancare lo studio pratico con spiegazioni teoriche, diagrammi visuali in formato **Mermaid** (ottimizzati per Obsidian) e comandi essenziali.

La guida è divisa in tre livelli:

| Livello | Nota | Contenuto |
| :--- | :--- | :--- |
| **Base** | [[Git 1 - Base]] | Uso quotidiano da soli: commit, storico, branch, GitHub, correzione degli errori |
| **Intermedio** | [[Git 2 - Intermedio]] | Versioni passate, tag, tracciabilità dei calcoli, Pull Request |
| **Avanzato** | [[Git 3 - Avanzato]] | Automazioni (hook, GitHub Actions), riscrittura dello storico, submodule, strategie di branching, struttura interna, firme |

---

> [!tip] Percorso consigliato per chi inizia
> Non serve imparare tutto subito. Procedi a tappe:
> 1. **Settimana 1:** `status`, `add`, `commit`, `log` (base, sezioni 6–8). Lavora solo in locale.
> 2. **Settimana 2:** `push`, `pull`, `clone` (base, sezioni 5 e 12). Collega GitHub.
> 3. **Settimana 3:** branch e merge (base, sezioni 10–11).
> 4. **Quando serve:** annullare errori e stash (base, sezioni 13–14).
> 5. **Passaggio all'intermedio:** tag, versioni passate e tracciabilità dei calcoli (intermedio, sezioni 1–3).
> 6. **Quando lavori con altri:** Pull Request (intermedio, sezione 4).
> 7. **Quando il progetto cresce:** pre-commit e test automatici (avanzato, sezioni 1–2), poi i workflow della sezione 8.
>
> La regola d'oro: **`git status` prima e dopo ogni comando.** Ti dice sempre dove sei e cosa sta succedendo.

---

## Livello Base

**Fondamenti**
1. [[Git 1 - Base#1. Glossario Concettuale: Che cos'è Git e come funziona?|Glossario Concettuale: Che cos'è Git e come funziona?]] – termini fondamentali e analogie
2. [[Git 1 - Base#2. Anatomia Interna della Cartella `.git`|Anatomia Interna della Cartella `.git`]] – com'è fatto il "cervello" del repository
3. [[Git 1 - Base#3. Architettura Visuale di Git (Diagrammi Mermaid per Obsidian)|Architettura Visuale di Git (Diagrammi Mermaid per Obsidian)]] – zone di lavoro, ciclo di vita dei file, branch

**Preparazione**
4. [[Git 1 - Base#4. Navigazione e Comandi Base di Bash (Terminale)|Navigazione e Comandi Base di Bash (Terminale)]] – muoversi nel terminale
5. [[Git 1 - Base#5. Installazione, Configurazione e Autenticazione|Installazione, Configurazione e Autenticazione]] – setup iniziale e accesso a GitHub
6. [[Git 1 - Base#6. Avviare un Progetto: i Due Scenari Tipici|Avviare un Progetto: i Due Scenari Tipici]] – clone o cartella locale, giornata tipo

**Uso quotidiano**
7. [[Git 1 - Base#7. Flusso di Lavoro Fondamentale (Status, Add, Commit)|Flusso di Lavoro Fondamentale (Status, Add, Commit)]] – salvare le modifiche
8. [[Git 1 - Base#8. Ispezione dello Storico e Confronto Codice (Log, Diff)|Ispezione dello Storico e Confronto Codice (Log, Diff)]] – consultare lo storico e confrontare versioni
9. [[Git 1 - Base#9. Il File `.gitignore`|Il File `.gitignore`]] – cosa non tracciare (template Python + Abaqus)

**Branch e lavoro remoto**
10. [[Git 1 - Base#10. Gestione dei Branch (Rami di Sviluppo)|Gestione dei Branch (Rami di Sviluppo)]] – sviluppare in rami separati
11. [[Git 1 - Base#11. Risoluzione dei Conflitti di Merge|Risoluzione dei Conflitti di Merge]] – come risolverli
12. [[Git 1 - Base#12. Lavoro Remoto (GitHub, GitLab, Bitbucket)|Lavoro Remoto (GitHub, GitLab, Bitbucket)]] – push, pull, fetch

**Correggere errori**
13. [[Git 1 - Base#13. Annullamento e Ripristino delle Modifiche|Annullamento e Ripristino delle Modifiche]] – mappa "ho sbagliato, cosa faccio?"
14. [[Git 1 - Base#14. Comandi Utili e Salvataggi Temporanei (Stash)|Comandi Utili e Salvataggi Temporanei (Stash)]] – mettere da parte il lavoro in corso

**Riferimento rapido**
15. [[Git 1 - Base#15. Errori Frequenti e Soluzioni|Errori Frequenti e Soluzioni]] – messaggi di errore e soluzioni
16. [[Git 1 - Base#16. Buone Pratiche|Buone Pratiche]]
17. [[Git 1 - Base#17. Tabella Riassuntiva dei Comandi Essenziali|Tabella Riassuntiva dei Comandi Essenziali]] – i comandi essenziali in una pagina

---

## Livello Intermedio

1. [[Git 2 - Intermedio#1. Tag (Etichettare le Versioni)|Tag (Etichettare le Versioni)]] – etichettare le versioni
2. [[Git 2 - Intermedio#2. Tornare a un Commit Passato ("Viaggio nel Tempo")|Tornare a un Commit Passato ("Viaggio nel Tempo")]] – consultare, ripristinare o riprendere versioni passate
3. [[Git 2 - Intermedio#3. Tracciabilità dei Calcoli|Tracciabilità dei Calcoli]] – risalire dal risultato alla versione del codice
4. [[Git 2 - Intermedio#4. Pull Request e Flusso di Lavoro Collaborativo|Pull Request e Flusso di Lavoro Collaborativo]] – revisione e merge su GitHub
5. [[Git 2 - Intermedio#5. Prossimi Argomenti di questo Livello|Prossimi Argomenti di questo Livello]] – argomenti in arrivo

---

## Livello Avanzato

1. [[Git 3 - Avanzato#1. Hook e Framework pre-commit|Hook e Framework pre-commit]] – controlli automatici prima di ogni commit
2. [[Git 3 - Avanzato#2. GitHub Actions e Test Automatici|GitHub Actions e Test Automatici]] – test di regressione a ogni push
3. [[Git 3 - Avanzato#3. Riscrittura dello Storico con git filter-repo|Riscrittura dello Storico con git filter-repo]] – rimuovere file pesanti o password dallo storico
4. [[Git 3 - Avanzato#4. Submodule e Subtree|Submodule e Subtree]] – condividere codice tra repository
5. [[Git 3 - Avanzato#5. Strategie di Branching|Strategie di Branching]] – GitHub Flow, Git Flow, trunk-based
6. [[Git 3 - Avanzato#6. Struttura Interna di Git|Struttura Interna di Git]] – oggetti, riferimenti, comandi plumbing
7. [[Git 3 - Avanzato#7. Commit e Tag Firmati|Commit e Tag Firmati]] – firmare commit e tag con chiave SSH
8. [[Git 3 - Avanzato#8. Workflow Avanzati|Workflow Avanzati]] – procedure complete pronte da seguire
9. [[Git 3 - Avanzato#9. Tabella Riassuntiva dei Comandi Avanzati|Tabella Riassuntiva dei Comandi Avanzati]] – i comandi avanzati in una pagina
