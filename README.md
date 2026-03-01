# TP 2.3 – Gérer les conflits

Ce dépôt contient `index.html` et `style.css` pour pratiquer la résolution de conflits.

## Tâches

1. Sur `main` : modifier `index.html` (le `<h1>` ou le `<p>`), commiter
2. Créer une branche `feature/update-home`
3. Dans cette branche, modifier **la même zone** dans `index.html` (version différente)
4. Commiter sur `feature/update-home`
5. Revenir sur `main` et lancer `git merge feature/update-home` → **conflit !**
6. Repérer les marqueurs `<<<<<<<`, `=======`, `>>>>>>>`
7. Résoudre manuellement, `git add index.html`, finaliser le merge
8. Vérifier l'historique et supprimer la branche

## Astuce : identifier un conflit

Après le merge qui échoue :
```bash
git status         # montre les fichiers en conflit
git diff           # montre les marqueurs de conflit
```
