# Bonjour Forge

[Accueil](../index.md) <a href="javascript:void(0)" onclick="window.history.back()">Retour</a>

Premier contact avec Forge : du chemin le plus court entre une requête
HTTP et une réponse texte. Sans base de données. Sans entité. Sans
template Jinja2. Sans CRUD.

Ce parcours suit l'ordre pédagogique du starter d'entrée
[Bonjour Forge](/docs/forge/starters/welcome-forge/debutant/welcome/) :

```text
forge run → route → contrôleur → Request → Response.text(...)
```

!!! tip "Forge n'est pas encore installé ?"
    Commencez par le parcours d'installation :
    [VM Debian vierge](/docs/forge/install/vm-debian/),
    [pipx](/docs/forge/install/pipx/),
    [depuis GitHub](/docs/forge/install/github/),
    [Windows + WSL (parcours complet)](/docs/forge/install/windows-wsl/).

---

## 1. Lancer Forge avec `forge run`

Une fois Forge installé et un projet créé (`forge new mon-projet`), la
commande officielle de développement est :

```bash
forge run
```

`forge run` lit `APP_ENV` (défaut `dev`), démarre le serveur de
développement et active l'autoreload : `python app.py` est redémarré
automatiquement dès qu'un fichier applicatif change. Pour désactiver
l'autoreload (chemin legacy) :

```bash
forge run --no-reload
```

En production (`APP_ENV=prod`), `forge run` refuse de démarrer le
serveur intégré et affiche la stratégie WSGI recommandée — voir
[Déploiement WSGI minimal](/docs/forge/deployment/wsgi-deployment/).

Une fois le serveur démarré, ouvrez `https://localhost:8000/welcome`
dans votre navigateur.

---

## 2. Comprendre la route

Toutes les routes Forge sont déclarées **explicitement** dans
`mvc/routes.py`. Aucune découverte automatique, aucune convention
cachée :

```python
# mvc/routes.py
from mvc.controllers.welcome_controller import WelcomeController

with router.group("", public=True) as pub:
    pub.add("GET", "/welcome",       WelcomeController.index, name="welcome-index")
    pub.add("GET", "/welcome/greet", WelcomeController.greet, name="welcome-greet")
```

Chaque ligne associe une méthode HTTP et un chemin à une méthode de
contrôleur. Ce qui est dans `mvc/routes.py` est exactement ce qui est
routé.

---

## 3. Comprendre le contrôleur

Un contrôleur Forge est une classe Python qui reçoit une `Request` et
retourne une `Response`. Les méthodes sont statiques, typées et
explicites :

```python
from core.http.request import Request
from core.http.response import Response
from core.mvc.controller.base_controller import BaseController


class WelcomeController(BaseController):
    @staticmethod
    def index(request: Request) -> Response:
        ...
```

Les annotations `request: Request -> Response` sont systématiques pour
que Pylance/VS Code propose l'autocomplétion sur `request.query(...)`,
`request.form(...)`, `request.json(...)`, `request.file(...)`,
`request.route(...)` et `request.header(...)` sans import manuel.
Voir [Convention HTTP inspectable](/docs/forge/reference/http/).

---

## 4. Retourner `Response.text("Bonjour Forge")`

La méthode la plus courte : aucun template, aucun moteur Jinja2.

```python
@staticmethod
def index(request: Request) -> Response:
    return Response.text("Bonjour Forge")
```

`Response.text(...)` produit une réponse `text/plain; charset=utf-8`.
Le navigateur sur `/welcome` affiche simplement :

```text
Bonjour Forge
```

Le cycle complet est minimal :

```text
Navigateur → GET /welcome → Router → WelcomeController.index(request) → Response.text(...)
```

---

## 5. Utiliser `request.query(...)`

`request.query("name", default="Forge")` retourne la première valeur
du paramètre `?name=...`, ou la valeur par défaut.

```python
@staticmethod
def greet(request: Request) -> Response:
    name = request.query("name", default="Forge")
    return Response.text(f"Bonjour {name}")
```

- `https://localhost:8000/welcome/greet?name=Roger` → `Bonjour Roger`
- `https://localhost:8000/welcome/greet` → `Bonjour Forge`

D'autres accesseurs nommés couvrent les autres canaux d'entrée :

| Accesseur | Lit | Retourne |
|---|---|---|
| `request.query(key, default=None)` | query string | `str` ou `default` |
| `request.form(key, default=None)` | formulaire `application/x-www-form-urlencoded` | `str` ou `default` |
| `request.json(key, default=None)` | body JSON | valeur JSON ou `default` |
| `request.header(name, default=None)` | en-têtes HTTP (insensible à la casse) | `str` ou `default` |
| `request.route(key, default=None)` | paramètres dynamiques (`/contacts/{id}`) | `str` ou `default` |
| `request.file(key, default=None)` | upload `multipart/form-data` | `UploadedFile` ou `default` |

---

## Récapitulatif des outils livrés

Cette progression met en jeu les briques DX livrées depuis la phase beta 11 :

| Brique | Rôle |
|---|---|
| `forge run` | Point d'entrée officiel — autoreload par défaut en dev |
| `Request` inspectable | Accesseurs nommés (`param`, `form`, `json`, `header`, …) |
| `Response.text(...)` | Réponse `text/plain; charset=utf-8` |
| `Response.html(...)` | Réponse `text/html; charset=utf-8` |
| `Response.json(...)` | Réponse `application/json; charset=utf-8` |
| Squelettes typés | `request: Request -> Response` partout par défaut |
| Starter `welcome` (`Bonjour Forge`) | Parcours d'entrée sans BDD ni template |

---

## Aller plus loin

Une fois ce premier contact assimilé :

| Étape | Ressource |
|---|---|
| **Progression officielle des starters** | [Progression recommandée](/docs/forge/starters/#progression-recommandee) |
| Démarrer un projet réel | [Démarrer avec Forge](/docs/forge/guide/getting-started/) |
| Parcours guidé avec MariaDB | [Guide de démarrage](/docs/forge/guide/guide/) |
| Première application complète | [Application complète](/docs/forge/guide/app-complete-tutorial/) |
| Catalogue des starters | [Vue d'ensemble des starters](/docs/forge/starters/) |
| Détails du starter `welcome` | [Bonjour Forge — starter](/docs/forge/starters/welcome-forge/debutant/welcome/) |
| Référence HTTP complète | [Convention HTTP inspectable](/docs/forge/reference/http/) |
| Toutes les commandes CLI | [Commandes CLI](/docs/forge/reference/cli-commands/) |

!!! info "Ne sautez pas directement vers le CRUD Contacts"
    Le starter `Contacts CRUD` est l'**étape 9** d'une progression de
    neuf paliers. Plusieurs notions intermédiaires (vue Jinja2, route
    dynamique, formulaire POST, validation, SQL) méritent leurs propres
    starters — voir la
    [progression recommandée](/docs/forge/starters/#progression-recommandee).

---

## Voir aussi

- [API Forge complète](/docs/forge/reference/api/)
- [Roadmap Forge](/docs/forge/roadmap/forge-roadmap/) — tickets DX livrés depuis la phase beta 11
- [Contrat de stabilité](/docs/forge/release/stability-contract/) — fichiers garantis préservés
- [Release et compatibilité](/docs/forge/release/release-and-compatibility/) — versions supportées
