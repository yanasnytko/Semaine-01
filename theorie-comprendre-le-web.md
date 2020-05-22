
# Comprendre le World Wide Web

  

## Introduction 

  Avant de vous lancer dans l'apprentissage des langage de programmation, il est important de comprendre comment le web fonctionne. Nous allons aborder brièvement l'histoire du Web, son fonctionnement et ce qui vous permet de consulter une page Web grâce à vos téléphones, tablettes ou ordinateur.

  

## Table des matières

  1. L'histoire du Web en Bref
  2. Qu'est ce qu'un Client / Browser
  3. Qu'est ce qu'un Serveur  ? 
  4. Comment transférer vos fichiers locaux vers un hébergeur 
  5. Quelle est la différence entre un site statique et un site dynamique ? 
  6. Tips et Astuces:  les outils de développement

  

## Fichiers

  

Listing des ressources présentes sur le repository en lien avec la théorie vue dans ce cours

  

## 1. L'histoire du Web en Bref

  

### Le saviez vous?

En anglais Web (aussi appelé World Wide Web)  signifie "la Toile", on peut l'imaginer telle une toile d'araignée tissée reliant tous ses utilisateurs par delà les frontières physiques, de langues et de distances. 

Ce réseau inventé entre 1989 et 1990 a permis de donner accès à la connaissance et au partage à travers le monde et fait aujourd'hui partie intégrante de notre quotidien. 

Imaginez vous une journée sans accès à votre réseau social favoris? Que feriez vous sans Wikipédia ?

Le Web a permis de créer des liens entre les populations, et de rendre l'information disponible à tous. Actualité, livres, vidéos, musique, jeux... 

Mais savez vous à qui vous devez cette merveilleuse invention? 

Tim Berners-Lee ainsi que Robert Cailliau ont inventé ce merveilleux outils. On peut donc affirmer que la moitié de la paternité du Web revient à la Belgique, en effet Robert Cailliau est un ingénieur Liégeois, plutôt cool n'est ce pas?


 ## 2.  Qu'est ce qu'un client

Un client ou, client HTTP est l'outils permettant l'affichage des fichiers contenus sur un serveur. Ces fichiers comprennent l’entièreté du contenu d'un site web ou d'une application. En d'autres termes il s'agit d'un Browser, en français: votre navigateur favoris -> Chrome, Firefox, Safari, Opera.... Internet explorer pour les plus aventureux!

Un terme compliqué pour un outils simple que vous utilisez déjà tout les jours!

### 2.1 Développement Front-End

Lorsque l'on parle d'affichage client, on parle donc de ce que votre navigateur interprète du serveur. 

Pour que votre Browser puisse interprêter ces données, il faut qu'elles aient été rendues disponnibles et compréhensibles à la lecture de votre navigateur via le développement Client, c'est à dire le développement **Front-End**. 

Codé en HTML, CSS et Javascript, qui sont les seuls langages (même si HTML et CSS ne sont pas des langages à prorprement parlé contrairement à Javascript) compris et interprêté par le Browser.
Le browser n'est donc que le traducteur entre le code fournit par le développeur (d'abord côté serveur, puis côté client) et l'utilisateur. Un navigateur retranscrit le langage "machine" dans un langage compréhensible par l'humain et permet l'affichage visuel du contenu.

Le client permet d'envoyer des demande (requêtes) d'actions à performer sur les données contenues par le serveur. Une fois ces demandes reçues par le serveur, c'est le serveur qui décide si oui ou non il va performer cette action et de quelle façon. 

Par exemple: vous décidez de changer votre nom et prénom sur Facebook. Facebook vous demande de remplir un formulaire et de l'envoyer. Il s'agit d'une action appellée "Submit" ou "Post". Le serveur reçois cette demande et en fonction des restrictions programmées par les développeur et de sa configuration, l'action sera performée ou non.

**Un client peut également fonctionner de manière indépendante, sans l'aide d'un serveur.**

> Allez dans le dossier exercice de la semaine 1, et double cliquez sur votre fichier exemple-client.html, observez ce qu'il se passe

Ce type de développement ne fonctionne uniquement que dans le cadre des sites statiques (nous aborderons plus loin la différence entre un site statique et un site dynamique), dans le cas de l'exercice actuel, les fichiers sont hébergés par votre ordinateur et affiché dans votre navigateur. Ils ne contiennent que du contenu interprêtables par le navigateur et ne permettent pas de perfomer d'action sur les données affichées. 

