# MediaScribe-Releases

Repository pubblico di distribuzione per le release Windows di MediaScribe.

- Releases: https://github.com/diegopiermarini/MediaScribe-Releases/releases
- Repository applicazione: https://github.com/diegopiermarini/MediaScribe-Releases

## Cosa contiene

- installer `.exe` pubblicati nelle GitHub Releases
- checksum `SHA256SUMS.txt` per verifica integrita
- documentazione minima per gli utenti finali

## Flusso di pubblicazione

Le release non vengono buildate in questo repository.

Le release vengono generate tramite una pipeline automatizzata e pubblicate automaticamente in questo repository.

- una GitHub Release con l'installer `MediaScribe-Setup-<versione>.exe`
- il file `SHA256SUMS.txt`

Le versioni pubblicate seguono Semantic Versioning nel formato `vMAJOR.MINOR.PATCH`.

## Download

Per scaricare una versione:

1. apri la sezione Releases di questo repository
2. scarica l'installer `.exe`
3. opzionalmente verifica il checksum SHA-256

