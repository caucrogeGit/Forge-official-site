# Bilan — niveau intermédiaire

Récapitulatif des compétences acquises au **niveau intermédiaire** du starter
*Bonjour Forge*. Ce niveau fait passer des opérations unitaires (niveau
débutant) à une petite application pilotée par les données.

## Ce que vous avez validé

| Palier | Compétence acquise |
|--------|--------------------|
| 1 — [Lister des enregistrements](/docs/forge/starters/welcome-forge/intermediaire/list-records/) | Lire **plusieurs** lignes avec `fetch_all` et les itérer dans une vue (`{% for %}`). |
| 2 — [Rechercher / filtrer](/docs/forge/starters/welcome-forge/intermediaire/filter-list/) | Filtrer une liste avec `request.param` + `WHERE … LIKE ?` paramétré. |
| 3 — [Paginer une liste](/docs/forge/starters/welcome-forge/intermediaire/pagination/) | `LIMIT ? OFFSET ?` + `COUNT(*)`, liens précédent/suivant. |
| 4 — [Héritage de gabarit](/docs/forge/starters/welcome-forge/intermediaire/layout-template/) | Factoriser l'enveloppe HTML avec `{% extends %}` + `{% block %}`. |
| 5 — [Modifier un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/update-record/) | Formulaire pré-rempli + `UPDATE … WHERE id = ?` (POST + CSRF). |
| 6 — [Supprimer un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/delete-record/) | Action destructive `POST` + CSRF + `DELETE … WHERE id = ?`. |
| 7 — [Mémoriser un état en session](/docs/forge/starters/welcome-forge/intermediaire/session-state/) | Garder un état entre requêtes via le store de session + cookie durci. |
| 8 — [Messages flash](/docs/forge/starters/welcome-forge/intermediaire/flash-messages/) | Confirmer une action one-shot (`set_flash`/`get_flash`), motif POST-Redirect-GET. |

Vous savez maintenant construire à la main une petite application liste /
recherche / pagination / édition / suppression, avec gabarits factorisés, état
de session et retour utilisateur.

## Et ensuite

Place au **niveau avancé** : données reliées, upload de fichiers, envoi
d'emails, API JSON et écritures transactionnelles.

[Niveau avancé : Relations entre tables](/docs/forge/starters/welcome-forge/avance/relations/)
