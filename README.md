# Fanavotana — Plateforme communautaire

> Réunir contenus, échanges et diffusion en direct dans une application web dédiée à une communauté chrétienne malgache.

**Domaines :** Développement full stack · API Python · Temps réel · Gestion de contenus

## Le besoin

Une communauté souhaite accéder à ses ressources, partager des publications, échanger et suivre des événements dans un espace cohérent. Le projet associe une dimension sociale à des contenus de lecture et d'apprentissage.

Fanavotana rassemble ces usages autour d'une interface React et d'un backend FastAPI.

## Périmètre de réalisation

- Interface web et API organisées par domaines fonctionnels.
- Modélisation des données et migrations PostgreSQL.
- Authentification, profils et permissions.
- Messagerie en temps réel et intégration de services multimédias.
- Tests et automatisation des contrôles de qualité.

## Fonctionnalités

| Domaine | Capacités |
|---|---|
| Communauté | Profils, abonnements, fil d'actualité, réactions et commentaires |
| Messagerie | Conversations privées et de groupe, échanges en temps réel |
| Événements | Publications d'événements et inscriptions |
| Direct | Gestion des diffusions, intégration LiveKit et référencement des replays |
| Baiboly | Lecture biblique, recherche, favoris, annotations et plans de lecture |
| Fihirana | Collections de cantiques, favoris, historique et permissions d'accès |
| Enseignements | Catégories, brouillons, publication et export PDF |
| Médias | Galerie, albums et bibliothèque de médias |
| Recherche | Recherche unifiée dans plusieurs types de contenus |
| Administration | Backoffice et gestion des accès selon les rôles |

La diffusion en direct et les services externes nécessitent leur configuration dans l'environnement de l'application.

## Exemple de parcours

Un membre consulte une publication, échange dans une conversation, retrouve un cantique et reprend son plan de lecture. Un responsable prépare un enseignement ou programme une diffusion, avec des permissions adaptées à son rôle.

## Architecture technique

| Couche | Technologies |
|---|---|
| Frontend | React 19, TypeScript, Vite, Tailwind CSS |
| État de l'interface | Zustand |
| Backend | Python, FastAPI, SQLAlchemy 2 |
| Données et migrations | PostgreSQL, Alembic |
| Authentification | JWT avec renouvellement, intégration Google OAuth |
| Échanges en temps réel | Socket.IO |
| Diffusion en direct | LiveKit |
| Médias | Cloudinary |
| Qualité | pytest, Ruff, Vitest, React Testing Library, ESLint |
| Automatisation | GitHub Actions |

## Points d'ingénierie

- **Organisation par domaine :** séparer les fonctions communautaires, éditoriales et administratives.
- **Continuité de session :** gérer le renouvellement des jetons côté client.
- **Évolution des données :** utiliser des migrations Alembic pour suivre le schéma PostgreSQL.
- **Permissions :** distinguer les usages des membres, responsables et administrateurs.
- **Qualité :** prévoir des contrôles backend et frontend, ainsi que des tests sur une base dédiée.

La documentation du projet décrit une chaîne de contrôles automatisés incluant lint, tests, migrations, vérification TypeScript et build. Cette présentation ne prétend pas certifier l'état courant de leur exécution.

## Ce que ce projet démontre

La conception d'une application complète associant API, interface typée, base relationnelle, contenus, permissions et interactions en temps réel.

L'apport fonctionnel est de réunir les ressources et les échanges de la communauté dans un même produit. Aucun nombre d'utilisateurs ni résultat de performance non mesuré n'est annoncé.

## À propos

Projet présenté par [Elia Randriantsiory](https://github.com/EliaRandriantsiory).

Ce dépôt est une **présentation de portfolio**. Il ne contient pas le code source de l'application, ni de données métier, de configuration de production ou d'identifiants. Les technologies tierces restent la propriété de leurs auteurs respectifs.

### Autres réalisations

- [Odoo ERP — Personnalisation métier](https://github.com/EliaRandriantsiory/odoo-erp-showcase)
- [RNT Server Manager — Administration Linux](https://github.com/EliaRandriantsiory/rnt-server-manager-showcase)
- [Fanavotana — Plateforme communautaire](https://github.com/EliaRandriantsiory/fanavotana-showcase)
