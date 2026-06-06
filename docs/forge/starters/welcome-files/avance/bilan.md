# Bilan — niveau avancé (Files)

Récapitulatif du **niveau avancé** de la progression *Bonjour Forge Files*. Ce
niveau ouvre le capot : les **primitives** de stockage sécurisé que tout le module
— et les opt-ins média — composent (ADR-020).

## Ce que vous avez validé

| Palier | Compétence acquise |
|--------|--------------------|
| 1 — [Assainir un nom de fichier](/docs/forge/starters/welcome-files/avance/file-safe-name/) | Réduire un nom utilisateur arbitraire à un nom sûr (`secure_filename`). |
| 2 — [Chemin anti-traversal](/docs/forge/starters/welcome-files/avance/file-safe-path/) | Juger/normaliser un chemin (`is_safe_media_path`, `normalize_media_path`). |
| 3 — [Écrire des octets générés](/docs/forge/starters/welcome-files/avance/file-bytes/) | Écrire un contenu produit côté serveur (`save_bytes`). |

Vous comprenez les primitives sur lesquelles `save_upload`, `serve_media_file` et
les modules média sont bâtis.

## Et ensuite

La progression *Bonjour Forge Files* est terminée. `forge-mvc-files` est la
**fondation** de stockage média de Forge : `forge-mvc-images` en est le premier
client, et les futurs opt-ins média composeront ces mêmes primitives (ADR-020).

[Aide-mémoire de la progression Files](/docs/forge/starters/welcome-files/recapitulatif/)
