# Bilan — starter Bonjour Forge

Vous venez de terminer les **11 paliers** du starter de découverte
*Bonjour Forge*. Cette page récapitule **ce que vous avez validé** :
chaque ligne est une compétence acquise et réutilisable dans n'importe
quel projet Forge.

## Ce que vous avez validé

| Palier | Compétence validée |
|--------|--------------------|
| 1 — [Bonjour Forge](/docs/forge/starters/welcome-forge/debutant/welcome/) | Le cycle requête → contrôleur → réponse ; `Response.text(...)`. |
| 2 — [Paramètres d'URL](/docs/forge/starters/welcome-forge/debutant/query-params/) | Lire la *query string* avec `request.param("k", default=...)`. |
| 3 — [Première vue HTML](/docs/forge/starters/welcome-forge/debutant/first-html-view/) | Rendre un template avec `BaseController.render(...)`. |
| 4 — [Route dynamique](/docs/forge/starters/welcome-forge/debutant/dynamic-route/) | Lire un segment d'URL avec `request.route_param("id")`. |
| 5 — [Inspecter une requête](/docs/forge/starters/welcome-forge/debutant/request-debug/) | Explorer la requête en dev (`request.data`, `Response.debug(...)`). |
| 6 — [Réponse JSON](/docs/forge/starters/welcome-forge/debutant/json-response/) | Renvoyer des données structurées avec `Response.json({...})`. |
| 7 — [Le jeton CSRF](/docs/forge/starters/welcome-forge/debutant/csrf/) | Protéger les formulaires (`BaseController.csrf_token(...)`). |
| 8 — [Premier formulaire POST](/docs/forge/starters/welcome-forge/debutant/form-post/) | Traiter un POST et lire `request.form("k", default=...)`. |
| 9 — [Validation serveur](/docs/forge/starters/welcome-forge/debutant/server-validation/) | Refuser une valeur invalide avec un statut `422`. |
| 10 — [Première base SQL](/docs/forge/starters/welcome-forge/debutant/first-sql/) | Lire en base avec du SQL visible (`fetch_one`). |
| 11 — [Écrire en base](/docs/forge/starters/welcome-forge/debutant/first-sql-write/) | Insérer une ligne avec `insert(...)`. |

## À garder sous la main

L'[aide-mémoire de la progression](/docs/forge/starters/welcome-forge/recapitulatif/) rassemble toutes ces
API (réponses, requête, base de données, sécurité) sur une seule page.

## Et ensuite

Vous avez terminé le **niveau débutant** : HTTP, vues, formulaires protégés,
validation et SQL en lecture/écriture. Place au **niveau intermédiaire** :
listes, recherche, pagination, gabarits, mise à jour/suppression, sessions et
messages flash.

[Niveau intermédiaire : Lister des enregistrements](/docs/forge/starters/welcome-forge/intermediaire/list-records/)
