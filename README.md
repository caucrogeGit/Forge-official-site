# Forge-web

Site officiel du framework Forge.

Objectif du projet :

- publier https://forgemvc.com ;
- héberger la landing page publique ;
- héberger la documentation Forge générée avec MkDocs ;
- préparer un déploiement statique simple ;
- garder ce projet séparé du framework Forge.

## Périmètre

Ce dépôt concerne uniquement Forge-web :

- landing page ;
- documentation publique ;
- génération statique ;
- notes d'infrastructure ;
- scripts de build et de déploiement.

Ce dépôt ne doit pas modifier le cœur du framework Forge.

## Structure initiale

- landing/ : source de la landing page statique ;
- docs/ : documentation publique ou sources MkDocs ;
- site/ : site généré, non versionné ;
- infra/ : notes et fichiers d'infrastructure sans secrets ;
- notes/ : notes de travail du projet ;
- scripts/ : scripts locaux de génération ou déploiement.

## Décision initiale

Le site sera statique dans un premier temps.

MkDocs servira à générer la documentation.

Le reverse proxy et HTTPS seront traités plus tard, probablement avec Caddy.

Proxmox ne doit jamais être exposé directement au public.