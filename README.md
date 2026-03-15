# Application Chat Temps Réel

> **Projet académique** - Module Technologies JS et Développement Mobile  
> ENSA Khouribga | 2025-2026  
> **Équipe de 4 personnes** - **Projet réalisé principalement par 1 membre**

---

## Objectif

Messagerie instantanée full-stack avec communication temps réel intégrant :
- Backend Node.js/Express + MongoDB
- Frontend React responsive
- Socket.IO pour messagerie instantanée
- Authentification JWT/Passport.js

**Contexte :** Projet de groupe où une seule personne a pu développer l'application complète en raison de contraintes de temps liées à d'autres projets simultanés.

---

## Technologies

**Backend**
- Node.js + Express.js (serveur)
- MongoDB + Mongoose (base de données)
- Socket.IO (WebSocket temps réel)
- JWT + Passport.js (authentification)
- bcrypt (chiffrement mots de passe)

**Frontend**
- React (interface utilisateur)
- Context API (gestion état)
- Socket.IO client (temps réel)
- Responsive design

---

## Architecture de l'Application

### Backend (Node.js/Express)

**Structure MVC complète :**
```
backend/
├── config/
│   ├── db.js (connexion MongoDB)
│   ├── passport.js (stratégies auth)
│   └── socket.js (configuration Socket.IO)
│
├── controllers/
│   ├── authController.js
│   ├── userController.js
│   ├── roomController.js
│   └── messageController.js
│
├── middleware/
│   ├── authenticate.js (vérification JWT)
│   └── errorHandler.js
│
├── models/
│   ├── User.js (schéma MongoDB)
│   ├── Room.js (salons de discussion)
│   └── Message.js (messages)
│
├── routes/
│   ├── authRoutes.js (inscription, connexion)
│   ├── userRoutes.js (profils)
│   ├── roomRoutes.js (salons)
│   └── messageRoutes.js (messages)
│
└── utils/
    ├── generateToken.js (JWT)
    ├── validators.js
    └── logger.js
```

**Fonctionnalités backend :**
- API REST complète (CRUD utilisateurs, salons, messages)
- Authentification JWT + Google OAuth
- Validation et sécurisation (bcrypt, sanitization)
- Architecture MVC bien structurée

### Frontend (React)

**Structure composants :**
```
frontend/
├── components/
│   ├── Auth/ (inscription, connexion)
│   ├── Chat/ (interface messagerie)
│   ├── Rooms/ (gestion salons)
│   ├── Users/ (liste utilisateurs)
│   └── Layout/ (header, sidebar)
│
├── context/
│   ├── AuthContext.jsx (gestion auth)
│   ├── ChatContext.jsx (état chat)
│   ├── SocketContext.jsx (Socket.IO)
│   └── NotificationContext.jsx
│
├── hooks/
│   ├── useAuth.js
│   ├── useChat.js
│   └── useSocket.js
│
└── services/
    ├── api.js (appels API)
    ├── authService.js
    ├── chatService.js
    └── roomService.js
```

**Fonctionnalités frontend :**
- Interface responsive (mobile/desktop)
- Messagerie temps réel Socket.IO
- Salons publics/privés
- Modes clair/sombre
- Typing indicators
- Accusés de lecture

---

## Fonctionnalités Implémentées

### Authentification
- ✅ Inscription avec validation
- ✅ Connexion JWT
- ✅ Google OAuth
- ✅ Déconnexion sécurisée

### Messagerie
- ✅ Messages temps réel (Socket.IO)
- ✅ Salons publics (accès libre)
- ✅ Salons privés (sur invitation)
- ✅ Typing indicators ("X est en train d'écrire...")
- ✅ Horodatage messages
- ✅ Accusés de lecture
- ✅ Édition/suppression messages

### Interface
- ✅ Design responsive (PC/mobile)
- ✅ Modes clair/sombre (sauvegarde préférences)
- ✅ Statuts en ligne temps réel
- ✅ Notifications

---

## Documentation

**[Rapport de projet (PDF)](docs/rapport-projet.pdf)** *(si disponible)*

*Ce projet illustre une application full-stack MERN (MongoDB, Express, React, Node.js) complète avec communication temps réel.*

---

## Compétences Découvertes (Observation du Projet)

**Backend**
- Architecture Node.js/Express (MVC)
- MongoDB/Mongoose (NoSQL)
- API REST (authentification, CRUD)
- Socket.IO (WebSocket)
- Sécurité (JWT, bcrypt)

**Frontend**
- React (composants, hooks)
- Context API (gestion état)
- Socket.IO client
- Design responsive

**Architecture**
- Full-stack MERN
- Communication temps réel
- Authentification complète

---

## 💭 Réflexion Personnelle

**Apprentissage :
- Comprendre l'architecture d'une application full-stack moderne
- Découvrir Socket.IO pour la communication temps réel
- Observer les bonnes pratiques de structuration backend/frontend
- Apprécier la complexité d'un projet MERN Stack complet

---

## Contact

**Wissal RHANDI**
- 📧 wissalrhandi685@gmail.com
- 💼 [LinkedIn](https://linkedin.com/in/wissalrhandi)
- 📍 Khouribga, Maroc
