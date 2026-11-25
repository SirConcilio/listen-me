# Changelog

## v0.1.2 Music & Radio Update

Disponibile come [pre-release Alpha](https://github.com/SirConcilio/listen-me/releases/tag/Alpha), con asset `Listen_Me_v0.1.2_update.zip`. Presenza verificata il 25 novembre 2026; collaudo dell'archivio ancora da eseguire.

- Riorganizzati il layout desktop, il login e il modulo di registrazione con conferma password.
- Aggiunte ricerca delle radio con Radio Browser, filtro per paese e tre emittenti SomaFM. Il player segnala la diretta all'avvio effettivo dello stream e rimuove la barra di avanzamento.
- Aggiunte la ricerca YouTube tramite chiave API e la ricerca e lo streaming Jamendo tramite Client ID. È disponibile anche il player incorporato per i link YouTube.
- L'aggiornamento è progettato per riutilizzare il database esistente. Il salvataggio automatico dei risultati esterni in playlist e statistiche resta da implementare.
- La conversazione di sviluppo riporta controlli di sintassi PHP e JavaScript e di integrità ZIP superati, oltre alla verifica della provenienza degli stream. Restano da collaudare la riproduzione effettiva delle radio, le integrazioni musicali e l'aggiornamento completo su XAMPP con MySQL.

## v0.1.1

- Sostituito l'operatore `??=` in `bootstrap.php` con un controllo esplicito della sessione per mantenere il token CSRF ed evitare l'errore di parsing sulle versioni di PHP che non riconoscono l'operatore.
- La conversazione di sviluppo riporta il controllo di sintassi con PHP 8.4. L'utente ha confermato l'avvio su XAMPP dopo la correzione.

## v0.1

- Primo prototipo con autenticazione, profilo, player audio, videoclip YouTube e integrazione Radio Browser.
- Introdotti playlist collaborative, gruppi con invito, note, commenti, reazioni, valutazioni e statistiche di ascolto.
- La conversazione di sviluppo riporta i controlli di sintassi PHP e JavaScript. Il collaudo con MySQL e la riproduzione delle radio rimanevano aperti.
