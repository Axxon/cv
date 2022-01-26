# Software engineer XP

## Sapiendo · LeadDev (Freelance févr. 2021 - aujourd’hui · 11 mois févr. 2021)

### Objectifs

- Assurer la qualité et livraison sur l’ensemble des projets Sapiendo.

### Réalisations

- Virtualisation des différents projets sur docker, mise en place de la stack de dev, configuration des builds et 
déploiements via gitlab-ci.
- Refactoring global pour que les données non techniques puissent être assurées par des experts métiers non développeurs 
(portage des variables contextuelles à l’année en cours, sur des fichiers de configuration). 
- Création et maintenance d’un microservice (php8/sf5) multi-containers inter-communicant encapsulant un binaire chargé
de transformer des pdf en xml, les entrées/sorties par ApiPlatform.
- Tache de lead, mise en place de normalisation gitflow inter-équipes, review, fix, support.
- Configuration du déploiement des modules du projet principal sur différents environnements prod, preprod (16 déclinaisons).
- Features front et back (Laravel, vue.js).
- Création d’un outils pour gérer l’ensemble des variables d’environnement pour toutes les déclinaisons.
- Création d’un outils de vérification de l’état de services des environnements, test api via postman newman gitlab-ci.
- Envoi de l’ensemble des logs sur AWSCloudwatch.

## Groupe Blachère · Ingénieur d'études et de développement (CDD déc. 2020 - janv. 2021 · 2 mois)

### Objectif

- Aider un binôme de développeurs séniors PHP à la réalisation d’une refonte des outils utilisés par les équipes 
achat/vente de l’entreprise.

### Réalisation

J’ai accompagné le binôme au départ pour leur transmettre les informations prisent auprès des utilisateurs dont ils 
avaient besoin pour éclaircir la trajectoire à prendre dans leurs développements, j’ai sensibilité le fait qu’il était
nécessaire d’engager un product owner afin d'expliciter les tâches à réaliser et rationaliser la complexité de la tâche
par des user stories. Par l’extraction d’informations/besoins auprès de l’utilisateur final et le chef de projet, j’ai 
codé un outil portant sur le placement de produits de commandes sur un espace de stockage. 
Ceci pour des chargements, du stock aux transporteurs. 

Comme ingrédients phares: un ensemble de commandes traitées comme paramètre volumétrique 
(en fonction des dimensions des produits contenus), puis un espace de stockage lui aussi avec ses propriétés volumétriques. 
Résultant à une suggestion de placements de produits sur des zones spécifiques sur une grille hebdomadaire. 
J’ai conçu un algorithme en full oriented object (tell don’t ask & code as documentation ...) 
dans un contexte domain driven design (Stack-Docker/PHP7/Sf5 + tests unitaires/phpstan => code coverage à 90%).
Modifiable par l’utilisateur par des formulaires symfony et visible par une représentation graphique deux dimensions.

## Ax§n · réalisation d'un projet personnel & RD (2019 - 2020 · 1 an 1 mois)

### Objectif

- Reprendre et étendre l’ensemble de mes connaissances prise au cours de mes dernières expériences, se remettre à jours 
sur la dernière version symfony (5), prendre un projet DDD comme modèle (CodelyTV/php-ddd-example).
- Implémenter une architecture hexagonale avec des concepts CRS/AMQP, respecter les principes décrits dans le dernier 
ouvrage de Mathias Noback (Object Design Style guide) ceci afin de créer un serveur « datawarehouse » qui appel des 
données sur différents fournisseurs et centralisant un ensemble de métadonnées concernant une sélection de titres 
musicaux/labels/artistes.

### Réalisation

- Création du service testé unitairement(mockery) et respectant les contraintes citées précédemment. 
- Isolation/virtualisation du projet avec Docker/Makefile.


## SensioLabs · Ingénieur d'études et de développement (avr. 2018 - sept. 2018 · 6 mois, en full remote) 

### Réalisation

