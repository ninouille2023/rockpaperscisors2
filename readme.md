# Les commandes de base de Github

## Première étape : initialiser un repo

* Créez dans Github, un nouveau repository
* Nommez le comme vous le souhaitez
* Vous pouvez choisir sa visibilité :
    * Public : Si vous souhaitez que tout le monde puisse y avoir accès
    * Private : Si vous souhaitez être le seul à y accéder
* La description est optionnelle : remplissez-la si vous le souhaitez
* Allez en bas de page, cliquez sur "Create repository"

Votre repository est maintenant créé, vous allez pouvoir faire votre premier commit.

## Faire son premier commit

Vous allez vous rendre compte qu'il y a un petit encadré nommé "Quick setup" qui vous propose deux possibilités : HTTPS et SSH.

Si ce n'est pas fait par défaut, choisissez HTTPS.

### Initialisation de Github sur votre machine

Sur Visual Studio Code :
* Ouvrez un terminal (3 possibilités)
  * Menu affichage > Terminal
  * CTRL + ù
  * En bas à gauche, vous avez une icone triangle et rond. Cliquez dessus

Initialisez github sur le dossier qui est ouvert avec la commande  ``git init`` 
Une fois que git est initialisé, vous allez devoir indiquer quel(s) fichier(s) vous souhaitez envoyer sur github. Pour cela :
* ``git add *`` Pour ajouter TOUS les fichier
* ``git add nomDuFichier`` pour ajouter UN fichier en particulier.

Pour info, vous ne devez PAS entrer vous-même le nom complet du dossier ou du fichier. Ca augmente le risque d'erreur. Au lieu d'écrire le nom complet vous-mêmes, vous devez écrire seulement la ou les premières lettres et appuyer sur la touche ``tab``

Dans le cas ou il existe plusieurs fichiers qui commencent avec les mêmes lettres, il vous suffit de continuer à appuyer sur ``tab`` jusqu'à arriver au bon fichier.

Si vous avez plusieurs fichiers à ajouter, MAIS que vous ne souhaitez pas ajouter tous les fichiers qui se trouvent dans votre dossier de travail, vous pouvez faire plusieurs fois ``git add nomDuFichier``

#### En résumé

* ``git init`` - Pour initaliser le repo github
* ``git add NomDuFichier`` - Pour ajouter un fichier

## Exercice
* Initialisez le repo github sur VSCode
* Ajoutez le fichier readme

### Faire la liaison avec le repo distant
Vous venez d'initialiser git sur votre machine, mais il ne sait pas encore qu'il doit être lié à votre repository distant.
Pour cela, vous allez devoir connecter l'origine à)votre repository distant.

Commençons par ajouter un petit message qui précise ce qu'on a fait comme modification/ajout/suppression

* ``git commit -m "explication du commit"`` 

exemple :
* ``git commit -m "Ajout du fichier readme"``

Une fois que le message de commit est définir, on va choisir la branche sur laquelle on va travailler.

Lorsque vous souhaitez stocker vos fichiers sur github, si vous le souhaitez, vous pouvez stocker différentes versions de vos fichiers. Cela s'appelle des branches.

La branche principale sur laquelle vos fichiers sont enregistrés s'appelle "main".

* ``git branch -m main``

Cette commande indique qu'on sélectionne la branche "main".

Il est maintenant temps de connecter votre repo local (votre machine) à votre repo distant (github). Pour cela, utilisez cette commande :
* ``git remote add origin LIEN_DE_VOTRE_REPO``

Exemple :
* ``git remote add origin https://github.com/JackAdamsJenkins/rockpaperscisors.git``

Maintenant que le repo local et distant sont connectés, il vous reste à envoyer vos fichiers sur github. Cela se fait avec la commande ``git push -u origin main``

## En résumé
Voici les commandes a lancer :
* ``git init`` pour initialiser le repo github
* ``git add NomDuFichier`` pour ajouter un fichier
* ``git commit -m "Nom du commit"`` pour ajouter une description de la modification/ajout
* ``git branch -m main`` pour choisir la branche principale
* ``git remote add origin URL_REPO_GITHUB`` pour connecter le repo local et distant
* ``git push -u origin main`` pour envoyer les modification à github

## Informations :
Les commandes ``git init``, ``git branch`` et ``git remote add origin`` sont à lancer UNE SEULE FOIS au moment de l'initalisation du repo. 

Une fois que ces commandes ont été faites, pendant le reste du développement de votre projet, vous pouvez utiliser les commandes suivantes : ``git commit -m "message de modification"``, ``git add NomDuFichierModifié``, ``git push``.

C'est ces trois commandes que vous utiliserez à chaque fois :
* ``git commit -m "message de modification"``
* ``git add nomDuFichierModifié``
* ``git push``