# Aide-mémoire de la progression Images

Récapitulatif des paliers de la progression *Bonjour Forge Images* et des API du
module opt-in `forge-mvc-images` introduites à chaque étape.

!!! note "Module opt-in"
    Toute cette progression suppose `forge-mvc-images` installé. Le paquet
    dépend de `forge-mvc-files` et il est publié sur PyPI depuis `1.0.0-beta.13`
    (`pip install --pre forge-mvc-images`, palier « Installation » en tête de
    parcours). Le cœur de Forge reste autonome.

## Niveau débutant — traitement (sans base de données)

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Bonjour Forge Images](/docs/forge/starters/welcome-images/debutant/images-welcome/) | Vérifier le module, inspecter formats et tailles de variantes | `ALLOWED_IMAGE_EXTENSIONS`, `IMAGE_VARIANT_SIZES` |
| 2 | [Téléverser une image](/docs/forge/starters/welcome-images/debutant/image-upload/) | Vérifier le contenu avant d'écrire, générer les variantes | `save_image_upload` |
| 3 | [Miniatures et variantes](/docs/forge/starters/welcome-images/debutant/image-variants/) | Dériver les chemins des variantes et leurs URL | `image_variant_relative_paths`, `media_url` |

## Niveau intermédiaire — couche médias en base

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Rattacher une image à une entité](/docs/forge/starters/welcome-images/intermediaire/image-attach/) | Créer une ligne `media` reliée à une entité | `attach_media_to_entity` |
| 2 | [Afficher la galerie](/docs/forge/starters/welcome-images/intermediaire/image-gallery/) | Lire et afficher les images d'une entité avec variantes | `get_media_gallery` |
| 3 | [Texte alternatif et ordre](/docs/forge/starters/welcome-images/intermediaire/image-alt-order/) | Éditer accessibilité et ordre d'affichage | `update_media_alt_text`, `update_media_position` |

## Niveau avancé — couverture, suppression, sécurité

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Image de couverture](/docs/forge/starters/welcome-images/avance/image-cover/) | Désigner et afficher la couverture d'une entité | `get_cover_media` |
| 2 | [Supprimer proprement](/docs/forge/starters/welcome-images/avance/image-delete/) | Supprimer ligne + fichier + variantes en une fois | `delete_media` |
| 3 | [Garde de sécurité à l'upload](/docs/forge/starters/welcome-images/avance/image-safety/) | Refuser un fichier piégé ou une image-bombe | `verify_image_content`, `upload_max_image_pixels` |
