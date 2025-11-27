# Backlog du projet

Pour voir les détails des User Stories, se référer au fichier [Sprint0/Sprint0.md](Sprint0/Sprint0.md).
Pour voir les tâches associées à chaque User Story, se référer au fichier [Sprint0/US_Tasks.md](Sprint0/US_Tasks.md).

--- 

## Planification des Sprints

### Sprint 1 (25/10 au 05/11)

**Objectifs :**
- Permettre aux utilisateurs de créer un compte et se connecter.
- Permettre la création de base d'un projet.

**Tâches prévues :**

#### US1 : Création de Compte
- T1.1 : Concevoir le schéma de base de données pour les utilisateurs — 1 pt  
- T1.2 : Développer l'API de création de compte — 1 pt  
- T1.3 : Implémenter la validation des données utilisateur client/serveur — 1 pt  
- T1.4 : Créer le formulaire d'inscription front-end — 1 pt  

#### US2 : Connexion au Compte
- T2.1 : Implémenter l'authentification JWT — 2 pts  
- T2.2 : Implémenter l'API de connexion — 1 pt  
- T2.3 : Créer le formulaire de connexion front-end — 1 pt  

#### US3 : Gestion de Profil
- T3.1 : Développer l'API de gestion de profil — 1 pt  
- T3.2 : Interface de modification du profil utilisateur — 1 pt  
- T3.3 : Changement de mot de passe — 1 pt  

#### US4 : Création de Projet
- T4.1 : Développer l'API de création de projet — 1 pt  
- T4.2 : Concevoir la base de données pour les projets — 1 pt  
- T4.3 : Créer l'interface front-end pour la création de projet — 1 pt  


**Répartition des tâches :**
Kenzo: T1.4, T2.3, T4.3, T3.2
Felix: T1.2, T1.3, T2.1, T2.2
Justus: T1.1, T3.1, T3.3, T4.1, T4.2

**Coût total du Sprint :**
14 points

### Sprint 2 (06/11 au 19/11)

**Objectifs :**
- Gérer la structure et les membres d’un projet.  
- Mettre en place la sauvegarde automatique des données. 
- Issues et Tâches
- Gestion du backlog. 
- Visualisation et assignation des tâches.

**Tâches prévues :**

#### US5 : Gestion de Projet
- T5.1 : Développer l'API de gestion des membres — 2 pts  
- T5.2 : Implémenter les paramètres de projet — 1 pt  
- T5.3 : Créer l'interface front-end pour la gestion des membres — 1 pt  
- T5.4 : Créer l'interface front-end pour les paramètres du projet — 1 pt  
- T5.5 : Contrôles d'accès basés sur les rôles — 1 pt  

#### US6 : Sauvegarde des Données
- T6.1 : Créer la base de données de sauvegarde — 1 pt  
- T6.2 : Implémenter la sauvegarde automatique — 2 pts  
- T6.3 : Implémenter la restauration automatique — 1 pt  

#### US7 à US10 : Issues et Tâches
- T7.1 : Développer l'API de création d'issue (POST /projects/:id/issues), une issue est composée d'un titre, d'une description et d'une priorité - 1 point
- T7.2 : Créer le formulaire de création d'issue (front-end) - 1 point
- T8.1 : Développer l'API d'assignation d'issue (PUT /projects/:id/issues/:issueId/assign) - 1 point
- T8.2 : Créer le formulaire d'assignation d'issue (front-end) - 1 point
- T9.1 : Développer l'API de modification du statut d'issue (PUT /projects/:id/issues/:issueId/status) - 1 point
- T9.2 : Créer l'interface front-end pour changer le statut (dropdown/boutons) - 1 point
- T10.1 : Développer l'API de création de tâches liées aux issues (POST /projects/:id/issues/:issueId/tasks) - 1 point
- T10.2 : Créer le formulaire de création de tâches (front-end) - 1 point

#### US11 à US14 : Backlog, Kanban, Assignations, Temps
- T11.1 : Développer l'API de récupération du backlog (GET /projects/:id/backlog) - 1 point
- T11.2 : Créer la vue liste du backlog (front-end) - 1 point
- T11.3 : Implémenter les filtres et tri du backlog - 1 point
- T12.1 : Créer la vue Kanban pour les tâches (front-end) - 1 point
- T12.2 : Implémenter le toggle entre vue Kanban et vue liste - 1 point  
- T13.1 : Développer l'API pour récupérer les tâches assignées à un utilisateur (GET /users/me/tasks) - 1 point
- T13.2 : Créer le dashboard personnel des tâches assignées (front-end) - 1 point 


### Coût total du Sprint 2 : **25 points**


### Sprint 3 (20/11 au 03/12)

**Objectifs :**

**Tâches prévues :**
- suivi du temps
- releases, tests et documentation.  

#### US14 à US16 : Releases
- T14.1 : Ajouter les champs de temps estimé/passé à la base de données et API (PUT /tasks/:id/time) - 1 point
- T14.2 : Créer l'interface de saisie du temps (front-end) - 1 point
- T15.1 : Développer l'API de création de releases (POST /projects/:id/releases) - 1 point
- T15.2 : Créer l'interface de création de release/tag (front-end) - 1 point
- T16.1 : Développer l'API d'historique des releases (GET /projects/:id/releases) - 1 point
- T16.2 : Créer la vue timeline des releases (front-end) - 1 point

#### US17 à US19 : Tests
- T17.1 : Développer l'API de création de cas de test (POST /projects/:id/test-cases) - 1 point
- T17.2 : Créer le formulaire de création de cas de test (front-end) - 1 point
- T18.1 : Développer l'API d'exécution de test (POST /test-cases/:id/execute) - 1 point
- T18.2 : Créer l'interface d'exécution et mise à jour des résultats (front-end) - 1 point
- T19.1 : Développer l'API des statistiques de tests (GET /projects/:id/test-dashboard) - 1 point
- T19.2 : Créer le dashboard des tests avec graphiques (front-end) - 1 point

#### US20 à US22 : Documentation
- T20.1 : Développer l'API CRUD pour la documentation (POST/PUT/GET/DELETE /projects/:id/docs) - 1 point
- T20.2 : Créer l'éditeur Markdown pour la documentation (front-end) - 1 point
- T21.1 : Implémenter le système de catégories/sections pour la documentation (base de données + API) - 1 point
- T21.2 : Créer la navigation arborescente de la documentation (front-end) - 1 point
- T22.1 : Développer l'API de liaison documentation-issues (POST /docs/:id/link-issue) - 1 point
- T22.2 : Créer l'interface de liaison dans l'éditeur de documentation (front-end) - 1 point


**Coût total du Sprint 3 :** **18 points**
