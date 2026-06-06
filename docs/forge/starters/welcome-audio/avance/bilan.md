# Bilan — niveau avancé (Audio)

Récapitulatif du **niveau avancé** de la progression *Bonjour Forge Audio*. Ce
niveau ajoute le traitement (`ffprobe`/`ffmpeg`) et le diagnostic.

## Ce que vous avez validé

| Palier | Compétence acquise |
|--------|--------------------|
| 1 — [Sonder un audio](/docs/forge/starters/welcome-audio/avance/audio-probe/) | Extraire les métadonnées via `ffprobe` (`probe_audio`). |
| 2 — [Transcoder en MP3](/docs/forge/starters/welcome-audio/avance/audio-transcode/) | Convertir en MP3 via `ffmpeg`, synchrone et sans état (`transcode_to_mp3`). |
| 3 — [Diagnostiquer le module Audio](/docs/forge/starters/welcome-audio/avance/audio-doctor/) | Exposer les contrôles non invasifs de `forge audio:doctor`. |

Vous maîtrisez la chaîne audio complète : ingestion, lecture, sondage, transcodage,
diagnostic.

## Et ensuite

La progression *Bonjour Forge Audio* est terminée. `forge-mvc-audio` est une chaîne
audio **sobre et sans état** : opérations synchrones, fichiers repérés par uuid,
aucune table. Pour les gros volumes, on déporte le transcodage hors de la requête.

[Aide-mémoire de la progression Audio](/docs/forge/starters/welcome-audio/recapitulatif/)
