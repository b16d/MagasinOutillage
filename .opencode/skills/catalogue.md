# Skill — Domaine Catalogue Produits

## Contexte
Le domaine catalogue gère les produits du magasin d'outillage :
références, noms, descriptions, prix, stock et catégories.

## Règles métier
- Un produit peut être actif ou inactif (soft delete)
- Un produit appartient à une catégorie
- Un produit a une référence unique
- Le prix d'un produit est toujours strictement positif
- Le stock est un entier positif ou nul
