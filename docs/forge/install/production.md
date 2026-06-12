# Déploiement production

[Accueil](../index.md) <a href="javascript:void(0)" onclick="window.history.back()">Retour</a>

Cette page sert d'entrée vers les guides de déploiement production de Forge.
Le contenu détaillé reste dans les pages dédiées — ne pas dupliquer ici.

!!! warning "Outils de développement, pas de production"
    `python app.py` et `forge run` sont des outils de développement. En
    production publique, Forge se déploie obligatoirement derrière un
    serveur WSGI (Gunicorn) et un reverse proxy (Caddy ou Nginx).

## À lire dans l'ordre

1. [Déploiement WSGI minimal](/docs/forge/deployment/wsgi-deployment/) — architecture cible,
   `create_configured_wsgi_app()`, configuration Gunicorn de référence.
2. [Limites de production](/docs/forge/deployment/production-limits/) — ce que Forge ne fait
   pas et où poser des garde-fous applicatifs.
3. [Guide de déploiement](/docs/forge/deployment/deployment/) — pas-à-pas systemd, MariaDB,
   HTTPS, contrôles `forge deploy:check`.

## Voir aussi

- [Déploiement avancé](/docs/forge/deployment/deploy-advanced/) — scénarios étendus.
- [Sécurité en production](/docs/forge/deployment/production-security/) — durcissement et audit.
