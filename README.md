# Blasti — بلاصتي 🚕

**Plateforme de réservation de places dans les grands taxis intra-ville.**

Blasti est un projet de fin d'année (PFA) qui vise à faciliter les déplacements en grand taxi partagé. Les passagers pourront rechercher un taxi sur leur trajet, réserver une à six places et suivre son arrivée. Les chauffeurs pourront déclarer leurs trajets, gérer les demandes et suivre les places disponibles.

## Fonctionnalités prévues

- **Passagers :** recherche par trajet, réservation, suivi en temps réel, historique et évaluation.
- **Chauffeurs :** gestion des trajets et des réservations, localisation, prises en charge et déposes.
- **Administration :** gestion des chauffeurs, véhicules, agréments, villes et lignes, modération et statistiques.
- **Fiabilité :** gestion des places en cas de réservations simultanées, notifications et reprise après une coupure réseau.
- **Analyse de la demande :** prévisions par ligne et créneau horaire à partir de données disponibles ou simulées.

Le paiement en espèces est prévu pour la première version.

## Technologies envisagées

- **Applications mobiles :** Flutter et Dart, avec une base de code partagée pour les applications client et chauffeur.
- **Backend :** Java et Spring Boot, avec API REST et WebSocket.
- **Données :** PostgreSQL, PostGIS et Redis.
- **Cartographie et itinéraires :** OpenStreetMap et OSRM.
- **Notifications :** Firebase Cloud Messaging.
- **Back-office et déploiement :** Spring MVC/Thymeleaf et Docker.

## État du projet

Le projet est en phase de planification. Les fonctionnalités et technologies ci-dessus sont prévues et restent à valider dans le cahier des charges.

Le [plan complet de développement](docs/PLANNING.md) présente l'architecture, les exigences, les tests, les jalons et une répartition de travail 50/50 sur deux développeurs.

Le [plan microservices](docs/PLANNING-MICROSERVICES.md) en est la variante pour un travail séparé des deux développeurs : services par propriétaire, contrats consommateur, budget et calendrier sur 16 semaines.

## Contributeurs

- **BAGHDAD Mohamed**
- **BAAKKA Monssef**

Projet PFA — EMSI Rabat, 5IIR, option Développement Digital et Systèmes d'Information.
