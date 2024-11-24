# Gestion des branches

## Nouvelle feature

Si vous avez une nouvelle feature à réaliser ou une correction de bug
Veillez à être initialement sur la branche `main`

- `git checkout main`
- `git pull origin main`

On crée ensuite notre nouvelle branche à partir de main

- `git checkout -b feat/nomenrapportaveccequejevaisfaire`
  ou
- `git checkout -b fix/nomenrapportaveccequejevaisfaire`

Vous développez maintenant sur votre branche.
Quand votre développement de votre nouvelle feature ou de votre bug est terminé

- `git add lefichierquejaimodifier`
  Exemple:
- `git add ./src/components/Footer.js`

On commit ensuite

- `git commit -m "feat: cequejaifaitdanslesgrandeslignes"`
  ou
- `git commit -m "fix: cequejaicorrigédanslesgrandeslignes"`

On envoie ensuite notre branche et notre commit sur le serveur distant

- `git push origin feat/nomdemabranche`
  ou
- `git push origin fix/nomdemabranche`

Ensuite, allez sur l'onglet `Pull Request` de votre Repository
exemple: https://github.com/NicolasMoulin1/portfolio/pulls

Créez votre PR (PULL REQUEST) à partir de votre branche avec main en destination.
Il reste plus qu'à merger la PR quand vous êtes certain que vos changements sont bons. (Généralement, un autre développeur regarde notre PR et vérifie que notre code est correct et respecte les standards du projet et n'apporte pas de risque de bug)
