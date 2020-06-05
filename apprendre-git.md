## Apprendre Git

C'est le nerf de la guerre, aussi important qu'un language, Git est un logiciel de versionning, il permet de travailler en collaboration en entreprise ou en coopérative avec vos collègues, amis, co-apprenants.
Il s'agit du plus utilisé et du plus accessible, cependant, il s'agit de notions complexes qui vont vous demander rigueur et attention.

**À quoi ça sert concrètement?**

Git va vous permettre de travailler en collaboration avec les formateurs et vos collègues apprenants. En effet, grâce à Git vous pouvez héberger vos fichiers, récupérer les fichiers sources d'un projet, les modifier, vous joindre au travail d'un de vos camarade.

Dans le cadre de notre formation vous serez amenés à utiliser Git tout les jours, en effet nous allons vous demander de trouver vos consignes sur la plateforme et de rendre vos travaux sur cette même plateforme.
Nous verrons plus loin dans cette introduction comment procéder.

### **1. Lexique**

Pour vous donner un petit coup de pouce voici déjà un lexique des termes les plus courants rencontrés:

- **Repository**: Vous l'avez déjà un peu approché pendant votre test, un repository ou "dépôt" en français, sert à déposer toute les informations / fichiers / éléments graphiques nécessaires à votre projet 

- **Clone:** Un clone est la version téléchargée du repository qui vous est propre et qui se situe en local dans votre ordinateur. Vous pouvez le mettre à jour avec un *pull* et ajouter du contenu (voir le chapitre workflow)

- **Branche:** Une branche dans git c'est un peu comme les 4 branches d'une fourchette, on part du même point (la master, qui équivaudrait au manche de la fourchette) suivi des branches dans son prolongement prenant chacune un autre chemin. Chaque branche que vous créez part donc d'un tronc commun (la master par exemple) et crée une version qui lui est propre et sur laquelle vous pouvez travailler sans risquer d'altérer le contenu de la branche master.
Par convention on ne pousse un travail sur la master que lorsqu'il est complètement terminé. 
Vous pouvez créer une branche portant le nom "développement" sur laquelle vous pourrez mettre l'avancement intermédiaire de votre travail, et ainsi qu'une déviant de développement, portant votre nom, vous permettant de travailler sur une feature sans empiéter sur le travail de vos camarade dans le cadre d'un travail de groupe, ou simplement par soucis du détail si vous travaillez seul et que vous craignez de faire une mauvaise manipulation.

- **Fetch:** va chercher les nouvelles données potentielles sur un repository distant 

- **Pull:** va chercher et intègre les nouvelles données potentielles sur un repository distant pour les intégrer à celui que vous possédez en local sur votre ordinateur

- **Changes:** tout changement que vous avez créé sur votre version locale du repo, ces changements sont soumis à validation, nous verrons plus tard une manière simple de les valider.

- **Staged changes:** tout changement que vous avez créés et validés sur votre version locale du repository

