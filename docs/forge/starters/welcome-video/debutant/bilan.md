# Bilan — niveau débutant (Vidéo)

Récapitulatif des compétences acquises au **niveau débutant** de la progression
*Bonjour Forge Vidéo*. Ce niveau découvre le module opt-in `forge-mvc-video` et la
**lecture** des données, sans ffmpeg ni infrastructure.

## Ce que vous avez validé

| Palier | Compétence acquise |
|--------|--------------------|
| 1 — [Bonjour Forge Vidéo](/docs/forge/starters/welcome-video/debutant/video-welcome/) | Vérifier le module et inspecter sa configuration (`load_video_config`), token masqué. |
| 2 — [Lister les vidéos](/docs/forge/starters/welcome-video/debutant/video-list/) | Lire les dernières vidéos (`VideoRepository.list_recent`) et rester pédagogique (`503`) si la table manque. |
| 3 — [Le détail d'une vidéo](/docs/forge/starters/welcome-video/debutant/video-detail/) | Cibler une vidéo par UUID (`get_by_uuid`), distinguer trouvée / inconnue (`404`) / indisponible (`503`). |

Vous savez maintenant inspecter la configuration du module et lire les vidéos
enregistrées — liste comme détail unitaire.

## Et ensuite

Place au **niveau intermédiaire** : téléverser une vidéo, la servir en streaming
et suivre son cycle de vie.

[Niveau intermédiaire : Téléverser une vidéo](/docs/forge/starters/welcome-video/intermediaire/video-upload/)
