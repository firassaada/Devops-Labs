# 1. Installation et configuration de Kubernetes :
Nous avons intalle minikube et on a éxecuté la commande 
minukbe start
![Capture d'écran 2024-05-09 222145](https://github.com/firassaada/Devops-Labs/assets/92325496/e735a222-5c6b-4ce1-aab4-1ded1cd6564f)

-le cluster est démarré :
![Capture d'écran 2024-05-10 024945](https://github.com/firassaada/Devops-Labs/assets/92325496/143edd90-63ba-4f08-bfeb-99f5f988e509)

# 2. Déploiement de l'application :

Nous avons créer une application ExpressJs qui retourne "Hello World" pour une requete GET , puis nous avons contenarisé cette application 

![Capture d'écran 2024-05-09 224928](https://github.com/firassaada/Devops-Labs/assets/92325496/0bb26e26-f05a-4780-a3f3-224a694e908a)

![Capture d'écran 2024-05-09 224907](https://github.com/firassaada/Devops-Labs/assets/92325496/c0a25b46-c765-46f6-aec1-c0bf56565362)

on de même publier cette application dans le DockerHub 
![Capture d'écran 2024-05-09 231406](https://github.com/firassaada/Devops-Labs/assets/92325496/ea092fbf-094a-4f8a-969a-bfccdd31df66)

puis nous avons crée un fichier YAML pour assurer le deploiement de l'application 

![Capture d'écran 2024-05-10 001711](https://github.com/firassaada/Devops-Labs/assets/92325496/c15b4749-1c51-482b-83b8-21a713237166)

et lancer la commande pour faire le deploiement 

![Capture d'écran 2024-05-10 001659](https://github.com/firassaada/Devops-Labs/assets/92325496/6849725f-286c-4c55-897d-c3266419dc6a)

![Capture d'écran 2024-05-10 001835](https://github.com/firassaada/Devops-Labs/assets/92325496/de959dc9-0f59-442b-8f7e-969019489e7e)

# 3. Gestion des répliques :

nous avons lancer cette commande pour la gestion des repliques :
kubectl scale deployment nom-du-deploiement --replicas=5

![Capture d'écran 2024-05-10 002035](https://github.com/firassaada/Devops-Labs/assets/92325496/7d550dc9-1d9f-4f74-966d-ea35a9b5c2fd)

# Définition des services :

![Capture d'écran 2024-05-10 031342](https://github.com/firassaada/Devops-Labs/assets/92325496/2602294a-e05c-4b52-9a6e-b2570f32042d)

![Capture d'écran 2024-05-10 005253](https://github.com/firassaada/Devops-Labs/assets/92325496/f828316c-68db-4d5e-b78c-8fe014791fec)

# 5. Exposition externe de l'application :

nous avons crée un Load-Balancer 

![Capture d'écran 2024-05-10 011823](https://github.com/firassaada/Devops-Labs/assets/92325496/fa108d65-3420-4fc5-bbfd-7f087fec3b81)

![Capture d'écran 2024-05-10 005857](https://github.com/firassaada/Devops-Labs/assets/92325496/c6e25b2a-ecd4-48a6-99c6-f680fdf6882c)

et on a pu vérifié que l'application est en train de s'executer et on a pu lui accéder de l'externe : 

![Capture d'écran 2024-05-10 011944](https://github.com/firassaada/Devops-Labs/assets/92325496/af4e3948-a38e-4432-a1a7-61c979f96571)


# 6. Gestion des mises à jour :

on a modifié l'application de façon qu'elle donne une autre réponse "Hello world version2" , on l'a contenerisé de façon a avoir un autre version (2.0) de la meme image , puis on a publié une 2eme version de l'image sur DockerHub 

![Capture d'écran 2024-05-10 014818](https://github.com/firassaada/Devops-Labs/assets/92325496/808fa396-b064-4060-9626-0b36580df5b0)

d'ou le resultat finale 

![Capture d'écran 2024-05-10 014940](https://github.com/firassaada/Devops-Labs/assets/92325496/5e998450-bf96-44b6-8fcd-5cadac160d93)