- **Commit:** un commit contient les changements que vous avez validés, il possède un code de référence qui permet d'être retrouvé et donc de pouvoir observer les différences entre la version précédente du code et la version du retenue par le commit. Il possède un code, un nom, une description. Nous allons simplement nous atterder sur le nom dans le cadre de notre formation: idéalement le nom doit comporter l'objet du travail (par exemple pour une nouvelle fonctionnalité on l'appellera : feature; le nom de la fonctionnalité; et la modification apportée à cette fonctionnalité)

*Exemple d'un nom de commit conforme:*

`"feature/index: creation d'index.html"`

- **Push:** Après avoir commit votre travail, il est présent dans la mémoire git de votre dossier en local, pour l'uploader sur la mémoire distante il vous faut "pousser" (= push en anglais), le push permet donc de mettre à disposition en ligne le travail que vous avez effectué en local. 

### **2. Usage idéal:**

***Le matin à 9h:*** 
1. Vous allez fetch le repos distant (celui de la sirius-school) afin de détecter les éventuels changements
2. Vous allez pull le résultat du fetch et l'intégrer à votre repo

***Lorsque vous travaillez:***

1. Vous écrivez vos changements et les sauvegardez via la commande CTRL+S sur l'ensemble de vos fichiers ou ouvrez l'onglet file et clickez sur "save all" -> leur état est labellé sur "Changes"
2. Vous validez les changements que vous avez effectués -> leur état est labellé "Staged Changes"
3. Vous commitez vos fichiers, le nom de commit est obligatoire, un champs s'ouvre automatiquement dans l'interface à cet effet: écrivez le nom du commit et validez avec le v 
4. Maintenant vous pouvez push vos fichiers cliquez sur les trois petits points, sélectionnez push
5. Vos fichiers sont uploadés sur github

### **3. Exemple avec l'interface VSCode pour Git**
Nous verrons dans les semaines à venir l'usage plus poussé de Git et Github, mais pour l'instant contentez vous de l'utiliser via l'interface Gitdesktop ou via VScode en clickant sur cette icone dans votre barre d'outil pour accéder aux commande git, la pastille indique le nombre de changement trackés par Git:

![Imgur](https://i.imgur.com/bMFK1iz.png)

Lorsque vous clickez sur cet outil vous obtenez une interface telle que celle-ci:

![Imgur](https://i.imgur.com/ftCfnso.png)

1. Le point 1 reprend les changements que vous avez apporté à vos fichiers mais que vous n'avez pas encore signalé comme changement à retenir pour git. Pour confirmer à git qu'il doit bien prendre en compte les changements fait à ces fichiers il suffit de passer son curseur sur le nom du fichier, un plus apparait, clickez dessus afin de les labeller "Staged Changes"

2. Les changements une fois dans Staged Changes peuvent être "commité", écrivez le nom du commit tel que je vous l'ai expliqué plus haut.

3. Une fois le message écrit vous pouvez clicker sur le point 3, comme vous le voyez il s'agit d'un petit V de validation. Clicker dessus enregistrera sur la version locale de votre repository (le dossier dans lequel vous travaillés) les changements, pour les envoyer sur le site GitHub et le rendre disponnible à tous il vous faudra "push" votre travail après l'avoir commité

**Mais comment on push?**

4. Clickez sur les trois petits points, vous verrez apparaître cette interface:

![Imgur](https://i.imgur.com/MQ5Xlcd.png)

5. Clickez sur push

6. Et voilà votre travail se trouve sur votre repository "fork" de la semaine! Il nous est donc accessible à la correction!


### **4. Exercice obligatoire**

Pour débuter un petit jeu permettant de visualiser les commandes (allez le plus loin possible, communiquez moi l'étape à laquele vous êtes arrivé accompagné d'un screenshot de cette étape):

https://learngitbranching.js.org/?locale=fr_FR

## **Forker un repository et le mettre à jour**

Qu'est ce qu'un fork me direz vous?
Plutôt que de cloner le dossier de la semaine sur votre ordinateur, nous vous demanderons de le "forker". C'est à dire de créer une copie du repository (ou dépôt en français) qui vous sera propre et vous permettra de travailler en toute sécurité sans la crainte d'une mauvaise manipulation entrainant une altération du Repo de la school!

Pour ce faire clickez sur l'onglet fork en haut à droite de votre interface:

![Imgur](https://i.imgur.com/tzLFdEM.png)

Voilà, vous possédez désormais une copie personnelle du dépôt de notre première semaine dans votre onglet repositories que vous pouvez cloner sur votre ordinateur.

Pour ce faire: 

1. Allez dans "your repositories" sélectionnez votre fork, clickez sur "clone or download" 
![Imgur](https://i.imgur.com/oAgknwA.png)

2. Clickez ensuite sur Open in Desktop

![Imgur](https://i.imgur.com/QreDb5H.png)

3. Clickez sur Ouvrir Github Desktop dans la boite d'alerte:
![Imgur](https://i.imgur.com/TmPT756.png)

4. Git desktop va alors se lancer et se charger de télécharger votre clone sur votre ordinateur: Par défaut le chemin vers ce fichier sera documents/Github/le-nom-du-fork, vous pouvez décider de modifier le chemin de destination en clickant sur choose (par exemple Bureau/le-nom-du-fork pour l'avoir directement sur votre bureau) ensuite clickez sur clone

![Imgur](https://i.imgur.com/h0pDiX7.png)

5. Et voilà votre dossier est cloné sur votre ordinateur !


Chaque jour, veillez à mettre à jour votre Fork, en effet, nous pourrions y apporter des modifications qui ne se retrouveront pas automatiquement sur votre version du dépôt. 

### **Comment mettre son fork à jour**

Il n'existe malheureusement pas d'outils visuels concernant la mise à jour de votre fork. 
Pour ce faire il vous faudra donc avoir recours à votre terminal de commande.
Ouvrez git bash dans l'onglet terminal de VSCode, tirez la petite languette bleue en bas de votre écran vers le haut en maintenant le click gauche de votre souris et remontant vers le haut la flèche:

![Imgur](https://i.imgur.com/2PTM1q8.png)


**Vous obtenez ce résultat:**


![Imgur](https://i.imgur.com/gmGqMnF.png)



Le chemin relatif du dossier dans lequel vous êtes en train de travailler est indiqué, ainsi que le nom de la branche.
Pour apprendre à naviguer dans votre terminal référez vous au fichier de théorie apprendre-le-terminal <!-- Ajouter le lien vers la théorie -->

**Mettre à jour son fork: on y est**

Comme je vous l'ai dis, pour mettre à jour votre fork vous allez devoir passer par le terminal.
Pas de panique, je vais vous fournir un pense bête contenant la commande à copier coller dedans.

Il s'agit en réalité de demander à votre Git, installé sur votre PC, d'aller chercher sur le repository de la sirius-school, les éventuels changements qui y sont apporté et de les ajouter à votre propre version du fork.

Pour ce faire entrez cette commande à chaque nouvelle semaine que vous forkez:

# Ajouter l'upstream 
L'upstream c'est le serveur distant sur lequel est stocké le repo à l'origine de votre fork, il faut indiquer à votre ordinateur où il doit aller chercher l'information, pour ce faire tapez cette commande dans le terminal en remplaçant l'url d'exemple par l'url du repository d'origine:

`git remote add upstream https://url-du-repo-de-la-semaine.git`
# Lister serveurs distants pour vérifier l'ajout de upstream

`git remote -v`

# Récupèrer les commits de l'upstream

`git fetch upstream`

# Intégrer les commits à ma version du repo
`git pull`

N'oubliez pas d'enregistrer les changements en local mais également sur votre repo Github, voir le chapitre "Workflow" ici plus haut.


# Faire une pull request

Une fois vos travaux terminés nous vous demanderons de nous envoyer une pull request.
Mais qu'est ce donc que cela encore!
Une pull request permet d'avertir le propriétaire du repository orginel, que vous avez apporté une modification à votre version du repo. En gros que vous avez collaboré au projet.
La pull request permet de comparer les changements effectués grâce à une interface spécifiant le code originel et le code apporté par le collaborateur (assigné).
Il possède un champs "commentaire" sous chaque changement qui permet au reviewer (le correcteur) de proposer une solution tierse ou de commenter la solution proposée, dans notre cas il nous permettra de corriger votre travail et de vous laisser des propositions d'améliorations.

Pour réaliser une pull request: effectuez, validez, pushez vos changements sur votre repository distant (Github). 

1. Ouvrez votre repository
2. Clickez sur pull request

![Imgur](https://i.imgur.com/rfTNbH2.png)

3. CLickez sur new pull request

 ![Imgur](https://i.imgur.com/IbQsuwd.png)

4. Clickez sur create pull request

![Imgur](https://i.imgur.com/6qQjNwU.png)

5. Remplissez le formulaires: 

![Imgur](https://i.imgur.com/O6Zff4I.png)

- En point 1: Indiquez le titre de l'exercice
- En point 2:  Laissez une description de ce que vous avez réalisés, un guide d'utilisation si nécessaire, les difficultés que vous avez rencontrés, toute information qui vous semble pertinente de nous communiquer
- En point 3: sélectionnez la personne à qui demander une review: en l'occurence Jeremy ou Julie
- Sélectionnez les assignés au projet: vous et toute personne y ayant collaboré
- Sélectionnez le label correspondant à votre travail (par exemple dans ce cas ci il s'agit de documentation mais vous pourriez rencontrer un bug et nous envoyer une pull request labellée bug afin que nous puissions travailler dessus ensemble)
- Clickez sur Create pull request, les notifications des commentaires de connexions vous serons envoyées sur votre boite mail @siriusschool.be

## Autre ressources à bûcher pendant les 7 semaines de cours:

### 1. OpenClassRoom

Suivez les parcours gratuits tels que ce parcours sur git, il est très recommandé d'y porter une attention toute particulière, Git est le logiciel de versionning actuellement le plus utilisé en entreprise:
https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-github

### 2. Grafikart

Comme à son habitude le très bon youtubeur Grafikart a produit une série de vidéo sur le sujet, étant donné que l'installation de git a déjà été réalisée sur votre machine vous pouvez passer ces étapes dans les tutoriaux; n'allez pas plus loin que les vidéos "travailler avec git" nous verrons le reste dans le module avancé de la formation.

### 3. La documentation Git (Anglais)

Des tutoriaux produits par l'organisation Github elle même (en anglais):

https://try.github.io/