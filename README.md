# FLUTTER

## Plan de cours

### Introduction

Présentation générale de Flutter et son utilité dans le développement d'applications mobiles.
Comparaison avec d'autres frameworks de développement mobile.
Installation de Flutter et configuration de l'environnement de développement.

### Dart : rappels

Présentation
Syntaxe de base : - type de données - variable et constantes - structures de controle (conditions / boucles) - fonctions (déclaration, arguments, valeur de retour)
Classes et objets : - encapsulation (propriété, méthodes) - héritage et polymorphisme - constructeur
Gestion des erreurs (try / catch)
Asynchronicité (Future)
Manipulation des données (Map / List / map / filter / reduce)

### Structure et architecture

Architecture de Flutter : widgets, stateful vs stateless widgets.
Structure d'une application Flutter : main.dart, Widgets, MaterialApp.
Premier projet : création d'une application Flutter simple.

### Interface utilisateur

Exploration des widgets de base de Flutter : Text, Image, Container, Row, Column, etc.
Mise en page : gestion des contraintes, utilisation des widgets Flex et Expanded.
Création d'une interface utilisateur simple pour une application mobile.

### Gestion d'état

Compréhension de la gestion de l'état dans une application Flutter.
Utilisation de setState pour mettre à jour l'interface utilisateur.
Gestion de l'état global avec Provider ou Riverpod.

### Routing

Navigation entre les écrans dans une application Flutter.
Utilisation de Routes nommées.
Gestion de la navigation avec MaterialApp et Navigator.

### API natives et communication

Utilisation des APIs natives avec les plugins Flutter.
Appels réseau avec le package http.
Intégration de la gestion des données avec Firebase.

### Déploiement

Préparation de l'application pour le déploiement.
Compilation de l'application pour les plateformes iOS et Android.
Publication de l'application sur Google Play Store et Apple App Store.

## Introduction à Flutter

### Définition

Flutter est un kit de développement logiciel (SDK) d'interface utilisateur open-source créé par Google et basé sur le langage Dart.
Il permet de développer des applications pour Android, iOS, Linux, Mac, Windows, Google Fuchsia et le web en utilisant une seule base de code.

### Version

La version Flutter 1.0 est publiée fin2018 et est la première version stable du framwork.
La version Flutter 3.0 est publiée en 2022 (actuelle : 3.19).

### Avantages

**Multiplateforme :**
Un code unique pour plusieurs plateformes ce qui réduit le temps et les coûts de developpement.

**Performances :**
Le code est compilé en langage machine supprimant ainsi le "pont" JavaScript et accélérant son exécution.

**Outils :**
Mise à disposition aux développeurs d'outils tel que le "hot reload" qui permettent d'afficher les modifications apportées sans redémarage ou perte des états en cours.

**Widgets :**
Bilbliothèque de widgets riche et personnalisable qui offre une grande variété d'éléments d'interface utilisateur adaptés à chaque plateforme.

**Indépendance :**
Les composants sont indépendants de la plateforme utilisés permettant d'assurer la cohérence du rendu de l'application sur toutes les plateformes.

### Inconvéniants

**Apprentissage :**
La courbe d'apprentiisage de Flutter est plus raide que pour d'autres frameworks, le langage Dart étant moins utilisé que la langage JavaScript (avec React Native par exemple).

**Fonctionnalité natives :**
Accès limité aux fonctionnalités natives à la plateforme car Flutter utilise ses propres widgets.

### Mise en place de l'environnement de developpement

**Flutter :**

- [Téléchargement](https://flutter.dev/)
- extraction du package dans un répertoire de son choix (éviter les répertoires avec caractères spéciaux ou espace)
- ajouter flutter aux variables d'environnement
- vérifier l'installation depuis un terminal exécutant la commande <code>flutter doctor</code>

**Editeur de code :**
Plusieurs éditeurs sont utilisables avec Flutter :

- Visual Studio Code
- Android Studio
- IntelliJ IDEA
- etc ...

Nous utiliserons ici Visual Studio Code:

- [Téléchargement](https://code.visualstudio.com/)
- installation
- installation des extensions :
  - Flutter
  - Dart

**Création d'un nouveau projet :**

- <code>ctrl + shift + P</code> pour ouvrir la palette de commande
- indiquer <code>flutter</code> dans la recherche et séléctionner <code>Flutter : New Project</code>
- séléctionner le dossier de destination
- nommer le projet

La création du projet est rapide, vous pouvez commencer à travailler dès maintenant.
