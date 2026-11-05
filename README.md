# IOTTY — releases

Distribuzione pubblica dell'app Android IOTTY (sideload + auto-update).
Il codice sorgente è nel repo privato IOTTY (`mobile/`).

- **`latest.json`** — manifest versione corrente (l'app lo legge per l'auto-update).
- **`iotty-latest.apk`** — ultimo APK installabile.

## Installazione (prima volta)
Scarica `iotty-latest.apk` dal telefono e installalo (abilita "origini sconosciute").
Dai aggiornamenti successivi ci pensa l'app da sola.

## Come si pubblica una nuova versione
1. Build APK release dell'app.
2. Sostituisci `iotty-latest.apk` con il nuovo.
3. Aggiorna `latest.json` (incrementa `version_code`, aggiorna `version_name`, `notes`).
4. `git commit` + `git push`.
