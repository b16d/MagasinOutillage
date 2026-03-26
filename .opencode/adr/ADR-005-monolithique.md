# ADR-005 — Architecture Monolithique

## Statut
Accepté

## Contexte
Le projet est en phase initiale. Le périmètre fonctionnel est limité à un seul domaine (catalogue produits).
Les alternatives considérées sont l'architecture monolithique et les microservices.

## Décision
Adopter une architecture monolithique pour ce projet.

## Conséquences
- Simplicité de développement, de déploiement et de débogage
- Un seul processus à démarrer et à maintenir
- Pas de complexité liée à la communication inter-services (HTTP, messaging)
- Scalabilité horizontale plus limitée qu'une architecture microservices
- En cas de forte croissance, une migration vers des microservices sera envisageable grâce à la Clean Architecture adoptée
