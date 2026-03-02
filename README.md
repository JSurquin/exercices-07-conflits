# TP 2.3 – Gérer les conflits

Ce dépôt contient `index.html` et `style.css` pour pratiquer la résolution de conflits.

## Tâches

1. Sur `main` : sans commiter
2. Créer une branche `feature/update-home` modifier `index.html` (le `<h1>` ou le `<p>`), et comittez
3. Commiter sur `feature/update-home`
4. Revenez sur main
5. Créer une branche `feature/update-home2` basé sur main modifier `index.html` (le `<h1>` ou le `<p>`), et comittez
6. Revenir sur `main` et lancer `git merge feature/update-home` → ok puis update-home2 **conflit** !
7. Repérer les marqueurs `<<<<<<<`, `=======`, `>>>>>>>`
8. Résoudre manuellement, `git add index.html`, finaliser le merge
9. Vérifier l'historique et supprimer la branche

## Astuce : identifier un conflit

Après le merge qui échoue :
```bash
git status         # montre les fichiers en conflit
git diff           # montre les marqueurs de conflit
```
