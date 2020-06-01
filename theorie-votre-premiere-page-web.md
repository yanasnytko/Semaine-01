# Votre première page web: une recette en HTML / CSS

## Introduction

Vous trouverez dans ce fichier toutes les ressources nécessaires à la réalisation de votre exercice de la semaine.

## Table des matières

1. Qu'est ce que le HTML
2. Qu'est ce que le CSS
3. MDN et autres ressources

## Qu'est ce que le HTML?

HTML est l'acronyme de HyperText Markup Language.
Le HTML n'est pas un langage à proprement parlé comme on peut le dire du Javascript ou du PHP. 
Il s'agit d'un "langage de balisage", il est directement interpêté par le navigateur, c'est à dire qu'il n'a besoin d'aucune traduction pour que le navigateur puisse rendre le contenu visible sur votre ordinateur / tablette / GSM. 
Par langage de balisage on entend qu'il utilise des balises telles que celles que nous avons vues la semaine dernière lors de votre premier exercice (les balises `<p> <h1> <h2>...`  )
elles indiquent l'endroit de la page où votre contenu doit être inséré, comme un coup de marqueur sur une carte.

C'est le squelette de votre page web, comme vos os soutiennent votre corps et ses différents tissus, le HTML soutient le contenu de votre page, permet de le styliser, de l'animer, de le rendre dynamique. Mais nous verrons cela plus tard.

Qu'entendons-nous par contenu?

Titres, textes, images, vidéos, liens vers d'autres pages...

## Qu'est ce que le CSS? 

Le CSS ou Cascading Style sheets (feuilles de style en cascade), permet la mise en forme de votre squelette, c'est la partie émergée de l'iceberg, celle que vous pouvez voir quand vous consulter vos pages web. 

Couleurs, polices, formes, tailles, mise en page, animations, tout ce qui rend "joli" (ou non) le squelette de votre page web ainsi que son contenu.
Rataché à votre HTML il vous permettra de mettre en oeuvre ce que vous verrez dans votre cours de Web Design. 
La synthaxe se compose de plusieurs éléments:
1. Le sélecteur: le nom de la balise à laquelle vous désirez attribuer un style (par exemple: h1), le nom de classe que vous avez personnalisé précédé d'un point (par exemple: .main-title), ou l'ID de l'élément précédé d'un # (par exemple: #main-container). 
2. La propriété CSS: il s'agit ici de la propriété qui va permettre la mise en page de votre contenu, par exemple si vous souhaitez modifier la taille de votre police la propriété CSS qui s'y ratache est "font-size". 
3. La valeur: et enfin la valeur que vous souhaitez apporter à la propriété, par exemple pour un titre vous désirerez peut être régler la taille de votre police sur 24px 

Voici un exemple de synthaxe CSS que vous pourriez retrouver dans votre code:

.main-title {
    font-size: 24px;
    color: white
}

Les bracelets ou "curly bracket" { } signifie l'ouverture du code, insérez y vos propriétés CSS, pour que le navigateur puisse passer à la propriété suivante n'oubliez jamais de faire suivre vos valeur d'un ";" point virgule et de passer à la ligne. 
Mais avant toute chose: pour permettre à votre CSS d'être appliqué à votre HTML vous devez le lier au fichier HTML; il existe trois façon d'appliquer du CSS à votre HTML vous les découvrirez dans cet article:
https://developer.mozilla.org/fr/docs/Apprendre/CSS/Utiliser_CSS_dans_une_page_web



### Astuces:

1. Pressez la page F12 de cette page web: TODO INSERER LE RESULTAT DE L'EXERCICE AVEC UN SCREENSHOT;
2. Voici l'interface "Outils développeur" de votre  navigateur (dans cet exemple il s'agit de chrome):

![](https://i.imgur.com/H6gm6Gt.png)

- En point 1: CSS écrit par le programmeur 

- En point 2: Espace permettant d'écrire par dessus le CSS rédigé par le programmeur; utile pour tester vos propriétés et vos valeurs avant de les écrire dans votre feuille de style

- En point 3: CSS pré-écrit par le navigateur -> votre navigateur possède un CSS pré-défini pour toutes les propriétés qui ne sont pas écrites par le programmeur. 

Modifiez quelques propriétés au sein de votre navigateur pour vous entrainez.

## MDN et autres ressources

La documentation firefox faites par des développeurs pour les développeurs: 
https://developer.mozilla.org/fr/

Il s'agit de votre nouveau livre de chevet, vous trouverez toutes les informations nécessaires à la réalisation de votre première page web dont le listing des balises HTML et propriétés CSS ainsi qu'un espace pour tester votre code;

Voici les deux ressources qui vous serons indispensables à la réalisation de votre exercice, épeluchez les, testez, découvrez, faites vous la main:

- Référencement des éléments(ou balises) HTML : https://developer.mozilla.org/fr/docs/Web/HTML/Element
- La documentation MDN pour le CSS étant un peu plus avancée, nous allons commencer par la W3school, elle n'est pas standard mais vous permettra de débuter et de réaliser votre premier exercice sereinement, nous reviendrons la semaine prochaine sur cette documentation:
https://www.w3schools.com/css/default.asp 