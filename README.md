# Mini-Projet DevOps avec Jenkins, ArgoCD et Helm  

![Site Web](https://staticassets.oxfam.org.uk/oxfamgb-production/images/OGB_122546_DSC_0280Emma_James_English.width-1000.jpg)  

## 🌟 Présentation du Site Web  
**Clothes STORE** est une plateforme web conçue pour comparer les prix entre différents fournisseurs de vêtements. Elle offre une solution pratique et efficace pour aider les utilisateurs à trouver les meilleures offres tout en simplifiant la gestion des fournisseurs et des produits.  

---

## 🎯 Objectifs du Projet  
Ce projet vise à conteneuriser et déployer une application web en utilisant Docker, Kubernetes et Jenkins pour l'intégration continue (CI). L'application est orchestrée sur un cluster Kubernetes local ( Minikube ).  

---

## ⚙️ Technologies Utilisées  

- **Docker** 🐳 : Conteneurisation.  
- **Jenkins** 🔧 : Intégration continue et automatisation des builds.  
- **Kubernetes** ☸️ : Orchestration des conteneurs.  
- **Helm** ⛵ : Déploiement des applications sur Kubernetes.  
- **ArgoCD** 🚀 : Gestion et automatisation des déploiements.  
- **Prometheus** 📈 : Monitoring et observabilité.  
- **Grafana** 📊 : Visualisation des métriques et analyse des données.  
 

---

## 🛠️ Étapes de Réalisation  

### 1️⃣ Création des Dockerfiles  
- **Server** : Création d’un fichier **Dockerfile** dans le dossier serveur.  
- **Client** : Création d’un fichier **Dockerfile** dans le dossier client.  
- **Docker Compose** : Fichier `docker-compose.yml` à la racine du projet pour orchestrer les conteneurs.  

![Docker](https://i.ibb.co/qjPw3cY/Capture.jpg)  

---

### 2️⃣ Mise en Place du CI avec Jenkins  
Pipeline Jenkins :  
1. **Start** : Initialisation de la pipeline.  
2. **Checkout SCM** : Récupération du code source depuis le dépôt.  
3. **Build Server Image** : Construction de l'image Docker pour le serveur.  
4. **Scan Server Image** : Analyse de l'image Docker pour détecter les vulnérabilités.  
5. **Build Client Image** : Construction de l'image Docker pour le client.  
6. **Scan Client Image** : Analyse de l'image Docker pour détecter les vulnérabilités.  
7. **Test Docker Hub Connectivity** : Vérification de la connexion au Docker Hub.  
8. **Push Images to Docker Hub** : Publication des images.  
9. **End** : Fin de la pipeline.  

![Pipeline Jenkins](https://i.ibb.co/4g5VfCr/pipeline-3.png)  

---

### 3️⃣ Déploiement avec Kubernetes  
Déploiement sur un cluster Kubernetes local :  
- **Configuration du cluster** : Installation et configuration avec Minikube, Kind ou k3s.  
- **Manifestes Kubernetes** : Déploiement des ressources nécessaires (Deployments, Services).  
- **Helm Charts** : Gestion et automatisation des déploiements avec Helm.  
- **ArgoCD** : Implémentation GitOps pour les déploiements.  

![ArgoCD](https://i.ibb.co/PTzgWFK/argocd-4.png)  

---

### 4️⃣ Monitoring avec Prometheus et Grafana  
- **Installation** : Déploiement de Prometheus et Grafana dans le namespace monitoring.
  ![Prometheus](https://i.ibb.co/5WZ8DqC/promethus-6.png)  

- **Configuration** : Collecte des métriques avec Prometheus et visualisation via Grafana.  

![Grafana](https://i.ibb.co/y84gNhk/installation-grafana-7.png)  

---

## ✅ Conclusion  
Ce projet a permis de mettre en œuvre une architecture robuste et scalable à l'aide de technologies modernes comme Docker, Kubernetes, Helm et ArgoCD. L'automatisation CI/CD garantit une gestion efficace des versions, une rapidité de mise à jour et une fiabilité accrue.  

---

## 📝 License  
Copyright (c) 2025 **[Chaabane Ben Fraj](https://www.github.com/chaabane123)**  

---

## 📬 Contact  
Pour toute question, n'hésitez pas à me contacter :  
- **Email** : [chaabane.benfraj@polytechnicien.tn](mailto:chaabane.benfraj@polytechnicien.tn)  
- **GitHub** : [Chaabane Ben Fraj](https://www.github.com/chaabane123)  