Pour rendre disponnibles ces fichiers ils sont simplement hébergé par une société d'hébergement qui se charge de les rendre disponnibles sur internet via une URL unique (voir le chapitre URL).

  ## 3. Qu'est ce qu'un serveur ? 

Nous venons de voir l'utilité d'un client, nous avons abordé la notion de serveur, mais qu'est ce qu'un serveur? 

Un serveur HTTP (ou WebService) est un logiciel utilisé pour stocker, transférer, manipuler, des données (fichiers) à travers le protocole HTTP. 
Il est le contenant et l'opérateur de toute les informations d'un site web, ou d'une application (web / mobile / desktop). 

![source: Schéma provenant d'OpenClassRoom ](http://user.oc-static.com/files/5001_6000/5675.jpg)
* Source: Schéma provenant d'OpenClassRoom

Nous avons évoqué dans le chapitre sur le Client que les requêtes / actions envoyées par l'utilisateur sont **gérées par le serveur.**

### 3.1 Développement Back-End

Le programmeur Back-End gère la programmation du serveur, il autorise ou non les requêtes et décide de la manière dont celles-ci seront traîtées, la façon dont les données seront manipulées puis retournées au client, il est l'opérateur, c'est lui le cerveau derrière chaque application ou site dynamique. On appelle ce type de programmation "la logique métier".

< Par exemple: Lorsqu'une requête n'abouti à rien de "connu" par le serveur, une erreur 404 est retournée, c'est la fameuse "404 not found" bien connue de tout le monde lorsque vous essayez de contacter une page n'existant pas ou plus.

Retenez simplement que le code fournit par le développeur Back-End contient la logique métier qui permet de performer l'action demandée par une requête (appel) effectuée par le client qui en retour interprétera les données reçues, performera des actions sur les données contenues par ces fichiers et que le client enverra ses requêtes et en traduira les réponses (que ce soit l'affichage d'une page ou la modification d'un nom sur facebook) pour l’œil humain via votre navigateur. 

### 3.1 Notion de serveur local et de web hosting

Comme nous venons de le voir le serveur est un contenant des fichiers programmés et écrit par le développeur. 

Nous distinguons 2 types de serveur:

