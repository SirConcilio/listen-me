# Listen_me

Piattaforma musicale con funzionalità social, progetto scolastico in PHP e MySQL/MariaDB (amministrazione tramite phpMyAdmin).

## Visione
Unire scoperta musicale, playlist e interazione tra amici, senza replicare contenuti protetti senza licenza.

## Requisiti
- Account, profili, gruppi e playlist personali/condivise.
- Note brevi associate alle canzoni, valutazioni da 1 a 5 stelle.
- Statistiche: ascolti totali, conteggi per brano e playlist, minuti di ascolto. Definire con precisione quando un ascolto è valido e prevenire duplicazioni.
- Visibilità delle playlist e statistiche regolata dalle preferenze di privacy; condivisione non obbligatoria e revocabile.
- Valutare API musicali ufficiali (Spotify o YouTube), accesso e limiti effettivi prima di scegliere un provider. Nessuna disponibilità gratuita di streaming integrale è presupposta.

## Stato
Archivio `listen_me.zip` presente nella libreria ChatGPT; sorgenti non ancora importati e feature implementate non verificate.

## Roadmap
- [ ] Importare il progetto e documentare versione PHP, dipendenze e schema SQL.
- [ ] Verificare API e condizioni d'uso, autenticazione e disponibilità playback.
- [ ] Implementare registrazione, sessioni sicure, gruppi e playlist.
- [ ] Registrare eventi di ascolto e aggregazioni statistiche.
- [ ] Gestire privacy, revoca del consenso, cancellazione/esportazione dati.
- [ ] Testare su mobile e preparare demo scolastica.

## Installazione prevista
`gh repo clone SirConcilio/listen-me`. Configurare PHP, server locale, MySQL e importare uno schema SQL privo di dati personali dopo il recupero del codice. Usare query parametrizzate, password hash e configurazione locale non versionata.
