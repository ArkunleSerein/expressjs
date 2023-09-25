# ExpressJS

Ce repos contient une appli express.js de type " Hello world " pour tester le déploiement.

## Install

```bash
git clone https://github.com/ArkunleSerein/expressjs
cd expressjs
npm install
```

## Utilisation

```bash
node app.js
```

[http://localhost:3000](http://localhost:3000)

## Déploiement sur Render.com

Prérequis : un compte Github.

- (optionnel) Forkez un repository ou créez en un nouveau sur Github si nécessaire
- Créez un compte sur [https://render.com/](https://render.com/)
- Créez un nouveau web service en cliquant sur l'icône "+".
- Cliquez sur "connect account" dans la serction "Github" à droite
- Vous vous retrouvez sur le site Github
- Tapez votre mot de passe Github
- selectionnez le repository que vous voulez publier
- Confirmez les permissions accordées
  Vous revenez sur le site de Render
- Cliquez sur le bouton "connect" du repository que vous voulez publier
- Remplissez les champs avec les données suivantes :

  ```bash
  General:

  Name: [sous-domaine-de-votre-appli]
  Region: Frankfurt (EU Central)
  Instance Type: Free
  Branch: main
  Root Directory: <nc>
  Build Command: npm install
  Start Command: node app.js
  ```

  Remplacez par le `[sous-domaine-de-votre-appli]` par le sous-domaine souhaité.
  Exemple : `foo` donnera `https://foo.onrender.com`

- Valider la configuration puis visiter le lien quand le build est terminé

### Mise à jour sur render.com

- Mettez le code à jour en local
- Commitez votre code avec `git add` et `git commit`
- Poussez votre code sur Github avec `git push`
- Vérifier que le code est à jour sur render.com
