# Projet - Simulateur d'un réseau ferroviaire


### Conception et Programmation Objets Avancées (module M3105)
### IUT d’Aix-Marseille – Dép. Informatique Aix-en-Provence, Semestre 3 – Année 2017-2018

* Sophie Nabitz - [sophie.nabitz@univ-avignon.fr](sophie.nabitz@univ-avignon.fr) - https://github.com/bastinz
* Sébastien Nedjar - [sebastien.nedjar@univ-amu.fr](sebastien.nedjar@univ-amu.fr) - https://github.com/nedseb
* Petru Valicov - [petru.valicov@univ-amu.fr](petru.valicov@univ-amu.fr) - https://github.com/pvalicov

**Date de rendu : 20 novembre 2017 à 23h59**  
**Date de soutenance : 23 novembre 2017**

*Le non-respect d’une des consignes ci-dessous impliquera une pénalité de 3 points minimum sur la note du projet. Les modalités pour la soutenance seront précisées ultérieurement.*

### Généralités
-   Vous travaillerez par équipe de 5 personnes et de manière collaborative en utilisant Git et en partageant le travail entre les membres de l'équipe sur GitHub.
-   Chaque membre de l'équipe fera des comits du code qu'il a écrit. L'équipe enseignante va en tenir compte lors de l'évaluation.
-  Le dépôt du projet de votre équipe devra être __privé__ (accessible uniquement par les membres de l'équipe). Une fois créé, vous rendrez ce dépôt accessible en lecture uniquement à l'équipe enseignante (les liens vers les comptes GitHub données en haut de la page).
-  Les modalités de déroulement des soutenances seront précisées ultérieurement.

### Remarques

La note du projet prendra en compte :

-   Le respect des consignes du sujet et des [contraintes du livrable](ContraintesLivrable.md).
-   La modélisation objet de votre application. Également, nous serons
    particulièrement attentifs à l’utilisation appropriée des patrons de conception que vous aurez mis en œuvre
-   La propreté et la lisibilité du code ainsi que tout ce qui
    facilitera sa compréhension par les correcteurs (noms des variables,
    commentaires, modularité, etc ).
-   La facilité d'utilisation du code (le fichier INSTALL/README est-il
    lisible et suffit-il pour utiliser le code ?). La compilation de
    votre code devrait marcher sur tout type de machine - pensez à
    tester avant le rendu final.
-   La correction et la cohérence du code.
-   La présentation de votre application durant la soutenance.

### Instructions

-   Il est **strictement interdit de copier du code** des projets de
    vos collègues. Attention : l’obfuscation du code n’est pas une
    solution, c’est très facile à détecter !
-   Vous pouvez aussi implémenter les bonus et/ou améliorations que vous
    aurez imaginés. Il est cependant conseillé de venir en parler avec
    votre enseignant de projet afin d’en discuter. Dans tous les cas, il
    faut __d’abord implémenter__ les fonctionnalités demandées dans
    le sujet.

Au cours de votre travail de conception et de réalisation, pensez à respecter les principes vus dans vos cours de conception objet durant votre formation.

Les modalités de réalisation de certaines fonctionnalités ne sont pas forcément spécifiées afin de vous donner une certaine liberté dans la conception. En revanche, vous devez respecter les contraintes imposées dans le sujet et justifier tout choix qui les contredit.

## Descriptif


### Fonctionnement général de l'application

La simulation du passage du temps dans votre système se fera par des itérations actionnées par l'utilisateur de l'application. 
Chaque itération est composée des étapes suivantes qui devront être réalisée séquentiellement :


Un utilisateur pourra simuler le fonctionnement du logiciel en déroulant étape après étape le scénario décrit ci-dessus.

Pour rendre le code plus compréhensible et simplifier la maintenance du projet, les parties «*traitement*» et la partie «*affichage*» seront séparées.

-   La couche *traitement* (package «`reseauferre.traitement`») :
    toutes les données et les traitements spécifiques (ex: ajouter des
    tronçons ferroviaires, ajouter des gares, ajouter des trains etc.) sont regroupés
    dans ce package. Les classes de cette couche ne concernent pas la
    partie graphique. Elles se contentent principalement d’effectuer des
    traitements métiers et de renvoyer des résultats.

-   La couche *graphique* (package «`reseauferre.affichage`»): cette
    couche gère l'affichage (interface utilisateur) et les actions de
    l’utilisateur (clics ou saisies au clavier).

## Mise en œuvre
La mise en œuvre du projet passera par la réalisation des classes et méthodes décrites ci-dessous.

### Gares


### Train

 

### Tronçons

### Contrôleur


### Visualisation du système – mode simplifié

Vous implémenterez un ensemble de vues permettant de représenter et modifier l'état interne du système. Votre programme devra en particulier intégrer les vues suivantes :

1.  Une vue qui affiche l'ensemble du réseau à l'état actuel (les trains 

2.  Une vue qui affiche le paneau des temps d'arrivée estimés dans les gares

3.  Un paneau affichant les perturbations dans le réseau : retards, pannes dans les trains ou dans les gares

Afin de ne pas retarder le travail, dans un premier temps, vos différentes vues seront représentées par des messages appropriés affichés dans le terminal.

### Visualisation du système – IHM

*(CETTE PARTIE EST À RÉALISER EN DERNIER)*

Réalisez une interface graphique incluant les éléments suivants :

-   Les différentes vues du système présentées précédemment sous forme de fenêtres indépendantes.

-   La vue 1 sera une vue interactive, c’est sur cette vue que les boutons seront “cliquables”

-   Un menu d'application incluant : paramètres, documentation, à propos de, quitter l'application, etc.

-   La gestion des erreurs d'affichage.