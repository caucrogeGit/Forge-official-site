# Bilan — niveau intermédiaire (Vidéo)

Récapitulatif des compétences acquises au **niveau intermédiaire** de la
progression *Bonjour Forge Vidéo*. Ce niveau fait passer de la lecture à une
petite chaîne **alimenter → servir → suivre**, toujours sans transcodage.

## Ce que vous avez validé

| Palier | Compétence acquise |
|--------|--------------------|
| 1 — [Téléverser une vidéo](/docs/forge/starters/welcome-video/intermediaire/video-upload/) | Ingérer un fichier (`ingest_video`), stockage sous UUID + ligne `videos` au statut `uploaded`, **sans ffmpeg**. |
| 2 — [Lire une vidéo](/docs/forge/starters/welcome-video/intermediaire/video-playback/) | Brancher la lecture officielle (`register_video_routes`), `GET /videos/{uuid}` en streaming Range. |
| 3 — [Suivre l'état d'une vidéo](/docs/forge/starters/welcome-video/intermediaire/video-status/) | Observer le cycle de vie par statut (`list_by_status`) : `uploaded → processing → ready`. |

Vous savez maintenant enregistrer une vidéo, la servir en streaming et suivre son
cycle de vie, sans transcodage.

## Et ensuite

Place au **niveau avancé** : on bascule vers le réel — sonde ffprobe, transcodage
ffmpeg, diagnostic du module.

[Niveau avancé : Sonder une vidéo](/docs/forge/starters/welcome-video/avance/video-probe/)
