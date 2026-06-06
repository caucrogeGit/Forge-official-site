# Release et compatibilité Forge

Cette section regroupe les documents officiels de versionnement, de compatibilité
et de migration pour Forge.

---

## Documents disponibles

### [Politique de release](/docs/forge/release/release-policy/)

Définit les règles SemVer adaptées de Forge :

- quand incrémenter MAJOR, MINOR ou PATCH ;
- règles Git et format de tag `vX.Y.Z` ;
- validation obligatoire avant chaque release ;
- structure du CHANGELOG.

### [Politique de dépréciation](/docs/forge/release/deprecation-policy/)

Définit le cycle de vie des fonctionnalités retirées :

- annonce → maintien → retrait ;
- avertissements CLI sur `stderr` ;
- `DeprecationWarning` Python ;
- alternatives obligatoires ;
- retrait réservé aux versions MAJOR.

### [Matrice de compatibilité](/docs/forge/release/compatibility/)

Documente les versions officiellement supportées :

- Python 3.12–3.14 ;
- MariaDB 10.11+ LTS, connecteur 1.1.14 ;
- Node.js / Tailwind CSS (build CSS uniquement) ;
- OS et dépendances runtime et dev ;
- tests opt-in MariaDB (`FORGE_E2E_MARIADB=1`).

### [Guide de migration](/docs/forge/features/migration-guide/)

Explique comment passer d'une version Forge à une autre :

- vérifications avant migration ;
- règles PATCH / MINOR / MAJOR ;
- fichiers générés vs fichiers préservés ;
- sauvegarde, rollback, checklist.

### [Politique LTS](/docs/forge/release/lts-policy/)

Évalue l'intérêt d'une version Long Term Support :

- arguments pour et contre une LTS immédiate ;
- trois scénarios documentés ;
- décision : Forge ne déclare pas encore de LTS ;
- conditions à remplir avant une future LTS.

### [Contrat de stabilité](/docs/forge/release/stability-contract/)

Définit ce qui est stable, interne ou expérimental en Forge :

- API publique garantie ;
- API interne (peut changer entre mineures) ;
- API expérimentale (disponible, interface peut évoluer) ;
- fichiers générés et préservés.

---

## Procédures opérationnelles

Ces documents concernent les mainteneurs de Forge :

- [Procédure de release](/docs/forge/release/release/) — checklist avant chaque tag
- [Validation locale](/docs/forge/release/release-local/) — test de la wheel localement

---

## Voir aussi

- [Guide de déploiement](/docs/forge/deployment/deployment/) — déployer un projet Forge
- [Sécurité en production](/docs/forge/deployment/production-security/) — checklist sécurité 30 points
- [Politique de release](/docs/forge/release/release-policy/) — règles MAJOR/MINOR/PATCH

---