- Lors de ma période d’activité chez Sensio, j’ai construit un site « demo » permettant à la relecture de mon code 
par l’ensemble de l’équipe, d’être en adéquation avec les standards de production du groupe. Un site utilisant 
l’ensemble des fondamentaux de symfony (entities, validation/persistence, routing, controllers, dependency injection, 
- securité, formulaires, twig ...).
- J’ai réalisé un site événementiel pour SensioLabs à l’occasion de ses 10 ans. SF3, utilisation de Sass, bootstrap 4,
Docker, Makefile.
- J’ai de contribué à la réalisation d’un projet « from scratch » disposant d’une API (API-Platform) et interface front 
en React permettant d’accéder à différents systèmes d’information internes à l’entreprise. Accompagné d’un lead et d’un 
développeur front, j’ai participé à la rédaction du code back-end avec le framework symfony4 permettant de mettre à la 
disposition de l’entreprise ses ressources informationnelles. pour se faire:

    - Définition des modèles de données (Entités, VO, mapping par annotation, migrations), validations des hydratations 
      des objets. Création de commandes (console) de déclenchement des extractions de données.
    - Appels HTTP (Guzzle) vers les ressources (microsoft-graph, yammer, bing). 
    - extractions/synchronisations/transformation du contenu (asynchrone), mise à disposition avec APIPlatform. 
      La gestion asynchrone des traitements à été l’implémenté par l’AMQP/C(-Q)RS avec l’usage de RabbitMq + Swarrot 
      (pour le paramétrage des consumers).
    - Utilisation de redis pour stockage temporaire.
    - Authentification par JsonWebToken
    - Vérification intégrale des fonctionnalités de l’api par des tests fonctionnels avec Behat, tests unitaires 
      (PhpUnit) et fixtures (Alice data fixtures) et mise en pre-prod sur SensioCloud.
    - Utilisation de Docker/Makefile et travis-ci pour la stack de developpement.
    - Review des productions avec le lead, documentations.


## Norsys · Ingénieur Études et Développement (2016 - 2018)

### Objectifs:

- Intégrer une large équipe, apprendre les processus de développement en groupe (git, ci, reviews). J’ai eu la chance 
dans cette entreprise de rencontrer des passionnés m’en ayant encore appris beaucoup.
- Participer à des projets à spécificités et contraintes différentes (architecture, budgets, configuration d’équipe ...). 

### Réalisations:

- Pour Décathlon, développement d'un système informationnel interne :
  - Récupération de data par LDAP (Annuaire).
  - Décryptage de code axé « east oriented programming », (pure Object Oriented Language), réalisation de flow-charts.
  - Création de nouvelles fonctionnalités avec l’usage du test driven development avec la librairie de test Atoum et de 
    son créateur.
  - J’ai opéré de nombreuses interactions avec le client afin de mieux ciblé sa demande.
  - Création des vues en twig.
  
- Pour Technal :
  - Implémentation php/sf des besoins métiers.
  - Documentations / Reviews 
  - Première expériences avec SCRUM (Poker planning, sprints, tickets …)

- Pour un redistributeur :
  - Isolation/Virtualisation du projet avec Docker.
  - Création de requêtes avec Pomm (orm pour postgresql). 
  - Correction de bugs.

- Pour Franprix, un site de formation interne :
  - J’ai été force de proposition sur l’ensemble des décisions techniques, l’architecture logiciel, le choix dépendences.
  - Définition des modèles, CRUDs, Tests unitaires, création de formulaires dynamiques, Twig, affichage des plannings, 
    interactions utilisateur/interface. Authentification, autorisations.
  - J’ai assumé le rôle de communiquant avec le product owner, fait des retours sur l’avancé des sprints, 
    interrogé/éclairci sur des détails d’implémentation de fonctionnalités.
         
- Pour Fiducial : 
  - Réalisation de formulaires (avec les controlleur + vues) en lecture/écriture, dynamiques, avec usages fréquents des
    prototypes ainsi que la gestions des erreurs.
  - Extension de la modélisation du domaine.
  - Création d’un package afin de faciliter le processus d’authentification sur une api interne.
  - Utilisation de Vagrant (sur un environnement windows afin de disposer d’un environnement de travail Linux, 
    le sous-système windows pour Linux n’existait pas).
  - Développement front Es6/Webpack.


## ActivCompany · Developpeur web apprentis (2015)

### Objectifs:

- assister le developpeur PHP/sf2 sur tout les projets
- passer à la pratique dans un contexte d'entreprise

### Réalisations:

- réalisation de sites vitrines sf2 simples
- réalisation d'un ERP avec Sf2
- réalisation d'un réseau social professionnel, refacto/correction code de ESN, developpement de features.