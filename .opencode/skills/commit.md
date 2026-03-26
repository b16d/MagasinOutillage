# Skill — Commit

## Déclenchement
Ce skill s'applique avant chaque commit.

## Règles de branche
- Avant chaque nouvelle tâche, toujours :
  1. `git checkout main`
  2. `git pull`
  3. `git checkout -b {nom-de-branche}`
- Nom de branche : suivre le format `{type}/{description-courte}` (ex: `feat/catalogue-product-entity`, `fix/price-validation`)
- Types autorisés : `feat`, `fix`, `refactor`, `test`, `docs`, `chore`

## Format du commit
- Message court : 50 caractères maximum, en français, à l'impératif (ex: "Ajoute l'entité Product")
- Description : liste des changements effectués (fichiers modifiés, ajoutés, supprimés)
- Format complet :
  ```
  {message court}

  - {changement 1}
  - {changement 2}
  - {changement 3}
  ```

## Interdictions
- Ne jamais faire de `git push`
- Ne jamais commiter directement sur `main` ou `master`
- Ne jamais utiliser `--no-verify`
