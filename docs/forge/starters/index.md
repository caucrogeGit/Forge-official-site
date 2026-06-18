# Starters Forge

<div style="border:1px solid #FED7AA;background:linear-gradient(135deg,#FFF7ED 0%,#FFFFFF 58%,#F8FAFC 100%);border-radius:18px;padding:1.5rem 1.6rem;margin:1rem 0 1.5rem 0;">
  <p style="margin:0 0 .35rem 0;font-size:.85rem;font-weight:700;color:#EA580C;text-transform:uppercase;letter-spacing:.08em;">Forge · Parcours applicatifs</p>
  <h2 style="margin:.1rem 0 .45rem 0;font-size:2rem;line-height:1.15;color:#0F172A;">Vue d'ensemble des starters</h2>
  <p style="margin:0;color:#334155;font-size:1.05rem;max-width:880px;">Des parcours progressifs pour apprendre Forge, reconstruire vite et adapter à un vrai projet.</p>
</div>

## Principe

Un **starter** Forge est un parcours d'apprentissage que l'on réalise à la main en suivant la documentation.
Chaque palier montre le contrôleur, la vue et la route à créer pour comprendre une mécanique du framework.
Un starter n'est pas un profil, voir
[Différence entre profil et starter](#difference-entre-profil-et-starter).

Profils recommandés selon le starter : `minimal` ou `standard` pour les paliers
avec base de données, aucun profil pour les paliers sans base.

## Catalogue

La progression cœur `welcome-forge` enseigne les fondamentaux ; chaque opt-in a
sa propre progression `welcome-<module>` (débutant puis avancé).

### Bonjour Forge : progression cœur (`welcome-forge`)

*Débutant, 11 paliers (tutoriel continu)* : [Bonjour Forge](/docs/forge/starters/welcome-forge/debutant/welcome/) · [Paramètres d'URL](/docs/forge/starters/welcome-forge/debutant/query-params/) · [Première vue HTML](/docs/forge/starters/welcome-forge/debutant/first-html-view/) · [Route dynamique](/docs/forge/starters/welcome-forge/debutant/dynamic-route/) · [Inspecter une requête](/docs/forge/starters/welcome-forge/debutant/request-debug/) · [Réponse JSON](/docs/forge/starters/welcome-forge/debutant/json-response/) · [Le jeton CSRF](/docs/forge/starters/welcome-forge/debutant/csrf/) · [Premier formulaire POST](/docs/forge/starters/welcome-forge/debutant/form-post/) · [Validation serveur](/docs/forge/starters/welcome-forge/debutant/server-validation/) · [Première base SQL](/docs/forge/starters/welcome-forge/debutant/first-sql/) · [Écrire en base](/docs/forge/starters/welcome-forge/debutant/first-sql-write/)

*Intermédiaire, 8 paliers (tutoriel continu)* : [Lister des enregistrements](/docs/forge/starters/welcome-forge/intermediaire/list-records/) · [Héritage de gabarit](/docs/forge/starters/welcome-forge/intermediaire/layout-template/) · [Rechercher / filtrer](/docs/forge/starters/welcome-forge/intermediaire/filter-list/) · [Paginer une liste](/docs/forge/starters/welcome-forge/intermediaire/pagination/) · [Modifier un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/update-record/) · [Supprimer un enregistrement](/docs/forge/starters/welcome-forge/intermediaire/delete-record/) · [Messages flash](/docs/forge/starters/welcome-forge/intermediaire/flash-messages/) · [Mémoriser un état en session](/docs/forge/starters/welcome-forge/intermediaire/session-state/)

*Avancé, 4 paliers (tutoriel continu)* : [Relations entre tables](/docs/forge/starters/welcome-forge/avance/relations/) · [Écritures transactionnelles](/docs/forge/starters/welcome-forge/avance/db-transaction/) · [Téléverser un fichier](/docs/forge/starters/welcome-forge/avance/file-upload/) · [API JSON protégée](/docs/forge/starters/welcome-forge/avance/json-api/)

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

Le niveau débutant `Bonjour Forge` est un **tutoriel continu** : vous
construisez à la main un seul projet qui grandit palier après palier (un
contrôleur qui s'enrichit, un `mvc/routes.py` qui s'accumule). **Ne sautez pas
directement aux notions SQL** : les paliers HTTP préparent l'accès base
sereinement. Les 11 paliers du niveau débutant :

1. **Bonjour Forge** : afficher une réponse texte avec `Response.text(...)`.
2. **Paramètres d'URL** : lire une valeur simple avec `request.query(...)`.
3. **Première vue HTML** : rendre une page avec `BaseController.render(...)`.
4. **Route dynamique** : lire un paramètre de route comme `/articles/{id}`.
5. **Inspecter une requête** : explorer `request.data` avec `Response.debug(...)` en développement.
6. **Réponse JSON** : retourner des données structurées avec `Response.json(...)`.
7. **Le jeton CSRF** : comprendre la protection CSRF des formulaires.
8. **Premier formulaire POST** : envoyer des données depuis un formulaire HTML.
9. **Validation serveur** : refuser ou accepter les données reçues.
10. **Première base SQL** : lire une donnée : MariaDB, migrations et SQL visible.
11. **Écrire en base** : insérer une ligne depuis un formulaire avec `db.insert(...)`.

Après le préambule d'installation, suivez les paliers dans l'ordre depuis
[Bonjour Forge](/docs/forge/starters/welcome-forge/debutant/welcome/).

Une fois ces **11 paliers** acquis, vous avez terminé le niveau débutant de
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

Un starter se suit **à la main**, palier par palier.
Pour une progression opt-in, commencez par sa page d'installation (installer le module, disposer d'un projet Forge), puis enchaînez les paliers.
Chaque palier indique le contrôleur, la vue et la route à créer dans le projet.

!!! note "Les starters ne se génèrent pas"
    Forge ne génère pas les starters et n'écrit jamais dans votre `mvc/routes.py`.
    Vous créez vous-même chaque fichier et ajoutez chaque route, en suivant la documentation du palier (voir [ADR-035](/docs/forge/adr/035-starters-manual-not-generated/)).
