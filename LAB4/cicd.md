# CICD :
## Phase de Build (CI) :

Dans cette phase:
Chaque fois qu'un développeur pousse du code vers notre répertoire GitHub,un BUILD est déclenché grâce à AWS CodeBuild. 
CodeBuild récupère le code et exécute les étapes de construction définies dans notre fichier buildspec.yml,
telles que la création d'une image Docker à partir du Dockerfile et son stockage dans Amazon ECR (Elastic Container Registry).
Ce processus garantit une construction cohérente et reproductible de notre application à chaque modification du code.

## Artifact : 

Une fois l'image Docker construite et stockée dans Amazon ECR, le fichier imagedefinitions.json est créé comme artefact de build, contenant les détails de l'image. 

## Phase de Déploiement(CD) :

l'artifact est ensuite utilisé pour déployer l'image sur un cluster ECS via AWS ECS.
Une fois déployée, la dernière version de l'application fonctionne dans un conteneur ECS en cours d'exécution,permettant la validation du déploiement.
Ce pipeline CI/CD accélère le développement, assure la cohérence des déploiements et garantit une meilleure qualité logicielle grâce à des tests automatisés.

![image](https://github.com/firassaada/Devops-Labs/assets/94303698/4e296364-47f4-4996-a265-e1ffa424c204)

![image](https://github.com/firassaada/Devops-Labs/assets/94303698/b85dda82-babb-4ad2-85aa-4e2606e9c10a)

# CICD with manual approval :

## Phase d'Approbation Manuelle :

Dans cette nouvelle phase d'approbation manuelle, une fois que l'image Docker est construite avec succès et que le fichier imagedefinitions.json est produit comme artefact de build, le processus est temporairement suspendu. Un membre de l'équipe responsable du déploiement est alors notifié et invité à examiner les modifications proposées. Ce membre peut alors examiner les détails de l'image à déployer, y compris son nom, son tag et son URI, ainsi que toute autre information pertinente sur les changements introduits. Une fois que l'équipe est satisfaite des modifications, l'approbation manuelle est donnée, déclenchant ainsi la phase de déploiement.

![image](https://github.com/firassaada/Devops-Labs/assets/94303698/b690d26e-ebc6-44af-b7c8-ca234166431e)

![image](https://github.com/firassaada/Devops-Labs/assets/94303698/4d585317-b6da-42ed-80d3-c5b09337a61a)

![image](https://github.com/firassaada/Devops-Labs/assets/94303698/ba6e2f58-e8c5-4282-860b-3ecdf90b9a65)

![image](https://github.com/firassaada/Devops-Labs/assets/94303698/b3fde192-6f70-4ef8-8dfe-40c783ed9b00)

# CD with Iac(Terraform) :

