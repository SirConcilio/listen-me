# Listen Me

Piattaforma musicale social per un progetto scolastico, sviluppata in PHP, JavaScript e MySQL/MariaDB, con amministrazione tramite phpMyAdmin. Riunisce scoperta musicale, playlist e interazione tra amici.

## v0.1.2 Music & Radio Update

Aggiornamento destinato a una pre-release. Il pacchetto previsto è `Listen_Me_v0.1.2_update.zip`. La pubblicazione in [GitHub Releases](https://github.com/SirConcilio/listen-me/releases) è in attesa dell'archivio originale. Questo repository ospita attualmente la documentazione.

- Interfaccia con menu laterale e più spazio su desktop, layout adattabile agli smartphone, schermata di login dedicata e conferma password in registrazione.
- Radio Browser per la ricerca di emittenti, con filtro per paese. L'aggiornamento include Groove Salad, Lush e Groove Salad Classic di SomaFM. Il player mostra **In diretta** quando il browser segnala l'avvio dello stream e offre arresto e volume, senza barra di avanzamento.
- Riproduzione tramite link YouTube nel player incorporato. La ricerca tramite YouTube Data API v3 richiede una chiave API. La ricerca e lo streaming Jamendo richiedono un Client ID.
- Profili, gruppi con codice d'invito, playlist collaborative, note, valutazioni e statistiche di ascolto fanno parte del prototipo. I risultati delle API musicali esterne non vengono ancora salvati automaticamente nelle playlist o nelle statistiche MySQL.

## Aggiornamento su XAMPP

Su un'installazione esistente, esegui il backup di cartella e database. Quando il pacchetto sarà disponibile, estrai l'aggiornamento in `C:\xampp\htdocs\` e applicalo alla cartella `listen-me`. L'aggiornamento è progettato per riutilizzare il database esistente senza reimportarlo. Avvia Apache e MySQL e apri `http://localhost/listen-me/`.

Per attivare la ricerca YouTube e l'integrazione Jamendo, copia `music-config.example.php` in `music-config.local.php` e compila rispettivamente `youtube_api_key` e `jamendo_client_id`. Conserva il file con le credenziali solo in locale, fuori dal repository e dagli archivi da pubblicare. Radio Browser e il player YouTube tramite link non richiedono queste credenziali.

## Stato dei test

| Controllo | Esito disponibile |
| --- | --- |
| Avvio su XAMPP dopo la correzione v0.1.1 | Confermato dall'utente |
| Sintassi PHP e JavaScript e integrità ZIP v0.1.2 | Riportate come superate nella conversazione di sviluppo |
| Provenienza degli stream SomaFM | Riportata come verificata nella conversazione di sviluppo |
| Audio delle radio in diretta | Da verificare nel browser |
| Ricerca YouTube, streaming Jamendo e riproduzione tramite link YouTube | Da collaudare. Servono credenziali per la ricerca YouTube e per Jamendo |
| Collaudo completo v0.1.2 su XAMPP con MySQL | Da eseguire, inclusi login, registrazione e riutilizzo del database |

## Roadmap verso v0.2

- Completare il collaudo su XAMPP, delle radio e dei servizi musicali.
- Aggiungere player persistente, coda di riproduzione, radio preferite e copertine nel catalogo.
- Sviluppare amicizie e ascolto sincronizzato.
- Valutare il salvataggio dei brani esterni nelle playlist secondo le condizioni dei servizi.

Consulta il [changelog](CHANGELOG.md) per la cronologia delle versioni.
