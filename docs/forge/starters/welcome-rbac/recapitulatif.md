# Aide-mémoire de la progression RBAC

Récapitulatif des paliers de la progression *Bonjour Forge RBAC* et des API du module
opt-in `forge-mvc-rbac` introduites à chaque étape.

!!! note "Module opt-in"
    `forge-mvc-rbac` est **publié sur PyPI** : `pip install --pre forge-mvc-rbac`. Il
    repose sur un **contrat déclaratif** `mvc/security/rbac.json` (ADR-014). `can()`
    est auto-enregistré dans les templates.

## Niveau débutant — déclarer & comprendre (sans BDD)

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Bonjour Forge RBAC](/docs/forge/starters/welcome-rbac/debutant/rbac-welcome/) | Charger et inspecter le contrat | `load_rbac_contract` |
| 2 | [Code de permission](/docs/forge/starters/welcome-rbac/debutant/rbac-permission/) | Normaliser/valider une permission | `normalize_permission_code`, `validate_permission` |
| 3 | [Rôle et slug](/docs/forge/starters/welcome-rbac/debutant/rbac-role/) | Dériver/valider un rôle | `normalize_role_slug`, `validate_role` |

## Niveau intermédiaire — vérifier & appliquer (contrat)

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Vérifier une permission](/docs/forge/starters/welcome-rbac/intermediaire/rbac-check/) | Rôles → permission accordée ? | `has_contract_permission` |
| 2 | [Protéger une route](/docs/forge/starters/welcome-rbac/intermediaire/rbac-guard/) | Garde de route 403/passage | `require_contract_permission` |
| 3 | [Permission dans un template](/docs/forge/starters/welcome-rbac/intermediaire/rbac-template/) | Adapter l'UI avec `can()` | `make_can` |

## Niveau avancé — relier aux utilisateurs

| # | Palier | Ce qu'on apprend | API-clé |
|---|--------|------------------|---------|
| 1 | [Associer un rôle à un utilisateur](/docs/forge/starters/welcome-rbac/avance/rbac-user-role/) | Association user ↔ rôle | `create_auth_user_role` |
| 2 | [Résoudre les permissions](/docs/forge/starters/welcome-rbac/avance/rbac-resolve/) | Permissions effectives via `fetch_all` | `get_user_permissions`, `user_has_permission` |
| 3 | [Rôles de la requête](/docs/forge/starters/welcome-rbac/avance/rbac-request-roles/) | Vue runtime du RBAC | `get_request_roles`, `get_request_permissions` |
