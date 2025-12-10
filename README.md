# TP 24 : Conteneurisation Spring Angular

## **1. Objectif du TP**

L’objectif de ce TP est de containeriser une application full-stack composée de :
* un **backend Spring Boot** connecté à une base MySQL,
* un **frontend Angular** servi via Nginx,
* un service **phpMyAdmin**
* et un **docker-compose** permettant d’orchestrer l’ensemble.
---

## **2. Architecture du TP**

L’application est divisée en 3 services principaux :

* **MySQL** pour la base de données
* **Backend Spring Boot** pour l’API REST
* **Frontend Angular** pour l’interface utilisateur

Le tout orchestré via **docker-compose**.

---

## **2.1 Stack technologique**

| Composant           | Technologie utilisée   | Version / Image          |
| ------------------- | ---------------------- | ------------------------ |
| Backend API         | Spring Boot + Maven    | OpenJDK 17 + Maven 3.8.4 |
| Frontend            | Angular                | Node 14 + Nginx          |
| Base de données     | MySQL                  | mysql:latest             |
| Administration BDD  | phpMyAdmin             | phpmyadmin/phpmyadmin    |
| Orchestration       | Docker, Docker Compose | v3                       |
| Système de build FE | npm, Angular CLI       | —                        |

---

## **2.2 Structure du projet**

<img width="535" height="575" alt="image" src="https://github.com/user-attachments/assets/3f7cd778-34b6-44cb-83bc-3167b651c472" />

---

## **3. Résultat attendu**

Après exécution des commandes :

```
docker-compose build
docker-compose up -d
```
<img width="499" height="554" alt="image" src="https://github.com/user-attachments/assets/e2a32d15-c963-403b-a67f-1794a2659891" />

### Les conteneurs doivent être démarrés :

```
docker-compose ps
```

<img width="844" height="610" alt="image" src="https://github.com/user-attachments/assets/b3571b07-f74b-455e-9a6b-601bf45904a9" />


---

## **3.1  Accès à l’application**

### Frontend Angular

`http://localhost:8080/`

### Backend Spring Boot

`http://localhost:8085/`

<img width="565" height="413" alt="image" src="https://github.com/user-attachments/assets/b04701a0-bb9f-4d92-bec8-fb2a88832256" />

### phpMyAdmin

`http://localhost:8081`
Identifiants :

* **user** : root
* **password** : root

### Démonstration

https://github.com/user-attachments/assets/9c1da263-7f8c-4719-b874-acbaca11a233
---

## Auteur
**Réalisé par :** Abla MARGHOUB <br>
**Encadré par :** Pr. Mohamed LACHGAR<br> 
**Module :** Techniques de Programmation Avancée<br> 
**Cours :** Architecture Microservices : Conception, Déploiement et Orchestration<br>
**Établissement :** École Normale Supérieure - Université Cadi Ayyad<br>
---
