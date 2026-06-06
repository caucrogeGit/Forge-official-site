# Starters Forge

<div style="border:1px solid #FED7AA;background:linear-gradient(135deg,#FFF7ED 0%,#FFFFFF 58%,#F8FAFC 100%);border-radius:18px;padding:1.5rem 1.6rem;margin:1rem 0 1.5rem 0;">
  <p style="margin:0 0 .35rem 0;font-size:.85rem;font-weight:700;color:#EA580C;text-transform:uppercase;letter-spacing:.08em;">Forge · Parcours applicatifs</p>
  <h2 style="margin:.1rem 0 .45rem 0;font-size:2rem;line-height:1.15;color:#0F172A;">Vue d'ensemble des starters</h2>
  <p style="margin:0;color:#334155;font-size:1.05rem;max-width:880px;">Des parcours progressifs pour apprendre Forge, reconstruire vite et adapter à un vrai projet.</p>
</div>

## Principe

Un **starter** Forge est un exemple applicatif générable avec `forge starter:build`.
Il fournit un point de départ fonctionnel pour comprendre une mécanique du
framework. Un starter n'est pas un profil — voir
[Différence entre profil et starter](#difference-entre-profil-et-starter).

Profils recommandés selon le starter : `minimal` ou `standard` pour les paliers
avec base de données, aucun profil pour les paliers sans base.

## Catalogue

La progression cœur `welcome-forge` enseigne les fondamentaux ; chaque opt-in a
sa propre progression `welcome-<module>` (débutant → avancé). La liste exhaustive
est aussi disponible via `forge starter:list`.

### Bonjour Forge — progression cœur (`welcome-forge`)

*Débutant — 11 paliers* — [Bonjour Forge](/docs/forge/starters/welcome-forge/debutant/welcome/) · [Paramètres d'URL](/docs/forge/starters/welcome-forge/debutant/query-params/) · [Première vue HTML](/docs/forge/starters/welcome-forge/debutant/first-html-view/) · [Route dynamique](/docs/forge/starters/welcome-forge/debutant/dynamic-route/) · [Inspecter une requête](/docs/forge/starters/welcome-forge/debutant/request-debug/) · [Réponse JSON](/docs/forge/starters/welcome-forge/debutant/json-response/) · [Le jeton CSRF](/docs/forge/starters/welcome-forge/debutant/csrf/) · [Premier formulaire POST](/docs/forge/starters/welcome-forge/debutant/form-post/) · [Validation serveur](/docs/forge/starters/welcome-forge/debutant/server-validation/) · [Première base SQL](/docs/forge/starters/welcome-forge/debutant/first-sql/) · [Écrire en base](/docs/forge/starters/welcome-forge/debutant/first-sql-write/)

*Intermédiaire* — [Lister des enregistrements](/docs/forge/starters/welcome-forge/intermediaire/list-records/) · [Rechercher / filtrer](/docs/forge/starters/welcome-forge/intermediaire/filter-list/) · [Paginer une liste](/docs/forge/starters/welcome-forge/intermediaire/pagination/) · [Héritage de gabarit](/docs/forge/starters/welcome-forge/intermediaire/layout-template/) · [Modifier un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/update-record/) · [Supprimer un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/delete-record/) · [Mémoriser un état en session](/docs/forge/starters/welcome-forge/intermediaire/session-state/) · [Messages flash](/docs/forge/starters/welcome-forge/intermediaire/flash-messages/)

*Avancé* — [Relations entre tables](/docs/forge/starters/welcome-forge/avance/relations/) · [Téléverser un fichier](/docs/forge/starters/welcome-forge/avance/file-upload/) · [API JSON protégée](/docs/forge/starters/welcome-forge/avance/json-api/) · [Écritures transactionnelles](/docs/forge/starters/welcome-forge/avance/db-transaction/)

### IoT (opt-in `forge-mvc-iot`)

[Bonjour Forge IoT](/docs/forge/starters/welcome-iot/debutant/iot-welcome/) · [Lire les événements IoT](/docs/forge/starters/welcome-iot/debutant/iot-events/) · [Les événements d'un capteur](/docs/forge/starters/welcome-iot/debutant/iot-device/) · [Simuler une mesure IoT](/docs/forge/starters/welcome-iot/intermediaire/iot-simulate/) · [Exposer l'API IoT](/docs/forge/starters/welcome-iot/intermediaire/iot-api/) · [Tableau de bord IoT](/docs/forge/starters/welcome-iot/intermediaire/iot-dashboard/) · [Valider un message IoT](/docs/forge/starters/welcome-iot/avance/iot-contract/) · [Le subscriber MQTT](/docs/forge/starters/welcome-iot/avance/iot-subscriber/) · [Diagnostiquer le module IoT](/docs/forge/starters/welcome-iot/avance/iot-doctor/)

### Vidéo (opt-in `forge-mvc-video`)

[Bonjour Forge Vidéo](/docs/forge/starters/welcome-video/debutant/video-welcome/) · [Lister les vidéos](/docs/forge/starters/welcome-video/debutant/video-list/) · [Le détail d'une vidéo](/docs/forge/starters/welcome-video/debutant/video-detail/) · [Téléverser une vidéo](/docs/forge/starters/welcome-video/intermediaire/video-upload/) · [Lire une vidéo](/docs/forge/starters/welcome-video/intermediaire/video-playback/) · [Suivre l'état d'une vidéo](/docs/forge/starters/welcome-video/intermediaire/video-status/) · [Sonder une vidéo](/docs/forge/starters/welcome-video/avance/video-probe/) · [Transcoder une vidéo](/docs/forge/starters/welcome-video/avance/video-transcode/) · [Diagnostiquer le module Vidéo](/docs/forge/starters/welcome-video/avance/video-doctor/)

### Images (opt-in `forge-mvc-images`)

[Bonjour Forge Images](/docs/forge/starters/welcome-images/debutant/images-welcome/) · [Téléverser une image](/docs/forge/starters/welcome-images/debutant/image-upload/) · [Miniatures et variantes](/docs/forge/starters/welcome-images/debutant/image-variants/) · [Rattacher une image à une entité](/docs/forge/starters/welcome-images/intermediaire/image-attach/) · [Afficher la galerie](/docs/forge/starters/welcome-images/intermediaire/image-gallery/) · [Texte alternatif et ordre](/docs/forge/starters/welcome-images/intermediaire/image-alt-order/) · [Image de couverture](/docs/forge/starters/welcome-images/avance/image-cover/) · [Supprimer proprement](/docs/forge/starters/welcome-images/avance/image-delete/) · [Garde de sécurité à l'upload](/docs/forge/starters/welcome-images/avance/image-safety/)

### Fichiers (opt-in `forge-mvc-files`)

[Bonjour Forge Files](/docs/forge/starters/welcome-files/debutant/files-welcome/) · [Stocker un document](/docs/forge/starters/welcome-files/debutant/file-store/) · [Servir un fichier](/docs/forge/starters/welcome-files/debutant/file-serve/) · [Valider un upload](/docs/forge/starters/welcome-files/intermediaire/file-validate/) · [Limiter les uploads](/docs/forge/starters/welcome-files/intermediaire/file-rate-limit/) · [Supprimer un fichier](/docs/forge/starters/welcome-files/intermediaire/file-delete/) · [Assainir un nom de fichier](/docs/forge/starters/welcome-files/avance/file-safe-name/) · [Chemin anti-traversal](/docs/forge/starters/welcome-files/avance/file-safe-path/) · [Écrire des octets générés](/docs/forge/starters/welcome-files/avance/file-bytes/)

### Audio (opt-in `forge-mvc-audio`)

[Bonjour Forge Audio](/docs/forge/starters/welcome-audio/debutant/audio-welcome/) · [Téléverser un audio](/docs/forge/starters/welcome-audio/debutant/audio-upload/) · [Lire un audio](/docs/forge/starters/welcome-audio/debutant/audio-play/) · [Sonder un audio](/docs/forge/starters/welcome-audio/avance/audio-probe/) · [Transcoder en MP3](/docs/forge/starters/welcome-audio/avance/audio-transcode/) · [Diagnostiquer le module Audio](/docs/forge/starters/welcome-audio/avance/audio-doctor/)

### MFA (opt-in `forge-mvc-mfa`)

[Bonjour Forge MFA](/docs/forge/starters/welcome-mfa/debutant/mfa-welcome/) · [Secret TOTP et QR](/docs/forge/starters/welcome-mfa/debutant/mfa-secret/) · [Vérifier un code TOTP](/docs/forge/starters/welcome-mfa/debutant/mfa-verify/) · [Enrôler un facteur TOTP](/docs/forge/starters/welcome-mfa/intermediaire/mfa-enroll/) · [Challenge de connexion](/docs/forge/starters/welcome-mfa/intermediaire/mfa-challenge/) · [Codes de récupération](/docs/forge/starters/welcome-mfa/intermediaire/mfa-recovery/) · [Revalidation (step-up)](/docs/forge/starters/welcome-mfa/avance/mfa-revalidation/) · [Anti-rejeu TOTP](/docs/forge/starters/welcome-mfa/avance/mfa-replay/) · [Secret chiffré au repos](/docs/forge/starters/welcome-mfa/avance/mfa-crypto/)

### RBAC (opt-in `forge-mvc-rbac`)

[Bonjour Forge RBAC](/docs/forge/starters/welcome-rbac/debutant/rbac-welcome/) · [Code de permission](/docs/forge/starters/welcome-rbac/debutant/rbac-permission/) · [Rôle et slug](/docs/forge/starters/welcome-rbac/debutant/rbac-role/) · [Vérifier une permission](/docs/forge/starters/welcome-rbac/intermediaire/rbac-check/) · [Protéger une route](/docs/forge/starters/welcome-rbac/intermediaire/rbac-guard/) · [Permission dans un template](/docs/forge/starters/welcome-rbac/intermediaire/rbac-template/) · [Associer un rôle à un utilisateur](/docs/forge/starters/welcome-rbac/avance/rbac-user-role/) · [Résoudre les permissions](/docs/forge/starters/welcome-rbac/avance/rbac-resolve/) · [Rôles de la requête](/docs/forge/starters/welcome-rbac/avance/rbac-request-roles/)

### Workflow (opt-in `forge-mvc-workflow`)

[Bonjour Forge Workflow](/docs/forge/starters/welcome-workflow/debutant/workflow-welcome/) · [Nom de statut](/docs/forge/starters/welcome-workflow/debutant/workflow-status/) · [Retrouver un statut](/docs/forge/starters/welcome-workflow/debutant/workflow-find/) · [Déclarer les transitions](/docs/forge/starters/welcome-workflow/intermediaire/workflow-transition/) · [Vérifier une transition](/docs/forge/starters/welcome-workflow/intermediaire/workflow-check/) · [Transitions disponibles](/docs/forge/starters/welcome-workflow/intermediaire/workflow-available/) · [Badge de statut](/docs/forge/starters/welcome-workflow/avance/workflow-badge/) · [Couleur, libellé, classe](/docs/forge/starters/welcome-workflow/avance/workflow-color/) · [Helpers Workflow dans Jinja](/docs/forge/starters/welcome-workflow/avance/workflow-jinja/)

### Stats (opt-in `forge-mvc-stats`)

[Bonjour Forge Stats](/docs/forge/starters/welcome-stats/debutant/stats-welcome/) · [Nom d'événement](/docs/forge/starters/welcome-stats/debutant/stats-event/) · [Le schéma SQL](/docs/forge/starters/welcome-stats/debutant/stats-schema/) · [Le SQL d'insertion](/docs/forge/starters/welcome-stats/intermediaire/stats-track-sql/) · [Enregistrer un événement](/docs/forge/starters/welcome-stats/intermediaire/stats-track/) · [Valider un événement](/docs/forge/starters/welcome-stats/intermediaire/stats-validate/) · [Le SQL de consultation](/docs/forge/starters/welcome-stats/avance/stats-admin-sql/) · [Lister les événements](/docs/forge/starters/welcome-stats/avance/stats-list/) · [Normaliser une ligne](/docs/forge/starters/welcome-stats/avance/stats-normalize/)

### Mail (opt-in `forge-mvc-mail`)

[Bonjour Forge Mail](/docs/forge/starters/welcome-mail/debutant/mail-welcome/) · [Composer un message](/docs/forge/starters/welcome-mail/debutant/mail-message/) · [Choisir un transport](/docs/forge/starters/welcome-mail/intermediaire/mail-transport/) · [Rendre un template](/docs/forge/starters/welcome-mail/intermediaire/mail-template/) · [Configurer l'envoi](/docs/forge/starters/welcome-mail/avance/mail-config/) · [Diagnostiquer le module Mail](/docs/forge/starters/welcome-mail/avance/mail-doctor/)

## Progression recommandée

Le starter `Bonjour Forge` est volontairement minimal (deux routes texte,
zéro vue HTML, zéro base de données). **Ne sautez pas directement aux
notions SQL** : plusieurs paliers intermédiaires permettent d'aborder
l'accès base sereinement. La progression officielle est :

1. **Bonjour Forge** — afficher une réponse texte avec `Response.text(...)`.
   *(livré — starter `welcome`)*
2. **Paramètres d'URL** — lire une valeur simple avec `request.param(...)`.
   *(livré — starter `query-params`, ticket `STARTER-QUERY-PARAMS-001`)*
3. **Première vue HTML** — rendre une page avec `BaseController.render(...)`.
   *(livré — starter `first-html-view`, ticket `STARTER-FIRST-HTML-VIEW-001`)*
4. **Route dynamique** — lire un paramètre de route comme `/articles/{id}`.
   *(livré — starter `dynamic-route`, ticket `STARTER-DYNAMIC-ROUTE-001`)*
5. **Inspecter une requête** — explorer `request.data` avec `Response.debug(...)` en développement.
   *(livré — starter `request-debug`, ticket `STARTER-REQUEST-DEBUG-001`)*
6. **Réponse JSON** — retourner des données structurées avec `Response.json(...)`.
   *(livré — starter `json-response`, ticket `STARTER-JSON-RESPONSE-001`)*
7. **Le jeton CSRF** — comprendre la protection CSRF des formulaires.
   *(livré — starter `csrf`, ticket `STARTER-CSRF-001`)*
8. **Premier formulaire POST** — envoyer des données depuis un formulaire HTML.
   *(livré — starter `form-post`, ticket `STARTER-FORM-POST-001`)*
9. **Validation serveur** — refuser ou accepter les données reçues.
   *(livré — starter `server-validation`, ticket `STARTER-SERVER-VALIDATION-001`)*
10. **Première base SQL** — lire une donnée : MariaDB, migrations et SQL visible.
   *(livré — starter `first-sql`, ticket `STARTER-FIRST-SQL-001`)*
11. **Écrire en base** — insérer une ligne depuis un formulaire avec `db.insert(...)`.
   *(livré — starter `first-sql-write`, ticket `STARTER-FIRST-SQL-WRITE-001`)*

Une fois ces **11 paliers** acquis, vous avez terminé le starter de
découverte *Bonjour Forge*. Vous pouvez ensuite explorer les progressions
opt-in dédiées (IoT, vidéo, images, fichiers, audio, MFA, RBAC, workflow,
stats), chacune autonome et présentée par niveau dans le catalogue ci-dessus.

Le tableau de synthèse plus haut reste utile comme catalogue exhaustif
des starters disponibles aujourd'hui, mais l'ordre d'apprentissage
recommandé est celui des 11 paliers ci-dessus, suivi des progressions
opt-in de votre choix.

## Différence entre profil et starter

Un **profil** définit la base technique d'un projet créé avec `forge new`
(`forge new MonProjet --profile standard`). Un **starter** fournit un exemple
applicatif générable *après* la création du projet. Ils sont indépendants : un
profil ne remplace pas un starter, un starter ne modifie pas le profil, et un
starter peut illustrer un ou plusieurs profils.

Pour choisir un profil : [Profils de projet](/docs/forge/features/profiles/).

## Utiliser un starter

```bash
forge starter:list                 # catalogue complet depuis la CLI
forge starter:build <identifiant>  # ex. : forge starter:build welcome
```

Un starter se génère par son **identifiant public** (`welcome`, `query-params`,
`iot-welcome`…), pas par un numéro. Chaque page de starter liste les commandes
exactes, le modèle de données et les étapes de reconstruction.
