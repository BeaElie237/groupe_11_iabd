Nous allons vous présenter notre projet réalisé dans le cadre de l’examen de déploiement et gestion agile de modèles d’IA sur GitHub. Ce projet a été l’occasion de mettre en pratique nos compétences en gestion de versions, en collaboration sur GitHub, et en automatisation des workflows grâce à GitHub Actions. L’objectif était de développer, entraîner, valider et déployer un modèle d’IA tout en respectant les bonnes pratiques de gestion de projet et de collaboration.

---

Contexte et Objectifs :  
Le projet consistait à choisir un type de modèle d’IA (classification, régression, réseaux de neurones, etc.) et à mettre en place un pipeline complet, de la phase de prétraitement des données jusqu’au déploiement du modèle. L’accent était mis sur la collaboration via GitHub, la gestion des branches, et l’automatisation des processus avec GitHub Actions.  

Les objectifs principaux étaient :  
1. Collaboration efficace : Utiliser des branches individuelles pour chaque contributeur et gérer les fusions via des pull requests.  
2. Automatisation : Configurer un workflow GitHub Actions pour entraîner, valider et déployer le modèle à chaque push sur la branche main.  
3. Documentation et Sécurité : Générer automatiquement la documentation avec Pydoc et sécuriser les informations sensibles (comme les credentials SMTP) avec GitHub Secrets.

---

Structure du Projet :  
Le dépôt GitHub est organisé de la manière suivante :  
- Branches : Une branche main pour le code stable, et des branches individuelles pour chaque contributeur.  
- Répertoires :  
  - script : Contient les scripts Python pour le prétraitement, l’entraînement et l’évaluation du modèle.  
  - notebook : Jupyter Notebooks pour les analyses exploratoires et les explications détaillées.  
  - model : Stocke les modèles entraînés.  
  - data : Gère les ensembles de données via Git LFS pour les fichiers volumineux.  
  - doc : Documentation générée automatiquement avec Pydoc.  
  - keys : Contient les secrets et configurations sécurisés via Git Secrets.

---

Workflow GitHub Actions :  
Le cœur du projet réside dans l’automatisation avec GitHub Actions. Voici les étapes clés du workflow :  
1. Checkout du code : Récupération du code et des données avec Git LFS.  
2. Installation des dépendances : Installation des bibliothèques Python nécessaires.  
3. Prétraitement des données : Exécution du script de prétraitement.  
4. Entraînement du modèle : Entraînement du modèle avec les données préparées.  
5. Évaluation du modèle : Validation des performances du modèle.  
6. Archivage et envoi par e-mail : Archivage du modèle et de la documentation, puis envoi aux membres de l’équipe via e-mail.  

Chaque étape est commentée dans le fichier YAML pour une meilleure compréhension.

---

Collaboration et Bonnes Pratiques :  
Pour garantir une collaboration fluide, nous avons :  
- Utilisé des commits significatifs pour décrire clairement chaque modification.  
- Mis en place des pull requests pour fusionner les branches individuelles avec main, en veillant à ce que chaque PR soit revue par un autre membre.  
- Chaque membre a contribué à tous les scripts, assurant une répartition équitable du travail.


Résultats et Livrables :  
Le projet a abouti à :  
- Un dépôt GitHub bien structuré, avec au moins trois branches et des contributions claires de chaque membre.  
- Un workflow GitHub Actions fonctionnel, automatisant l’entraînement, la validation et le déploiement du modèle.  
- Une documentation générée automatiquement et sécurisée avec GitHub Secrets pour les informations sensibles.  
- Un modèle d’IA entraîné et déployé, prêt à être utilisé.
