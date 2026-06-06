# Décisions d'architecture (ADR)

Les *Architecture Decision Records* documentent les décisions structurantes
de Forge. Chaque ADR a **force décisionnelle** : à lire avant toute
proposition qui le concerne. Un nouvel ADR est requis pour toute décision
structurante (`docs/adr/<numéro>-<sujet>.md`).

| Numéro | Sujet |
|---|---|
| [ADR-001](/docs/forge/adr/001-auth-strategy/) | Stratégie d'authentification |
| [ADR-002](/docs/forge/adr/002-session-strategy/) | Stockage de session |
| [ADR-003](/docs/forge/adr/003-language-convention/) | API publique en anglais |
| [ADR-004](/docs/forge/adr/004-core-perimeter/) | Périmètre du core minimal strict |
| [ADR-005](/docs/forge/adr/005-packaging/) | Packaging hybride monorepo + multi-distributions PyPI |
| [ADR-006](/docs/forge/adr/006-python-version/) | Python 3.12+ minimum |
| [ADR-007](/docs/forge/adr/007-charter-v2-adoption/) | Adoption formelle de la charte v2 |
| [ADR-008](/docs/forge/adr/008-auth-audit-architecture/) | Audit auth : logging fourni, persistance applicative |
| [ADR-009](/docs/forge/adr/009-stability-policy-terrain/) | Politique de stabilité : audits, bêta consolidée, tests terrain |
| [ADR-010](/docs/forge/adr/010-auth-session-canonical-api/) | API canonique auth/session |
| [ADR-011](/docs/forge/adr/011-auth-audit-vocab-perimeter/) | Périmètre du vocabulaire d'audit auth |
| [ADR-012](/docs/forge/adr/012-legacy-format-deprecation-policy/) | Politique de dépréciation du format legacy |
| [ADR-013](/docs/forge/adr/013-nullable-required-contract-policy/) | Politique nullable / required des contrats |
| [ADR-014](/docs/forge/adr/014-rbac-contract-location/) | Emplacement du contrat RBAC |
| [ADR-015](/docs/forge/adr/015-dev-tls-handshake-per-thread/) | Handshake TLS par thread (dev-server) |
| [ADR-016](/docs/forge/adr/016-opt-in-unification/) | Unification du modèle opt-in : concept unique, cycle install/enable à 4 verbes |
| [ADR-017](/docs/forge/adr/017-slug-type/) | Type `slug` et module URL-slug canonique (`core/http/slug.py`) |
| [ADR-018](/docs/forge/adr/018-image-module-extraction/) | Extraction du traitement d'image hors du core : `forge-mvc-images` (proposé) |
| [ADR-019](/docs/forge/adr/019-upload-extraction/) | Extraction de l'upload générique hors du core : `forge-mvc-files` (proposé) |
| [ADR-020](/docs/forge/adr/020-files-media-storage-primitives/) | Périmètre de `forge-mvc-files` : primitives de stockage média génériques (proposé) |
| [ADR-021](/docs/forge/adr/021-pivot-extraction/) | Extraction de pivot advanced hors du core : `forge-mvc-pivot` (accepté) |
| [ADR-022](/docs/forge/adr/022-mail-extraction/) | Extraction de l'email hors du core : `forge-mvc-mail` (accepté) |
