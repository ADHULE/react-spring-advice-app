
 ## Combinaison Spring Boot & React avec Docker
 #Pourquoi combiner Spring Boot, React et Docker ?

Dans une application moderne, on sépare généralement :

🧠 Le backend : logique métier, API, base de données

🎨 Le frontend : interface utilisateur

🐳 Docker : environnement d’exécution et de déploiement

👉 Docker joue le rôle de “colle” qui assemble ces technologies hétérogènes dans un environnement unique, cohérent et reproductible.

2️⃣ Rôle de chaque technologie
🔙 Spring Boot (Backend)

## Spring Boot est utilisé pour :

Exposer des API REST

Gérer la logique métier

Communiquer avec la base de données

Fournir des services aux clients (frontend)

📌 Le backend ne s’occupe pas de l’affichage, uniquement des données et des règles métier.

🎨 React (Frontend)

## React permet de :

Créer une interface utilisateur dynamique

Consommer les API REST du backend

Gérer l’état de l’application côté client

📌 Le frontend ne connaît pas la base de données, il communique uniquement avec le backend via HTTP.

🐳 Docker (Orchestrateur)

## Docker permet de :

Isoler chaque technologie dans un container indépendant

Assurer que l’application fonctionne de la même manière sur toutes les machines

Faciliter le déploiement, les tests et la maintenance

3️⃣ Comment Docker combine Spring Boot et React ?
🔑 Principe fondamental

Chaque technologie tourne dans son propre container, mais tous les containers partagent un même réseau Docker.

🧱 Architecture Docker

Container Frontend React

Container Backend Spring Boot

Container Base de données (MariaDB)

Containers outils (phpMyAdmin, Adminer, MailHog, etc.)

Docker crée automatiquement :

🌐 un réseau interne

🔁 une communication directe entre services
