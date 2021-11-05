# first-mvc-with-admin
first MVC with administration in PHP 7 procedural - MariaDB with InnoDB engine - Session management

## GIT

Connectez-vous sur Github et rendez-vous à l'adresse:

    https://github.com/WebDevCF2m2021/first-mvc-with-admin

1. Créez un fork en haut à droite sur votre espace personnelle


    github.com/mikhawa/first-mvc-with-admin

2. Copiez le lien de votre fork (ce termine en .git)

sur code -> https


    github.com/mikhawa/first-mvc-with-admin.git

3. Ouvrez git bash à l'endroit ou vous voulez cloner votre fork (Attention de ne pas être dans un autre projet git !)


    git clone https://github.com/mikhawa/first-mvc-with-admin.git

4. Entrez dans le dossier en utilisant `cd` (change directory)


    cd first-mvc-with-admin

Vous devriez vous trouver sur la barnche `main` , pour le vérifier:


    git branch

5. Vous devez retourner sur le git d'origine sur github et copier le code, ensuite ajouter le dans le bash sous le nom `upstream` :


    git remote add upstream https://github.com/WebDevCF2m2021/first-mvc-with-admin.git

6. Vérifiez vos remotes (serveurs distants) en utilisant la commande

    git remote -v

7. Créez des branches

## Structure

### Nos dossiers de bases 

Ce sont nos dossier "non MVC" mise à part le contrôleur frontal se trouvant dans :
- public/index.php

`/.git`

Contient nos changements Git, ne jamais envoyer sur le FTP

`/data` 

Nos données de préparation et de création du site, peut se trouver sur github (ou pas!), par contre inutile en FTP

`/public` 

C'est le seul dossier qui sera accessible à l'utilisateur de votre site, c'est ici que l'on mettra le contrôleur frontal, ainsi que les dossiers publiques tels que `css`, `js`, `img` etc...

- index.php -> notre front controller

### Nos dossiers MVC

`MVC` est un `design pattern` (patron de conception) qui signifie 
- Model
- View
- Controller

C'est une manière de diviser le code pour :

1. Avoir une structure commune sur un projet
2. Déléguer les tâches sans risque d'écrasement de fichiers
3. Pouvoir séparer en logique métier la structure du site (le webdesigner travaille sur les vues, les webdeveloppers travaillent sur les modèles et les contrôleurs, le chef de projet impose la structure)

![Modèle MVC PHP](https://raw.githubusercontent.com/mikhawa/MVC-procedural-with-upload/main/datas/MVC.png)


https://fr.wikipedia.org/wiki/Mod%C3%A8le-vue-contr%C3%B4leur


## Virtualhost

On crée en local un virtualhost avec Wamp (ou autre).

Attention cette adresse pointe bien vers le dossier `public` du site :

`...votre_chemin.../first-mvc-with-admin/public`

pour avoir une adresse de type:

http://first-mvc-with-admin:8080/

