# 2. Introduction à Docker
- Installation de Docker sur votre environnement de développement.
- Création d’un Compte Docker Hub

  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/a4433315-7562-46be-b5d5-54266b83b816)

# 3. Utilisation de Docker :
- Création d'un conteneur Docker à partir d'une image existante : nginx port 8090
  First , we pull the nginx image and we run the containers with it :

  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/d6e7cbf8-5ef1-45c4-bb28-3f23bb3cfb75)

- Test et validation du fonctionnement du conteneur nginx
- Exploration du contenu du Conteneur

  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/3780b4d6-c452-449c-8a21-46d2c392aafe)

- Création d’un deuxième Conteneur nginx sur le port 8091
  
  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/9a312d2a-54e7-42e1-bcfe-1967010d4e81)

  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/0a4de02d-9993-4e53-87cc-12fbf15d31b0)

- Gestion des conteneurs Docker : liste,démarrage, arrêt, suppression

  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/028fe71e-bbc8-43fa-b0a7-7078a26b99a8)

 # 4. Exécution d'une application SpringBoot dans un conteneur Docker :
  Créer une Application SpringBoot avec un seule Contrôleur qui affiche le message «Bonjour »
- Ecrire le Dockerfile pour créer une image de cette application :
  
  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/479010e3-d9d6-4512-afea-0cdb029d3b59)

  ![image](https://github.com/firassaada/Devops-Labs/assets/94303698/9dcce40e-dfe9-443d-b54e-cfb96a91d91a)

# 8. Intégration de Docker dans un environnement DevOps :
Docker joue un rôle essentiel dans un flux de développement et de déploiement continu en permettant l'isolation et la portabilité des applications dans des environnements conteneurisés. 
Voici un résumé de son rôle :

* Isolation des Environnements: Docker isole les applications et leurs dépendances dans des conteneurs légers, ce qui garantit une cohérence entre les environnements de développement, de test et de production.

* Portabilité des Applications: Les conteneurs Docker encapsulent l'application ainsi que ses dépendances, ce qui permet de les exécuter de manière cohérente sur n'importe quel environnement compatible avec Docker, qu'il s'agisse d'un ordinateur portable, d'un serveur local ou d'un cloud public.

* Facilitation des Tests: Avec Docker, les développeurs peuvent créer des environnements de test reproductibles à la demande, ce qui accélère les cycles de test et garantit la fiabilité des déploiements.

* Déploiement Rapide: Docker simplifie le processus de déploiement en permettant la création d'images prêtes à l'emploi contenant l'application et ses dépendances. Ces images peuvent être déployées rapidement et de manière cohérente sur diverses plateformes.

* Intégration Continue: Docker s'intègre facilement aux outils d'intégration continue (CI) tels que Jenkins, GitLab CI, ou Travis CI, permettant une automatisation efficace des builds, des tests et des déploiements.




  
