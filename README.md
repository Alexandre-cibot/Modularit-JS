# Modularité en Javascript

##Introduction :

### Définition d’une programmation modulaire:

Un module est un simple fichier JS, généralement une function ou un objet qui est exporté pour le rendre utilisable par d’autres ficiher JS. On dit qu’on exporte un module et qu’on importe un module.
Par convention, on limite un module par fichier.

La modularité __n’existe pas nativement__ dans le JavaScript.

La notion import et d’export a été intégré dans ES6. Pour cela, il faut s'aider de l'ibrairies externes.

###Quel est l'intérêt de la modularité ?

Pour comprendre les avantage de la modularité moderne, il faut d’abord revenir sur les méthodes utilisés auparavant. 

Avant l’arrivé des modules-bundler (Gulp, Webpack, Browserify ..), pour séparer son code JS en plusieur fichiers, il fallait les importer à la suite des balises \<script\> dans le fichier HTML.
Cela était fastidieux, de plus avec cette méthode, on était obligé de respecter un ordre défini car on devait respecter les dépendances entre les scripts. Aujourd’hui avec les utilisations des modules bundler on peut gérer les dépendances plus facilement dans un seul fichier JavaScript. 

Grâce aux modules bundler, les développeurs peuvent tester leur codes et déceler les erreurs de codes plus facilement.

Avec des modules, il est alors plus facile de partager son code. Vu qu’une fonction/module est réparti dans un fichier, les développeurs pourront trouver le module qui les intéressent sans devoir à en modifier une grande partie. 

La modularité facilite le travail open-source via des plateformes comme Github. Le fait de séparer son code en module, offre une structure beaucoup plus maintenable et agréable au quotidien pour le développeur.

Javascript ne supportant pas nativement les modules, la communauté s’est chargé de créer des solutions pour pallier à ce manque. Les deux standards les plus populaires sont :

* CommonJS : Implémenté dans Node.js et Browserify, il se caractérise par :
  * Un design adapté au chargement synchrone

Exemple de syntaxe CommonJS: 

