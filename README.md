# ✅ Issues à créer pour OneClickMedical

## 📑 Table des matières

- [Implémenter l’authentification JWT](#implémenter-lauthentification-jwt)
- [Intégrer la connexion via Google (OAuth2)](#intégrer-la-connexion-via-google-oauth2)
- [Intégrer la connexion via Facebook (OAuth2)](#intégrer-la-connexion-via-facebook-oauth2)
- [Créer le système de rôles (RBAC)](#créer-le-système-de-rôles-rbac)
- [Mise en place des guards de sécurité par rôle](#mise-en-place-des-guards-de-sécurité-par-rôle)
- [Checklist de sécurité](#checklist-de-sécurité)
- [Création de créneaux de disponibilité (slots)](#création-de-créneaux-de-disponibilité-slots)
- [Création d’ordonnances et prescriptions](#création-dordonnances-et-prescriptions)
- [Ajout de rapports médicaux](#ajout-de-rapports-médicaux)
- [Créer un RDV en tant que médecin pour un patient](#créer-un-rdv-en-tant-que-médecin-pour-un-patient)
- [Workflow post-création du RDV](#workflow-post-création-du-rdv)
- [Prise de rendez-vous (par body malaise)](#prise-de-rendez-vous-par-body-malaise)
- [Feedback post-consultation](#feedback-post-consultation)
- [Historique des consultations](#historique-des-consultations)
- [Créer une base de données des médicaments](#créer-une-base-de-données-des-médicaments)
- [Ajout dynamique des médicaments dans une ordonnance](#ajout-dynamique-des-médicaments-dans-une-ordonnance)
- [Visualisation sécurisée du carnet médical par le patient](#visualisation-sécurisée-du-carnet-médical-par-le-patient)
- [Ajout d'observations dans le carnet médical](#ajout-dobservations-dans-le-carnet-médical)
- [Validation des soins réalisés](#validation-des-soins-réalisés)
- [Intégration de Socket.io pour chat temps réel](#intégration-de-socketio-pour-chat-temps-réel)
- [Implémentation du chatbot OCM-AI Assistant](#implémentation-du-chatbot-ocm-ai-assistant)
- [Notifications socket lors des changements de statut de RDV](#notifications-socket-lors-des-changements-de-statut-de-rdv)
- [Envoi de notifications par email](#envoi-de-notifications-par-email)
- [Création d’événements](#création-dévé-nements)
- [Tableau de bord dynamique selon rôle](#tableau-de-bord-dynamique-selon-rôle)
- [Initialiser la base de données avec Prisma](#initialiser-la-base-de-données-avec-prisma)
- [Fichier .env.example + instructions d’installation](#fichier-envexample--instructions-dinstallation)
- [Créer un README pro avec étapes de démarrage](#créer-un-readme-pro-avec-étapes-de-démarrage)
- [Mettre en place une procédure de déploiement](#mettre-en-place-une-procédure-de-déploiement)
- [Vue globale sur tous les patients et consultations](#vue-globale-sur-tous-les-patients-et-consultations)
- [Changement dynamique de rôle](#changement-dynamique-de-rôle)
- [Gestion des comptes utilisateurs (CRUD)](#gestion-des-comptes-utilisateurs-crud)
- [Logs d’activité](#logs-dactivité)
- [Super Admin : changer de rôle à la volée](#super-admin--changer-de-rôle-à-la-volée)

---

## Implémenter l’authentification JWT
**Description :** Permettre la connexion avec email et mot de passe via JWT  
**Labels :** `auth,backend,type:feature,priority:high`

## Intégrer la connexion via Google (OAuth2)
**Description :** Connexion utilisateur via Google OAuth  
**Labels :** `auth,backend,type:feature,priority:medium`

## Intégrer la connexion via Facebook (OAuth2)
**Description :** Connexion utilisateur via Facebook OAuth  
**Labels :** `auth,backend,type:feature,priority:medium`

## Créer le système de rôles (RBAC)
**Description :** Définir les rôles : patient, médecin, infirmier, super médecin, super admin, admin  
**Labels :** `auth,backend,type:feature,priority:high`

## Mise en place des guards de sécurité par rôle
**Description :** Interdire l'accès aux routes selon rôle avec NestJS guards  
**Labels :** `sécurité,backend,type:feature,priority:high`

## Checklist de sécurité
**Description :** Documenter et vérifier les règles de sécurité à chaque étape  
**Labels :** `sécurité,type:doc,priority:high`

## Création de créneaux de disponibilité (slots)
**Description :** Interface et back pour que les médecins définissent leurs horaires  
**Labels :** `médecin,backend,frontend,type:feature,priority:high`

## Création d’ordonnances et prescriptions
**Description :** Ajout d’ordonnances + sélection des médicaments depuis la base  
**Labels :** `médecin,carnet,type:feature,priority:high`

## Ajout de rapports médicaux
**Description :** Permettre au médecin d’uploader un rapport dans le carnet  
**Labels :** `médecin,carnet,type:feature,priority:medium`

## Créer un RDV en tant que médecin pour un patient
**Description :** Le médecin peut initier un rendez-vous et l’assigner à un patient  
**Labels :** `médecin,rendez-vous,frontend,backend,type:feature,priority:high`

## Workflow post-création du RDV
**Description :** Notifier et gérer le cas abonné/non-abonné après la création du RDV  
**Labels :** `rendez-vous,notifications,backend,type:feature,priority:medium`

## Prise de rendez-vous (par body malaise)
**Description :** Patient choisit une zone → proposition de créneaux  
**Labels :** `patient,frontend,type:feature,priority:high`

## Feedback post-consultation
**Description :** Patient peut noter médecin et ajouter un commentaire  
**Labels :** `patient,frontend,type:feature,priority:medium`

## Historique des consultations
**Description :** Interface avec filtres par date, médecin, statut  
**Labels :** `patient,frontend,type:feature,priority:medium`

## Créer une base de données des médicaments
**Description :** Structure table « drugs » avec nom, principe actif, posologie  
**Labels :** `backend,carnet,type:feature,priority:high`

## Ajout dynamique des médicaments dans une ordonnance
**Description :** Recherche rapide de médicaments dans le carnet  
**Labels :** `carnet,frontend,type:feature,priority:medium`

## Visualisation sécurisée du carnet médical par le patient
**Description :** Lecture seule, aucune option de téléchargement  
**Labels :** `patient,carnet,frontend,type:feature,priority:high`

## Ajout d'observations dans le carnet médical
**Description :** Notes infirmières visibles par médecin et patient  
**Labels :** `infirmier,carnet,backend,type:feature,priority:medium`

## Validation des soins réalisés
**Description :** Marquer les soins comme effectués par l'infirmier  
**Labels :** `infirmier,carnet,type:feature,priority:low`

## Intégration de Socket.io pour chat temps réel
**Description :** Patient ↔ médecin, message instantané, notifications socket  
**Labels :** `chat,frontend,backend,type:feature,priority:high`

## Implémentation du chatbot OCM-AI Assistant
**Description :** Assistant pour aider à la prise de RDV ou infos basiques  
**Labels :** `assistant,IA,frontend,type:feature,priority:medium`

## Notifications socket lors des changements de statut de RDV
**Description :** Ex: pending → confirmed, annulé, etc.  
**Labels :** `notifications,socket,backend,type:feature,priority:high`

## Envoi de notifications par email
**Description :** Ex: nouveau RDV, rappel, ordonnance disponible  
**Labels :** `notifications,email,backend,type:feature,priority:medium`

## Création d’événements
**Description :** Interface + module agenda médecin/infirmier/patient  
**Labels :** `événements,frontend,backend,type:feature,priority:medium`

## Tableau de bord dynamique selon rôle
**Description :** Indicateurs clés, résumé activité, RDV à venir  
**Labels :** `dashboard,frontend,type:feature,priority:medium`

## Initialiser la base de données avec Prisma
**Description :** Setup du schéma, migrations et seed de données  
**Labels :** `backend,base,type:setup,priority:medium`

## Fichier .env.example + instructions d’installation
**Description :** Créer un modèle d'environnement clair  
**Labels :** `setup,doc,type:config,priority:low`

## Créer un README pro avec étapes de démarrage
**Description :** Documentation de lancement projet  
**Labels :** `doc,type:doc,priority:medium`

## Mettre en place une procédure de déploiement
**Description :** Déploiement sur Railway, Vercel ou autre  
**Labels :** `devops,backend,type:setup,priority:low`

## Vue globale sur tous les patients et consultations
**Description :** Super-médecin accède à toutes les données  
**Labels :** `super-médecin,backend,frontend,type:feature,priority:high`

## Changement dynamique de rôle
**Description :** Le super-médecin peut switcher de rôle pour tester  
**Labels :** `super-médecin,auth,type:feature,priority:medium`

## Gestion des comptes utilisateurs (CRUD)
**Description :** Créer, modifier, désactiver un utilisateur  
**Labels :** `admin,backend,type:feature,priority:high`

## Logs d’activité
**Description :** Consulter les logs techniques des utilisateurs  
**Labels :** `admin,sécurité,type:feature,priority:medium`

## Super Admin : changer de rôle à la volée
**Description :** Option visible uniquement par super admin  
**Labels :** `super-admin,auth,type:feature,priority:medium`
