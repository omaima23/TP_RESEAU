# BE_Prog_C_Reseau
## BE Programmation C et réseau - 3 IMACS

L'objectif du BE est de réaliser une application distribuée de boîtes aux lettres sur Internet, utilisant l'API socket. Le langage de programmation utilisé est le C. Le travail à réaliser en TP est décomposé en 2 parties : 
  - la 1ère partie est principalement dédiée à la prise en main de l’API socket avec comme objectif de mettre en oeuvre l’application « tsock » utilisée dans le TP d’introduction aux réseaux, 
  - la 2ème partie traite vise le développement du système de boites aux lettres suscité. 

Les détails du sujet du BE est accessible :  https://urlz.fr/98al


## Contenu du dépôt « template » fourni
Ce dépôt inclut le code source initial fourni pour démarrer le BE ainsi qu’un fichier nous permettant de suivre votre avancement. Plus précisément : 
  - README.md qui notamment décrit la préparation de l’environnement de travail et le suivi des versions de votre travail; 
  - tsock_v0.c : code initial fourni pour démarrer la première partie du BE. 
  - avancement.md qui explicite votre avancement sur les différentes parties du BE. Ce point est à renseigner à chaque fin d’étape et par défaut à la fin de chaque séance de TP 


## Création du dépôt BE prog. C &  Réseau  

1. Création d’un compte git étudiant : Si vous ne disposez pas d’un compte git, connectez vous sur http://github.com/ et créez un compte par binôme. 

2. Afin d’être capable de mettre à jour le code que vous aurez produit sur le dépôt central Github, il vous faudra créer un jeton d’accès qui jouera le rôle de mot de passe. Veuillez le sauvegarder, car il vous le sera demandé lors de l'accès au dépôt central. Pour ce faire, veuillez suivre les étapes décrites : https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token

3. Création d’un dépôt Etudiant sur GitHub pour le BE prog. C & réseau
  
   Créer une copie du dépôt template enseignant : https://github.com/rezo-insat/BE_Prog_C_Reseau.git , en vous y rendant et en cliquant sur le bouton « use this template » situé dans le coin en haut, plutôt à droite de la page. Il est conseillé de le choisir comme dépôt privé. Dans ce cas, veuillez rajouter le compte : rezo-insat comme collaborateur afin de permettre à vos enseignants d'accéder à votre dépôt. Pour ce faire, sélectionner le bouton "settings" puis "collaborators" et rajouter comme utilisateur : rezo-insat. La marche à suivre est décrite ci-après : https://docs.github.com/en/organizations/managing-access-to-your-organizations-repositories/adding-outside-collaborators-to-repositories-in-your-organization

4. Créer un clone local de votre dépôt Github, i.e. une copie locale du dépôt sur votre compte insa. 
  
    cliquer sur le bouton « code » de votre dépôt, copier l’URL qui permet de l’identifier. 
	Ouvrir un terminal de votre machine. En vous plaçant dans le répertoire de travail de votre choix, taper depuis le terminal :

        git clone <url de votre dépôt>

    Vous avez désormais une copie locale de votre dépôt, que vous pouvez mettre à jour et modifier à volonté au gré de votre avancement sur le BE. 

5. Afin de nous permettre d’avoir accès à votre dépôt, merci de bien vouloir renseigner l'URL de votre dépôt sur le fichier (accessible depuis "Lien vers le fichier dépôts étudiants") se trouvant sur moodle (au bas de la section 3: "Bureau d'étude (BE) Prog C et Réseau").

## Build et lancement de tsock

Pour compiler et générer l’exécutable tsock depuis le code source fourni, taper :

    gcc tsock_v0.c -o tsock

Pour lancer l’exécutable, à titre d’exemple, en tant que puit :

    ./tsock -p <numero de port> 


## Suivi de versions de votre travail du BE

Vous pouvez travailler comme vous le souhaitez sur le contenu du répertoire local. Vous pouvez mettre à jour les fichiers existants, rajouter d’autres ainsi que des dossiers et en retirer certains à votre guise. 

Pour répercuter les changements que vous faites sur votre répertoire de travail local sur le dépôt central GitHub, sur votre terminal, taper :
 
    git add .
    git commit -m «un message décrivant la mise à jour»
    git push


- Creation d’une branche pour la partie 2 du BE
Au moment du démarrage de la partie 2, vous créerez une nouvelle branche à votre projet, à partir de laquelle vous développerez la partie 2. Sur votre dépôt, les deux parties de votre travail  coexisteront sur deux branches différentes. 

Créer une branche « BAL » , en tapant la commande suivante sur votre terminal :

    git branch BAL

Positionner vous sur la branche BAL 

    git checkout BAL


Positionner la branch BAL à partir de la branche « par défaut »
   
    git push --set-upstream origin BAL


Vous pouvez ensuite travailler en local sur la partie 2 du projet.

Au moment de pousser votre travail sur la branche 

    git add .
    git commit -m « descriptif de la nouvelle version »
    git push


## Suivi de votre avancement 

Un fichier avancement.md vous est fourni avec des étapes prédéfinies et discutées en TDs. A chaque étape terminée, veuillez le mettre à jour en conséquence. Par défaut, mettez à jour ce fichier en fin de séance. 


## Liens utiles 

Aide pour la création d’un dépôt depuis un template : https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template
