# X360 Mobile - Emulatore Xbox 360 per Android

<p align="center">
  <img src="https://x360mobile.com/logo.png" alt="Logo X360 Mobile" width="180" style="border-radius: 20%;"/>
</p>

<p align="center">
  <b>Un emulatore nativo sperimentale Xbox 360 per Android, basato nativamente su Xenia Canary.</b>
</p>

<p align="center">
  <a href="https://www.x360mobile.com"><b>Sito Ufficiale: www.x360mobile.com</b></a>
</p>

<p align="center">
  Choose Language / Scegli la lingua / Sprache wählen / Choisir la langue / Seleccionar idioma:
  <br>
  <a href="README.md">English</a> |
  <b>Italiano</b> |
  <a href="README.de.md">Deutsch</a> |
  <a href="README.fr.md">Français</a> |
  <a href="README.es.md">Español</a>
</p>

---

Benvenuti nel repository ufficiale di **X360 Mobile**, un emulatore nativo sperimentale per Xbox 360 sviluppato specificamente per la piattaforma Android. Creato utilizzando le moderne tecnologie ARM64 e Vulkan 1.3, X360 Mobile è il **pioniere nell'integrazione nativa del celeberrimo core Xenia Canary su Android**, offrendo ottimizzazioni avanzate e prestazioni elevate direttamente sui tuoi dispositivi mobili di fascia alta.

> [!NOTE]
> **Scopo del Repository:** 
> Per proteggere il codice sorgente e mantenere i miglioramenti proprietari relativi alle prestazioni, **X360 Mobile è closed-source**. Questo repository ufficiale non contiene il codice sorgente dell'emulatore. Funge invece da **archivio ufficiale delle versioni e piattaforma di distribuzione principale** per il rilascio delle build APK, la gestione dei problemi di compatibilità (Issues) e la condivisione delle guide utente.

---

## Caratteristiche Principali

* **Fondamenta Native su Xenia Canary:** Il primissimo emulatore Android progettato nativamente attorno a Xenia Canary fin dal suo concepimento, invece di migrare successivamente da Xenia Master, garantendo un'architettura e prestazioni superiori.
* **Backend Vulkan Moderno:** Sfrutta le API Vulkan 1.3 per offrire un utilizzo ottimale dell'hardware, framerate elevati e un basso sovraccarico di sistema.
* **Overlay Touch Personalizzato:** Gamepad virtuali completamente personalizzabili con feedback aptico, risposta analogica fluida e layout adatti a qualsiasi dimensione dello schermo.
* **Supporto per Controller Fisici:** Supporto plug-and-play immediato per controller esterni tramite Bluetooth o USB-OTG (inclusi Xbox Series X|S, DualSense, DualShock 4 e i principali controller per dispositivi mobili).
* **Profili Specifici per Gioco:** Regola risoluzioni, opzioni di compilazione degli shader e limiti di memoria singolarmente per ciascun gioco, per spremere ogni bit di potenza dal tuo dispositivo.
* **Ottimizzazioni per Mobile:** Traduzione integrata e dinamica del codice assembly PowerPC in istruzioni native ARM64 con micro-ottimizzazioni specifiche per i chipset Snapdragon e Dimensity.

---

## Requisiti di Sistema

L'emulazione di Xbox 360 è un processo sperimentale ed estremamente intenso a livello computazionale, che richiede una complessa traduzione hardware in tempo reale. Consulta la tabella seguente per comprendere le prestazioni attese sul tuo dispositivo.

| Specifica | Requisiti Minimi | Consigliati (Per Prestazioni Giocabili) |
| :--- | :--- | :--- |
| **Sistema Operativo** | Android 11 (64-bit) | Android 13 o più recente (64-bit) |
| **Processore e GPU** | Qualcomm Snapdragon con GPU Adreno (serie 600/700/800) | Qualcomm Snapdragon di fascia alta (consigliato Snapdragon 8 Gen 1 o superiore) |
| **RAM (Memoria)** | 6 GB RAM | 8 GB - 12 GB RAM (o superiore) |
| **Memoria (Velocità)**| Memoria ad alta velocità (consigliata UFS 3.1 o superiore) | Memoria ultra-veloce UFS 3.1/4.0 |

> [!WARNING]
> I dispositivi dotati di processori con GPU Mali, GPU Xclipse di Samsung (basate su AMD RDNA), GPU Adreno datate (precedenti alla serie 600) o chipset entry-level/economici subiranno gravi limitazioni delle prestazioni, glitch grafici, forte surriscaldamento (thermal throttling) o arresti anomali. Si raccomanda caldamente l'uso di un moderno processore Qualcomm Snapdragon con GPU Adreno per risultati ottimali.

---

## Guida Rapida

