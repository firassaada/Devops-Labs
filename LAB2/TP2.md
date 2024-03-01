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

# 5. Compréhension de l'Application SpringBoot :

![Capture d'écran 2024-03-01 030518](https://github.com/firassaada/Devops-Labs/assets/92325496/efb9e45e-f1df-4dcd-8ca2-cd133721f774)

![Capture d'écran 2024-03-01 030711](https://github.com/firassaada/Devops-Labs/assets/92325496/607c57e3-20e1-41af-bd45-6eb59c06b0d0)

![Capture d'écran 2024-03-01 030721](https://github.com/firassaada/Devops-Labs/assets/92325496/d6603ead-a1af-48f6-aa63-7ea0f5e33fdf)


# 6. Containerisation de l'Application : 

1-Lancer un container avec l’image officielle mongo :

![Capture d'écran 2024-03-01 015635](https://github.com/firassaada/Devops-Labs/assets/92325496/8f8c8f7e-fc4a-499e-a3bb-c18696d07a84)

2.1 - Création du network bridge pour assurer la communication entre les images mongo-db et l'image de notre application :

![Capture d'écran 2024-03-01 015808](https://github.com/firassaada/Devops-Labs/assets/92325496/a0066c2d-d2d7-418b-b873-efe8a3131d1c)

2.2 - Build de conteneur de notre application spring a partir du DockerFile

![Capture d'écran 2024-03-01 022053](https://github.com/firassaada/Devops-Labs/assets/92325496/4adb7cbd-5bbb-493d-b474-c4d9036b1893)

2.3 - Création de l'image a partir du conteneur déja crée :

![Capture d'écran 2024-03-01 022219](https://github.com/firassaada/Devops-Labs/assets/92325496/d791a004-446f-407e-a0ae-cc2dcef5fc16)

3- Test et validation :

![Capture d'écran 2024-03-01 022728](https://github.com/firassaada/Devops-Labs/assets/92325496/7a849fa5-f347-46be-aee0-e519e0f41d4e)

![Capture d'écran 2024-03-01 022425](https://github.com/firassaada/Devops-Labs/assets/92325496/0fd0fe3f-a4c4-41b7-b10b-a1c3de8cff20)

![Capture d'écran 2024-03-01 022412](https://github.com/firassaada/Devops-Labs/assets/92325496/51e19953-fe34-49d4-b151-617d962fd269)

4 - Lancement de l'application avec plusieur port:

![Capture d'écran 2024-03-01 022836](https://github.com/firassaada/Devops-Labs/assets/92325496/d8a07f09-e20c-49a4-ba1f-ed6ba5c875f3)

5 -Test et validation :

![Capture d'écran 2024-03-01 022859](https://github.com/firassaada/Devops-Labs/assets/92325496/46e1983d-9eb7-450f-aabe-fd53966731f4)


![Capture d'écran 2024-03-01 022849](https://github.com/firassaada/Devops-Labs/assets/92325496/23d1a7a5-7e7b-4aad-ba4d-cd420dffc5a4)


# 7. Docker Compose : 

1-Docker compose file :

![Capture d'écran 2024-03-01 031808](https://github.com/firassaada/Devops-Labs/assets/92325496/4c694613-95b7-42dd-88e4-50b3ecad3463)

2- Build des images à travers du docker compose:

![Capture d'écran 2024-03-01 023832](https://github.com/firassaada/Devops-Labs/assets/92325496/c1ba86b9-20ff-4784-938a-e803dee382da)


3- Test et Validation :

![Capture d'écran 2024-03-01 024151](https://github.com/firassaada/Devops-Labs/assets/92325496/faf39101-ef19-4d5f-913c-1ad63b31c5f4)


![Capture d'écran 2024-03-01 024106](https://github.com/firassaada/Devops-Labs/assets/92325496/9a88d089-104c-4c20-ac4d-62029f72ed9f)



# 8. Intégration de Docker dans un environnement DevOps :
Docker joue un rôle essentiel dans un flux de développement et de déploiement continu en permettant l'isolation et la portabilité des applications dans des environnements conteneurisés. 
Voici un résumé de son rôle :

* Isolation des Environnements: Docker isole les applications et leurs dépendances dans des conteneurs légers, ce qui garantit une cohérence entre les environnements de développement, de test et de production.

* Portabilité des Applications: Les conteneurs Docker encapsulent l'application ainsi que ses dépendances, ce qui permet de les exécuter de manière cohérente sur n'importe quel environnement compatible avec Docker, qu'il s'agisse d'un ordinateur portable, d'un serveur local ou d'un cloud public.

* Facilitation des Tests: Avec Docker, les développeurs peuvent créer des environnements de test reproductibles à la demande, ce qui accélère les cycles de test et garantit la fiabilité des déploiements.

* Déploiement Rapide: Docker simplifie le processus de déploiement en permettant la création d'images prêtes à l'emploi contenant l'application et ses dépendances. Ces images peuvent être déployées rapidement et de manière cohérente sur diverses plateformes.

* Intégration Continue: Docker s'intègre facilement aux outils d'intégration continue (CI) tels que Jenkins, GitLab CI, ou Travis CI, permettant une automatisation efficace des builds, des tests et des déploiements.

On peut maximiser la sécurité de nos déploiements Docker en production et réduire les risques de compromission de la sécurité en suivants certains pratiques :

    *Utilisation de Docker Bench Security:
    * Mises à jour régulières des images: 
    * Réduction de la surface d'attaque: 
    Minimisez la taille des images Docker en supprimant les composants inutiles et en utilisant des images de base minimales pour réduire la surface d'attaque potentielle.
    * Configuration sécurisée des conteneurs:
    Appliquez les principes du modèle de sécurité du principe du moindre privilège en limitant les privilèges des conteneurs Docker et en désactivant les fonctionnalités          potentiellement dangereuses comme les capacités, les points de montage sensibles, et l'accès au système hôte.
    * Authentification et autorisation: 
    Mettez en place des mécanismes d'authentification et d'autorisation robustes pour contrôler l'accès aux ressources Docker, y compris      les registres Docker, les API       Docker, et les ressources de conteneurs.
    * Sécurisation des connexions réseau: 
    Utilisez des réseaux Docker sécurisés, tels que des réseaux privés virtuels (VPN) ou des réseaux overlay chiffrés, pour sécuriser les communications entre les conteneurs     et les hôtes Docker.



  
