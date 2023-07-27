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