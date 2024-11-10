# Rendu Integration & Preprocessor

Ce projet de site web est développé avec HTML, SCSS (Sass). Le style est organisé avec des partials SCSS et des mixins pour faciliter la maintenance et la réutilisabilité du code.

## Table des matières

1. [Installation](#installation)
2. [Structure du Projet](#structure-du-projet)
3. [Utilisation de Sass](#utilisation-de-sass)
4. [Commandes Sass](#commandes-sass)
5. [Exécution du projet](#exécution-du-projet)

---

### Installation

1. **Cloner le dépôt** : Clonez le dépôt sur votre machine locale :
   ```bash
   git clone https://github.com/TerukiIIM/Integration-preprocessor.git
   ```

2. **Installer Node.js et npm** : Assurez-vous d’avoir [Node.js et npm](https://nodejs.org/) installés. Vous pouvez vérifier en exécutant :
   ```bash
   node -v
   npm -v
   ```

3. **Installer Sass** : Nous utilisons Dart Sass pour compiler le code SCSS en CSS. Vous pouvez installer Sass globalement avec npm :
   ```bash
   npm install -g sass
   ```

   Cela vous permet d'utiliser la commande `sass` dans le terminal pour compiler les fichiers Sass.
   Ps: si ça ne fonctionne pas avec le terminal powershell, essayer avec l'invite de commande (CMD)

### Structure du Projet

Le projet est organisé comme suit :

```
.
├── _mixins.scss             # Partials pour les mixins
├── _variables.scss          # Partials pour les variables de couleur, etc.
├── index.html               # Page principale du site
├── README.md                # Documentation du projet
└── style.scss               # Point d'entrée pour le code SCSS
```

### Utilisation de Sass

Les styles de ce projet sont écrits en SCSS, une syntaxe de Sass, pour structurer et modulariser les fichiers CSS. Nous avons organisé les styles en plusieurs partials (fichiers SCSS) afin de mieux structurer le code :

- **Variables** : `_variables.scss` contient les couleurs, polices et autres valeurs réutilisables.
- **Mixins** : `_mixins.scss` regroupe des mixins pour le style de boutons, le flexbox, et autres utilitaires.

### Commandes Sass

Pour compiler les fichiers SCSS en CSS, utilisez les commandes suivantes :

- **Compilation unique** :
  ```bash
  sass style.scss style.css
  ```

- **Compilation en mode watch** : Pour surveiller les changements et compiler automatiquement, utilisez :
  ```bash
  sass --watch style.scss style.css
  ```

Ces commandes prennent `style.scss` comme point d'entrée, puis compilent tous les partials importés dans `style.css`.

### Exécution du projet

1. **Ouvrir le fichier HTML** : Vous pouvez simplement ouvrir `index.html` dans votre navigateur pour voir le site en action. Les styles compilés seront appliqués automatiquement si vous utilisez la commande watch de Sass.

2. **Déploiement** : Si vous souhaitez déployer le site, assurez-vous que tous les fichiers nécessaires (HTML, CSS compilé, images, etc.) sont inclus dans le dossier que vous envoyez vers votre serveur de production.

---

## Auteur

Développé par Jérôme ZHAO, étudiant