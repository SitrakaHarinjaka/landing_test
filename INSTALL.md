# Guide d'installation du projet

## Configuration requise

Version Node: 20.10+

Si vous utiliser l'outil nvm, il suffit de lancer la commande
```bash
nvm use
```

## Mode développpement

Installation des paquets

```bash
npm i
// ou
yarn install
```

Puis lancer le projet

```bash
npm run dev
// ou
yarn dev
```

## Mode production

Construire l'app en mode production

```bash
# npm
npm run build

# yarn
yarn build
```

Prévisualiser l'app après l'étape de construction

```bash
# npm
npm run preview

# yarn
yarn preview
```