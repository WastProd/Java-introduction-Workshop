
# Introduction à Java et ses avantages par rapport au CPP

Ce workshop est conçu pour vous initier au développement java et notament une introduction à la reflection d'objet (ce qui n'est pas possible en CPP).
Il est conseillé d'utiliser un IDE comme IntelliJ ou Eclipse si vous voulez approfondir vos connaissances, *VSCode n'est pas fait pour les langages orienté objet.

Voici la [documentation officielle d'oracle sur la version LTS 21](https://docs.oracle.com/en/java/javase/21/docs/api/index.html).

## Prérequis
- JDK (java development kit) [disponible ici](https://www.oracle.com/fr/java/technologies/downloads/#java21) (il est conseillé d'utiliser la dernière LTS Java 21).
- IDE Java compatible : [Eclipse](https://eclipseide.org/) ou [IntelliJ Community Edition](https://www.jetbrains.com/idea/download/other.html).

## Installation & création d'un projet test

Créez un nouveau projet avec maven ou gradle (ici j'utiliserai gradle, sous IntelliJ).

![création d'un projet java test avec intellij](https://cdn.discordapp.com/attachments/1239922406626430996/1239922498141818901/Screenshot_from_2024-05-14_14-47-09.png?ex=6644af50&is=66435dd0&hm=2d7a473426aa4995a7a4c5ae3e683be600acebb704a4c591b18848d6574b9dd3&)

Une fois votre projet crée, votre IDE va automatiquement créer les fichiers de base et configurer votre compiler.

![exemple de projet test une fois crée](https://cdn.discordapp.com/attachments/1239922406626430996/1239924209430302730/Screenshot_from_2024-05-14_14-55-46.png?ex=6644b0e8&is=66435f68&hm=6e067bb14c09b4af2eb48e0d35096cdb9f08a4ac7b0bc15050dff0f2dd1b3661&)

### Exercice 1 : Lancer votre premier programme en java
- **Objectif** : Votre IDE à crée une classe main avec un "Hello world!" pour vous, entourez le d'une boucle pour qu'il apparaisse 10 fois dans votre console. 
- **Comment tester ?** : Une fois "votre Hello world!" écrit, tester votre programme avec le bouton run en haut à droite (sur IntelliJ). 

![exemple d'un run basique d'un sys.out.println()](https://cdn.discordapp.com/attachments/1239922406626430996/1239926117398220841/image.png?ex=6644b2af&is=6643612f&hm=f8950349d0aa5d3bf683fbafacc2350e26f2620530620168251d8098ac4f43a1&)

### Exercice 2 : Premier objet
- **Objectif** : Créez une classe "Car" avec un attribut "wheels" que vous définissez à 4 par défaut. Créez un getter de "wheels" dans la classe "Car".
- **Comment tester ?** : Créez un objet "Car" dans votre main et afficher le résultat du getter de l'argument "wheels".

### Exercice 3 : Interface et héritage
- **Objectif** : Créer une interface "Vehicle" avec une methode "getWheels" qui retourne un int. Modifiez la classe "Car" pour qu'elle hérite de l'interface "Vehicle" (faites les modification en conséquences)

### Exercice 4 : Interêt du Polymorphisme
- **Objectif** : Créez une deuxieme class qui hérite de l'interface "Vehicle" nommée "Truck" (avec 6 roues par exemple) puis créez une liste de type ArrayList dans votre main qui contient des objets d'interface "Vehicle".
- **Comment tester ?** : Créez des objets truck et car dans votre main, insérez les dans la liste et affichez leurs attributs en utilisant l'interface.

### Exercice 5 : Déconstruction
- **Objectif** : Créez un niveau d'héritage suplémentaire (ex: interface Car & Truck qui hérite de Vehicule) puis créez une classe pour les différents modèles de voitures/camions. Dans votre boucle, trouvez le moyen de différenciez les interfaces "Car" des "Truck".

### Exercice 6 : Finitions
- **Objectif** : Créez des méthodes de mouvements (ex: goFoward, goBackward, turnRight..) et une classe ENUM nommée "Direction" dans une classe Abstraite pour vos véhicules. L'objectif est d'implementer un système de véhicule complètement générique. (Cet exercice ne suit pas forcément l'archtechture des précédents)