1. **Scarica l'APK:** Vai nella nostra sezione [Releases](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/releases) e scarica l'ultimo pacchetto `.apk` stabile.
2. **Abilita Origini Sconosciute:** Se richiesto, consenti al tuo browser web o al gestore file di installare applicazioni da origini sconosciute nelle impostazioni di sicurezza di Android.
3. **Installa e Avvia:** Installa il file APK scaricato e avvia **X360 Mobile**.
4. **Configura le Directory:** Crea una cartella dedicata nella memoria interna o esterna del tuo dispositivo (ad es. `/Emulation/Xbox360/Games`) e inserisci lì i file di gioco legalmente ottenuti.
5. **Formati di Gioco:** L'emulatore supporta ufficialmente i formati `.iso`, `.xex` e le cartelle estratte (unpacked).
6. **Carica e Gioca:** Indirizza l'emulatore alla cartella dei tuoi giochi, seleziona un titolo e avvia la partita!

---

## Domande Frequenti (FAQ)

### X360 Mobile è gratuito?
**Sì.** X360 Mobile è completamente scaricabile e utilizzabile gratuitamente. Non addebitiamo costi né includiamo pubblicità invasive che possano rovinare l'esperienza di gioco.

### Perché il progetto è closed-source?
Abbiamo scelto di mantenere X360 Mobile closed-source per prevenire fork fraudolenti, re-packaging dannosi (ad esempio, inserimento di adware/spyware nelle nostre build) e per proteggere la nostra pipeline di conversione ARM64 e le ottimizzazioni del compilatore. Vogliamo garantire che gli utenti ricevano solo pacchetti sicuri, altamente ottimizzati e firmati ufficialmente direttamente da questo repository o dal nostro sito web ufficiale.

### X360 Mobile è correlato al progetto desktop Xenia?
X360 Mobile è basato sull'incredibile codice sorgente di **Xenia Canary** (un progetto open-source per PC). Abbiamo effettuato il porting, il refactoring e l'ottimizzazione del motore grafico e di esecuzione originale per farlo funzionare su Android. Nutriamo il massimo rispetto per gli sviluppatori originali di Xenia e puntiamo a offrire lo stesso livello di eccellenza sui dispositivi mobili.

### Quali giochi posso avviare in questo momento?
La compatibilità è in continuo sviluppo. Al momento sono stati **testati oltre 300 titoli**, dei quali circa il **40% è giocabile**.

Per una lista di compatibilità completa e sempre aggiornata, visita il nostro sito ufficiale su [www.x360mobile.com](https://www.x360mobile.com). Mentre i classici titoli Arcade, i giochi indie e i giochi 3D leggeri funzionano molto bene, i titoli AAA più esigenti (come *Red Dead Redemption*, *Halo 3* o *Gears of War*) sono avviabili e possono raggiungere velocità giocabili sui processori Snapdragon di punta più recenti, sebbene possano ancora mostrare piccoli glitch grafici o cali di fotogrammi.

---

## Segnalazione dei Problemi

Se riscontri crash, bug grafici o problemi di compatibilità:
1. Vai nella sezione [Issues](https://github.com/Ashnar2602/X360-Mobile---OFFICIAL/issues).
2. Cerca se il problema è già stato segnalato da un altro utente.
3. Se non è presente, apri una nuova issue utilizzando il nostro modello e includi:
   * Il modello del tuo dispositivo e il chipset (es. Samsung Galaxy S23, Snapdragon 8 Gen 2).
   * La versione esatta di Android e la RAM installata.
   * Il titolo del gioco e il formato (.iso o .xex).
   * Una descrizione dettagliata del bug e, se possibile, screenshot o video.

---

## Note Legali e Dichiarazione di Limitazione di Responsabilità

* **Xbox 360** è un marchio registrato di Microsoft Corporation. **X360 Mobile** non è in alcun modo affiliato, autorizzato, sponsorizzato o supportato da Microsoft Corporation, dalle sue collegate o dalle sue sussidiarie.
* Tutti i titoli dei giochi, le immagini e le risorse del brand sono marchi registrati dei rispettivi proprietari.
* **X360 Mobile** non include alcun file di gioco, software di sistema (dashboard) o ROM protetta da copyright. Gli utenti sono legalmente tenuti a possedere copie fisiche dei giochi e a effettuarne il dump per uso personale e non commerciale.
* Scaricando e utilizzando questo software, accetti i nostri termini di servizio e riconosci che l'emulazione è una tecnologia sperimentale utilizzata a tuo rischio e pericolo.

---

<p align="center">
  © 2026 X360 Mobile Team. Tutti i diritti riservati. <br>
  Per novità, aggiornamenti e altro, visita il sito <a href="https://www.x360mobile.com">www.x360mobile.com</a>.
</p>