Le serveur local (ou localhost, disponible par défaut dans votre navigateur à l'URL: http://localholst:8000),
Le web hosting ou serveur distant (disponnible à l'URL personnalisée du propriétaire de l'application ou site web).

###  3.2 URLs et ports
Une URL ou Uniform Resource Locator est l'adresse d'une page, d'un site ou d'une application web. 
Elle permet de localiser la page dans l'immensité de la toile du web. 
Une URL est donc personnalisée et unique. 

#### 3.1.1 Serveur distant
L'anatomie d'une URL lorsqu'elle est disponnible sur un serveur distant (hébergée par un serveur physique: le web hosting) se compose comme suit: 

![](https://www.mission-internet.fr/wp-content/uploads/2018/12/structure-dune-url.jpg)
* Source: www.mission-internet.fr

**Le nom du protocole (ou préfixe):** il s'agit du langage utilisé pour communiquer sur le réseau. HTTP est l'acronyme de HyperText Transfer Protocol, il permet de "transférer" les informations des pages Web (HTML, CSS, Javascript, etc..) vers le client. Il existe d'autres protocoles mais celui ci est le plus usité et celui dont nous ferons nous même usage.

**Le certificat de sécurité:** Il s'agit d'une surcouche ajoutée au protocole assurant la sécurité du site ou de l'application, elle permet par exemple d'effectuer des paiements en ligne, de s'identifier, d'envoyer des informations depuis le client vers le serveur (exemple: lorsque vous envoyez un email, la surcouche appellée SSL permet l'envois sécurisé de vos données).

**Le sous domaine**: Il permet de scinder le site en plusieurs partie et lui dédier des tâches différentes. Il peut se composer comme suit: "www", "ww2" ou "ww3". Il est utilisé pour le référencement SEO, une notion que nous aborderons plus tard dans la formation. Pour l'instant retenez simplement que "www" correspond au sous-domaine principal, celui que vous rencontrerez par défaut et le plus souvent. 

**Le nom de domaine**: Il s'agit du nom personnalisé et choisi par le propriétaire du site web ou de l'application et sert à l'identifier de manière précise. Il permet de contacter le serveur se rapportant au nom de domaine. Il est également possible de contacter le serveur via son adresse IP, ce qui rend la lecture de l'URL plus compliquée. Par exemple: vous pouvez vous rendre sur http://google.com à l'aide de son adresse IP physique (ou DNS): http://74.125.19.147

Pour l'instant nous nous contenterons d'utiliser les noms de domaines simplifiés

**L'extension:** Permet d'aller plus loin dans la personnalisation de l'URL, on peut la désigner soit sous l'acronyme d'un pays (ex: .be ), mais également sous la forme d'une activité (ex: .org pour organisation )

**Les routes:** Une URL peut également pointer vers un nom d'une page en particulier. 

> http://mon-site.be/contact

![](https://i.imgur.com/o8NPj0s.png)

**Les paramètres:** Il s'agit d'une notion plus complexe que nous aborderons plus tard dans le cours. Ils permettent d'effectuer des actions sur le serveur distant, ou de récupérer des informations spécifiques.

#### 3.1.2 Le serveur local

Par serveur local comprenez "hébergeur local" il ne s'agit pas du serveur "code métier" mais uniquement d'un outil permettant d'héberger localement sur votre ordinateur votre site statique ou dynamique.
Lorsque nos fichiers sont hébergé en "local", c'est à dire non pas sur le web mais uniquement sur votre ordinateur, l'intérêt se situe lors de la conception et de la maintenance de votre site ou de votre application, le serveur local permet de tester l'affichage et le bon fonctionnement de votre code. 

Dans ce cadre l'URL peut se représenter comme suit:

![](https://zupimages.net/up/20/21/p3a0.jpg)
* Source: MDN

Vous l'aurez compris le préfixe, le nom de domaine et l'extension sont donc remplacé par le localhost.

Les routes et paramètres sont toujours existant et permettent de vérifier le bon fonctionnement de votre code.

Il peut exister un serveur local dédié au *développement client* (front-end) et un serveur local dédié au *développement serveur* (back-end). Pour permettre à l'ordinateur de lancer le développement de ces deux parties simultanément vous aurez besoin de configurer un port spécifique pour chacune des parties. 

> Et du coup, c'est quoi un port?


### 3.2 Les ports

Pour chaque programmes exécutés simultanément sur internet (plusieurs onglets ouverts, des applications mobiles ou desktop, ou simplement plusieurs navigateurs ouverts en même temps) se voit attribuer une adresse unique, générée par votre ordinateur. Cette adresse n'est autre que le port. La combinaison de l'adresse IP (qui est, rappellons le,  l'adresse de contact du serveur à qui vous faites appel par exemple lorsque vous utilisez youtube ou google), et du port est appelé un Socket. 

> Les web socket sont une notion complexe que nous n'aborderons probablement pas dans le cadre de cette introduction à la programmation mais il est utile de savoir à quoi correspond ce terme car vous risquez d'en entendre régulièrement parler.


Du côté distant il existe également des ports, configurés par le programmeur ayant produit le code du serveur. Il décide du numéro de port et la combinaison IP + Port en fait une adresse de contact unique (le socket). 

Du côté d'un serveur local utilisé dans le cadre du développement le port utilisé par défaut est le 8000 ou 8080. Il existe des ports "enregistrés" allant du port 1024 au port 49151. 

Lorsqu'il s'avèrera de lancer plusieurs serveurs locaux il vous faudra vous même configurer les numéros de ports de vos applications, du côté serveur comme du côté client, contrairement à une application déjà réalisée et configurée par le programmeur. 

> Vous pouvez donc par exemple configurer le port 8080 pour le développement Front-end (développement côté client) et le développement Back-end (développement côté serveur) configuré sur le port 3630.

**La configuration de port personnalisés vous permet de développer plusieurs outils en même temps, gardez le bien à l'esprit, ceci vous sera de grande utilité lors du second module de votre formation**

## 4. Comment transférer vos fichiers locaux vers un hébergeur

Dans le cadre de notre formation et de son premier module nous nous contenterons d'utiliser Github, qui propose l'hébergement de vos fichiers *dans le cadre d'un **site statique uniquement***, la collaboration entre apprenants et formateurs (Comme vous l'avez vu ou le verrez dans l'introduction à Github, Git est un logiciel de versionning et Github l'hébergeur / le réseau social de ce logiciel). 

> *Vous pouvez donc envoyer vos fichiers sur votre repository Github afin de les y héberger*

![](https://i.imgur.com/5g7f0oU.png)

>*Pour ensuite les déployer grâce à l'outils **Github Page***

![](https://i.imgur.com/xyZotbI.png)

>*Il vous sera pour cela nécessaire d'apporter quelques configurations à votre repository, pour y accéder clickez sur l'onglet settings:*

![](https://i.imgur.com/8ggPIWn.png)

>*Un fois dans cet onglet configurez la page en fonction du dossier à utiliser pour être interprêté par le client: dans l'exemple suivant il s'agit d'un projet en React, il m'a donc été nécessaire de passer par un compileur permettant de traduire la librairie React en Javascript (interprêtable par le navigateur), ce compileur stock sa traduction dans le dossier docs, ma GHpage est donc configurée pour utiliser le dossier docs, nous verrons ultérieurement dans un petit exercice comment configurer simplement une GHpage pour un site statique en HTML/CSS/Javascript*

![](https://i.imgur.com/ZpU1vw9.png)

>*Lorsque configurée correctement, votre GHPage vous permettra d'avoir accès en ligne à votre création web!*

![](https://i.imgur.com/oODVjPU.png)

> **La mise en place de serveur locaux ou distant et d'hébergement feront l'objet d'un cours à part entière, il ne s'agit ici que d'une simple introduction**

##   5. Quelle est la différence entre un site statique et un site dynamique ? 

### 5.1 Site statique

Contrairement aux idées reçues un site statique n'est pas un site dépourvu d'animations. 

Lorsque nous parlons de site statique nous parlons de **"pages statiques" visibles telles qu'elles ont été conçues et ne pouvant recevoir de modification extérieur.** 

Pour être modifiées ces informations doivent d'abord repasser dans les mains du développeur pour ensuite être codées, uploadées et déployées. 

Si non, elles resteront toujours identiques à ce qui a été développé à sa création. 

> *Un site statique ne permet **aucune interaction** avec l'utilisateur et donc aucune modification ou ajout de données de sa part.*

Dans le cadre de ces 7 premières semaines de cours vous aurez l'occasion vous aussi de développer vos premiers sites statiques personnels dont votre propre C.V./Portfolio, un outils qui servira de vitrine auprès des futurs recruteurs!

### 5.2 Site dynamique

>*Contrairement au site statique, un site dynamique **peut être modifié par son utilisateur.***

 Reprenons comme exemple facebook, vous pouvez ajouter des publications, likez celles de vos amis, changer de photo de profil, etc. 

Dans le panel des sites ou application dynamiques nous pouvons retrouver: réseaux sociaux, blogs, plateforme de téléchargements ou de streaming telles que Netflix, application de gestion de temps (To-do liste), etc...

Pour ce faire l'utilisateur, comme nous l'avons vu précédement dans les chapitre Client/Serveur, va devoir envoyer une requête au serveur, ces requêtes peuvent uploader un nouveau contenu, récupérer un contenu, le modifier, ou le supprimer. Le serveur traîte la demande et effectue l'opération pour ensuite recevoir une réponse contenant le contenu demandé, modifié, ajouté, ou supprimé.

Nous aurons également l'occasion d'aborder de façon sommaire ces concepts durant certains projets de votre formation! 


## Tips et astuces : les outils de développement

Afin de faciliter le développement de vos applications, les différents navigateurs ont développé leur propre outils de développement, disponnibles en pressant la touche "inspecteur" F12 de votre clavier. 

Je vous renvois à cet article agrémenté de vidéos de KhanAcademy reprennant ce sujet, veillez à le lire et à regarder attentivement les vidéos, faites en faire bon usage!

https://fr.khanacademy.org/computing/computer-programming/html-css/web-development-tools/a/using-the-browser-developer-tools

Une petite astuce supplémentaire: pour constater les modifications sur votre site en conception dans le localhost, vous devez rafraîchir la page : plutôt que d'utiliser le bouton rafraîchir de votre navigateur, préféré la touche F5 de votre clavier! Et n'oubliez pas si vous avez les outils de développeur ouverts, de vider votre cache!

## Conclusion

Nous voici à la fin de cette introduction au vaste monde du Web, comme vous l'aurez compris, ce ne sont que des notions élémentaires que nous viendrons agrémenter tout au long de votre formation. Pas de panique, tout ceci semble difficile à appréhender au début, mais une fois les mains dans le camboui je n'ai aucun doute quant à vos capacité d'apprentissage. N'hésitez pas à revenir sur cette théorie dés qu'il s'avérera nécessaire. Petit à petit vous vous rendrez compte du chemin parcouru depuis cette introduction et de vos nouveaux talents de codeur en herbe.

Bon travail à tous!