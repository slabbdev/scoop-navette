# main-bucket draft — dossier prêt, PR à ouvrir quand la notabilité suivra

Le [bucket main de Scoop](https://github.com/ScoopInstaller/Main) donne le vrai
`scoop install navette` sans `bucket add`. Son critère d'entrée :
« reasonably well-known and widely used developer tool », quantifié en
**≥ 500 étoiles et ≥ 150 forks** GitHub — navette n'y est pas encore.

Quand le seuil sera atteint :

1. Ouvrir une PR sur `ScoopInstaller/Main` ajoutant `bucket/navette.json` (ce dossier).
2. Corps de PR prêt : [PR-BODY.md](PR-BODY.md) (checklist officielle pré-remplie).
3. Le nom `navette` est libre (vérifié 2026-10-08 : aucun `navette.json` dans le bucket).
4. `checkver: github` + `autoupdate` permettent à l'automatisation Scoop de suivre
   les releases sans intervention — rien à maintenir de notre côté après merge.

⚠️ Le manifest de CE dossier est une copie figée : ne pas oublier de le resynchroniser
sur la dernière release le jour de la PR (le `bucket/navette.json` de la racine, lui,
est auto-bumpé).
