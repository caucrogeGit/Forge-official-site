# Aide-mémoire de la progression

Récapitulatif des **24 paliers** de la progression *Bonjour Forge*, répartis en
trois niveaux, et des API Forge introduites à chaque étape. À garder sous la main
avant d'aborder les progressions opt-in autonomes.

## Niveau débutant — 11 paliers

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Bonjour Forge](/docs/forge/starters/welcome-forge/debutant/welcome/) | Premier contrôleur, une route, réponse texte | `Response.text(...)` |
| 2 | [Paramètres d'URL](/docs/forge/starters/welcome-forge/debutant/query-params/) | Lire la query string | `request.param("name", default=...)` |
| 3 | [Première vue HTML](/docs/forge/starters/welcome-forge/debutant/first-html-view/) | Rendre un template | `BaseController.render(...)` |
| 4 | [Route dynamique](/docs/forge/starters/welcome-forge/debutant/dynamic-route/) | Segment variable d'URL | `request.route_param("id")` |
| 5 | [Inspecter une requête](/docs/forge/starters/welcome-forge/debutant/request-debug/) | Explorer la requête en dev | `request.data`, `Response.debug(...)` |
| 6 | [Réponse JSON](/docs/forge/starters/welcome-forge/debutant/json-response/) | Données structurées (API) | `Response.json({...})` |
| 7 | [Le jeton CSRF](/docs/forge/starters/welcome-forge/debutant/csrf/) | Protéger les formulaires | `BaseController.csrf_token(request)` |
| 8 | [Premier formulaire POST](/docs/forge/starters/welcome-forge/debutant/form-post/) | Traiter un POST | `request.form("name", default=...)` |
| 9 | [Validation serveur](/docs/forge/starters/welcome-forge/debutant/server-validation/) | Refuser une valeur invalide | `Response.text(..., status=422)` |
| 10 | [Première base SQL](/docs/forge/starters/welcome-forge/debutant/first-sql/) | Lire en base, SQL visible | `core.database.db.fetch_one(...)` |
| 11 | [Écrire en base](/docs/forge/starters/welcome-forge/debutant/first-sql-write/) | Insérer une ligne | `core.database.db.insert(...)` |

## Niveau intermédiaire — 8 paliers

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Lister des enregistrements](/docs/forge/starters/welcome-forge/intermediaire/list-records/) | Lire plusieurs lignes et les itérer | `fetch_all(...)`, `{% for %}` |
| 2 | [Rechercher / filtrer](/docs/forge/starters/welcome-forge/intermediaire/filter-list/) | Filtrer une liste | `request.param("q")` + `WHERE … LIKE ?` |
| 3 | [Paginer une liste](/docs/forge/starters/welcome-forge/intermediaire/pagination/) | Découper une liste en pages | `LIMIT ? OFFSET ?`, `COUNT(*)` |
| 4 | [Héritage de gabarit](/docs/forge/starters/welcome-forge/intermediaire/layout-template/) | Factoriser l'enveloppe HTML | `{% extends %}`, `{% block %}` |
| 5 | [Modifier un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/update-record/) | Formulaire pré-rempli + mise à jour | `execute("UPDATE … WHERE id = ?")` |
| 6 | [Supprimer un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/delete-record/) | Action destructive sûre | `execute("DELETE … WHERE id = ?")` + CSRF |
| 7 | [Mémoriser un état en session](/docs/forge/starters/welcome-forge/intermediaire/session-state/) | Garder un état entre requêtes | `get_session_store()`, cookie durci |
| 8 | [Messages flash](/docs/forge/starters/welcome-forge/intermediaire/flash-messages/) | Retour one-shot après action | `set_flash` / `get_flash`, POST-Redirect-GET |

