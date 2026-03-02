# TP 2.3 – Gérer les conflits Git ⚔️

## Ce qui est préconfiguré dans ce dépôt

- **`main`** : contient `index.html` avec `<h1>Bienvenue sur Mon Projet - Version Principale</h1>`
- **`feature/update-home`** : contient `index.html` avec `<h1>Bienvenue - Nouveau Design Feature</h1>` (modifie la même ligne → conflit garanti !)

## Tâches

1. Cloner le dépôt et se placer sur `main`
2. Lancer `git merge feature/update-home` → conflit !
3. Repérer les marqueurs `<<<<<<<`, `=======`, `>>>>>>>`
4. Ouvrir `index.html`, résoudre manuellement le conflit (choisir ou combiner les deux versions)
5. `git add index.html`
6. `git commit` pour finaliser le merge
7. Vérifier l'historique avec `git log --graph --oneline --all`
8. Supprimer la branche `feature/update-home`

## Pourquoi y a-t-il un conflit ?

`main` et `feature/update-home` partent du **même commit de base** mais modifient **la même ligne** dans `index.html` (le `<h1>`).
Git ne peut pas choisir automatiquement → il vous demande de décider.
