# JudyApp - Gestion des factures avec Postman 🧾

Une application simple construite avec **Spring Boot** pour gérer les factures via une API REST. Ce projet a été conçu à des fins pédagogiques afin de pratiquer les opérations CRUD avec Postman.

---
Je me suis mise dans la peau d’une entreprise qui souhaite gérer ses factures d’une manière simple et rapide. L’idée derrière ce projet est d’apprendre à manipuler les opérations CRUD à travers une API REST en Java avec Spring Boot.
Ce projet fait partie de ma formation chez Studi et m’a permis de mieux comprendre la logique d’une application backend simple, tout en pratiquant avec des outils professionnels comme IntelliJ IDEA, Postman et GitHub.
---
Objectifs

    Créer un système simple pour ajouter, modifier, consulter et supprimer des factures.

    Simuler un projet réel pour mieux comprendre le fonctionnement d’une API REST avec Java Spring Boot.

    Organiser le projet de façon structurée (controller, model, repository).

    Mettre en pratique les bonnes habitudes de développement avec Git et Maven.

    Tester les routes HTTP via Postman.

 Sécurité & rôles utilisateurs

    Remarque : Ce projet étant un projet d’apprentissage individuel, je n’ai pas encore implémenté la gestion des utilisateurs ni de système d’authentification.
    Mais j’ai bien compris que dans une application réelle, il est essentiel de :

    Protéger l’accès aux routes sensibles via un système de login/mot de passe.

    Définir des rôles (comme admin, comptable, utilisateur simple) pour mieux contrôler les actions possibles.

    Chiffrer les données sensibles des utilisateurs (ex. mots de passe).

Ce sont des notions que je souhaite approfondir dans mes futurs projets
    
## 🔧 Technologies utilisées

- **Langage** : Java 21  
- **Framework** : Spring Boot  
- **Base de données** : H2 (mémoire)  
- **API** : RESTful (HTTP)  
- **IDE** : IntelliJ IDEA  
- **Outils de versionnage** : Git & GitHub  
- **Gestion des dépendances** : Maven  

---

## ✅ Fonctionnalités de l’API

- `GET /api/invoices` → Obtenir la liste de toutes les factures  
- `GET /api/invoices/{id}` → Récupérer une facture par son identifiant  
- `POST /api/invoices` → Créer une nouvelle facture  
- `PUT /api/invoices/{id}` → Mettre à jour une facture existante  
- `DELETE /api/invoices/{id}` → Supprimer une facture  

---

## 🗂️ Structure du projet

```
judyapp/
 ├── controller/         → Gère les requêtes HTTP (InvoiceController.java)
 ├── model/              → Modèle de données (Invoice.java)
 ├── repository/         → Interface JPA (InvoiceRepository.java)
 ├── resources/
 │   └── application.properties → Configuration (port, DB, etc.)
 ├── pom.xml             → Dépendances Maven
 └── README.md           → Documentation du projet
```
![java](https://github.com/user-attachments/assets/40e8352b-ff1a-46be-b2e7-bbc1cafdaf43)

---

## ▶️ Comment exécuter l'application localement

1. Ouvrir le projet avec **IntelliJ IDEA**  
2. Vérifier que **Java 21** est bien installé  
3. Lancer la classe `JudyappApplication.java` *(clic droit > Run)*  
4. Accéder à l’API via : `http://localhost:8080/api/invoices`  

---

## 📬 Exemples d'utilisation avec Postman

### ➕ POST – Ajouter une facture

**URL** : `http://localhost:8080/api/invoices`  
**Méthode** : POST  
**Body** (raw = JSON) :
```json
{
  "clientName": "Eman",
  "amount": 1200,
  "description": "ACHETER UN ORDINATEUR"
}
```

---

### 📥 GET – Obtenir toutes les factures

**URL** : `http://localhost:8080/api/invoices`  
**Méthode** : GET

---

### 🔄 PUT – Modifier une facture

**URL** : `http://localhost:8080/api/invoices/1`  
**Méthode** : PUT  
**Body** :
```json
{
  "clientName": "Eman Updated",
  "amount": 1500,
  "description": "ORDINATEUR MIS À JOUR"
}
```

---

### ❌ DELETE – Supprimer une facture

**URL** : `http://localhost:8080/api/invoices/1`  
**Méthode** : DELETE  

---

## 📸 Captures d’écran

### ✅ Ajoutez ici des images Postman :

- ☑️ Réponse 200 OK  
- ☑️ Réponse après POST  
- ☑️ Réponse après PUT  
- ☑️ Réponse après DELETE  

```

```

![get](https://github.com/user-attachments/assets/2248f6ce-046b-419d-9c63-d975d128e64d)
![GET BY ID](https://github.com/user-attachments/assets/36b78603-f71a-4f0c-81b9-dabf94fb4d95)
![delete](https://github.com/user-attachments/assets/ec540006-2fe2-408d-a7c3-d71b93214279)
![put](https://github.com/user-attachments/assets/1b19c87d-78f6-41d2-8497-34ddde466d76)
![PUST](https://github.com/user-attachments/assets/fe57043f-f4ec-4ff0-8819-0322c1fb30f0)

--

## 👩‍💻 Développeuse

**Nom** : Eman Abdulgader  
**GitHub** : [eman-java-dev](https://github.com/eman-java-dev)  
**Projet** : Formation Développeur d’Application (Studi)

---