## Niveau avancé — 5 paliers

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Relations entre tables](/docs/forge/starters/welcome-forge/avance/relations/) | Deux tables liées, lecture jointe | `FOREIGN KEY`, `SELECT … JOIN …` |
| 2 | [Téléverser un fichier](/docs/forge/starters/welcome-forge/avance/file-upload/) | Recevoir et stocker un fichier | `request.file(...)`, `save_upload(...)` |
| 3 | [API JSON protégée](/docs/forge/starters/welcome-forge/avance/json-api/) | Exposer du JSON derrière un jeton | `Response.json`, `request.header("Authorization")` |
| 4 | [Écritures transactionnelles](/docs/forge/starters/welcome-forge/avance/db-transaction/) | Plusieurs écritures atomiques | `with transaction() as tx:`, `insert(..., tx=tx)` |

## Réponses (`core.http.response.Response`)

| Méthode | Usage |
|---------|-------|
| `Response.text(body, status=200)` | Réponse `text/plain` |
| `Response.html(body)` | Réponse HTML brute |
| `Response.json(obj, status=200)` | Réponse `application/json` (données **et** code HTTP) |
| `Response.debug(obj)` | Page de debug (dev uniquement, `404` en prod) |
| `BaseController.render(template, request=..., context=...)` | Rendu d'un template Jinja2 |
| `BaseController.redirect(url)` | Redirection (motif POST-Redirect-GET) |

## Lecture de la requête (`core.http.request.Request`)

| Accès | Source |
|-------|--------|
| `request.param("k", default=...)` | Query string (`?k=...`) |
| `request.route_param("k")` | Segment de route (`/x/{k}`) |
| `request.form("k", default=...)` | Corps d'un formulaire POST |
| `request.file("k")` | Fichier reçu (`multipart/form-data`) |
| `request.header("Name", default=...)` | En-tête HTTP (`Authorization`…) |
| `request.data` | Vue globale (méthode, chemin, headers, body…) |

## Base de données (`core.database`)

| Fonction | Usage |
|----------|-------|
| `db.fetch_one(sql, params)` | Première ligne (`dict`) ou `None` |
| `db.fetch_all(sql, params)` | Liste de lignes |
| `db.insert(sql, params)` | Insertion (paramétrée) |
| `db.execute(sql, params)` | Écriture générique |
| `with transaction() as tx:` + `db.insert(..., tx=tx)` | Écritures **atomiques** (commit / rollback) |

Les requêtes restent **paramétrées** (placeholders `?`) — jamais de
concaténation de valeurs. **Forge garde le SQL visible.** Les relations
s'écrivent à la main (`JOIN`), sans ORM.

## Sessions & flash (`core.security.session`, `core.sessions.manager`)

| Fonction | Usage |
|----------|-------|
| `get_session_store()` | Store de session (mémoire par défaut) |
| `get_session_id(request)` / `get_session(session_id)` | Identifier / lire la session |
| `set_flash(request, message)` / `get_flash(session_id)` | Message one-shot (lu **et** supprimé) |

Cookie de session **durci** : `HttpOnly; SameSite=Strict; Secure`.

## Fichiers & email

| Fonction | Usage |
|----------|-------|
| `forge_mvc_files.save_upload(file, category)` | Valider (extension, MIME, taille) puis stocker un fichier |
| `forge_mvc_mail.MailMessage(...)` | Décrire un email (sujet, destinataire, corps) |
| `forge_mvc_mail.Mailer(transport).send(message)` | Envoyer ; `ConsoleTransport` en dev (aucun SMTP) |

## Sécurité

- **CSRF** : champ caché `csrf_token` exigé sur chaque POST, vérifié
  automatiquement (palier débutant 7).
- **Validation serveur** : ne jamais faire confiance au client ; valider avant
  d'utiliser ou d'écrire (palier débutant 9).
- **Uploads** : `save_upload` contrôle extension, type MIME et taille **avant**
  toute écriture disque (palier avancé 2).
- **API** : vérifier l'autorisation (`Bearer`) **avant** de produire la donnée ;
  un refus renvoie `401` (palier avancé 4).
