# Backlog du Projet - Gestion de Projet Agile

## Vue d'ensemble

Ce projet vise à créer une **plateforme de gestion de projet agile** permettant de gérer les utilisateurs, projets, issues, tâches, tests, releases et documentation.

### Technologies
- **Frontend:** Vue.js
- **Backend:** Spring Boot / Java
- **Base de données:** PostgreSQL, MongoDB (Docker)
- **Outils:** GitHub, Slack/Discord

---

## Résumé du Backlog

| ID | User Story | Priorité | Estimation | Sprint |
|----|------------|----------|------------|--------|
| US1 | Création de Compte | Haute | 4 pts | Sprint 1 |
| US2 | Connexion au Compte | Haute | 4 pts | Sprint 1 |
| US3 | Gestion de Profil | Moyenne | 3 pts | Sprint 1 |
| US4 | Création de Projet | Haute | 3 pts | Sprint 1 |
| US5 | Gestion de Projet | Haute | 5 pts | Sprint 2 |
| US6 | Sauvegarde des Données | Haute | 4 pts | Sprint 2 |
| US7 | Création d'une Issue | Haute | 2 pts | Sprint 2 |
| US8 | Assignation d'une Issue | Haute | 2 pts | Sprint 2 |
| US9 | Modification du Statut d'une Issue | Haute | 2 pts | Sprint 2 |
| US10 | Création de Tâches | Haute | 2 pts | Sprint 2 |
| US11 | Visualisation du Backlog | Haute | 3 pts | Sprint 2 |
| US12 | Visualisation des Tâches (Kanban/Liste) | Haute | 2 pts | Sprint 2 |
| US13 | Vue des Tâches Assignées | Moyenne | 2 pts | Sprint 2 |
| US14 | Suivi du Temps | Moyenne | 2 pts | Sprint 3 |
| US15 | Création de Tags et Releases | Basse | 2 pts | Sprint 3 |
| US16 | Historique des Releases | Basse | 2 pts | Sprint 3 |
| US17 | Création de Cas de Test | Moyenne | 2 pts | Sprint 3 |
| US18 | Exécution d'un Cas de Test | Moyenne | 2 pts | Sprint 3 |
| US19 | Tableau de Bord des Tests | Moyenne | 2 pts | Sprint 3 |
| US20 | Création et Édition de Documentation | Moyenne | 2 pts | Sprint 3 |
| US21 | Organisation de la Documentation | Moyenne | 2 pts | Sprint 3 |
| US22 | Liaison Documentation et Issues | Basse | 2 pts | Sprint 3 |
| US23 | Déployer l'application | Haute | 3 pts | Sprint 3 |

**Total estimé:** 60 points  
**Sprints planifiés:** 3  
**Sprint actuel:** Sprint 3 (19/11 au 03/12)

---

## Documentation détaillée

- **User Stories complètes:** [Sprint0/Sprint0.md](Sprint0/Sprint0.md)
- **Tâches par US:** [Sprint0/US_Tasks.md](Sprint0/US_Tasks.md)
- **Documentation utilisateur:** [docs/User.md](docs/User.md)
- **Documentation admin:** [docs/Admin.md](docs/Admin.md)
- **Documentation développeur:** [https://github.com/Tourlat/Conduite_de_projet_2025_Dev](https://github.com/Tourlat/Conduite_de_projet_2025_Dev) Nous avons laissé la documentation développeur sur notre repo github de développement.

---

## Planification des Sprints

---

### Sprint 1 (25/10 au 05/11)

**Objectifs:**
- Permettre aux utilisateurs de créer un compte et se connecter
- Permettre la création de base d'un projet
- Permettre la gestion du profil utilisateur

**Équipe:**
- **Scrum Master:** Kenzo
- **Développeurs Backend:** Félix, Justus
- **Développeurs Frontend:** Félix, Kenzo

**Tâches prévues:**

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



**Coût total:** 14 points  

---

### Sprint 2 (06/11 au 19/11)

**Objectifs:**
- Gérer la structure et les membres d'un projet
- Gestion complète des issues et tâches
- Visualisation du backlog et des tâches (Kanban/Liste)

**Équipe:**
- **Scrum Master:** Justus
- **Développeurs Backend:** Félix, Justus
- **Développeurs Frontend:** Félix, Kenzo

**Tâches prévues:**

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

**Coût total:** 25 points

---

### Sprint 3 (20/11 au 03/12)

**Objectifs:**
- Ajouter la gestion des releases et tags pour les projets.
- Ajouter la gestion des cas de test avec création, exécution.
- Mettre en place un système de gestion de la documentation avec création, édition.
- Mettre à jour la documentation utilisateur, admin et développeur pour notre projet.
- Déployer l'application.

**Équipe:**
- **Scrum Master:** Félix
- **Développeurs Backend:** Félix, Justus
- **Développeurs Frontend:** Félix, Kenzo

**Tâches prévues:**

#### US14 à US16 : Releases
- T14.1 : Ajouter les champs de temps estimé/passé à la base de données et API (PUT /tasks/:id/time) - 1 point
- T14.2 : Créer l'interface de saisie du temps (front-end) - 1 point
- T15.1 : Développer l'API de création de releases (POST /projects/:id/releases) - 1 point
- T15.2 : Créer l'interface de création de release/tag (front-end) - 1 point
- T16.1 : Développer l'API d'historique des releases (GET /projects/:id/releases) - 1 point
- T16.2 : Créer la vue timeline des releases (front-end) - 1 point

#### US17 à US19 : Tests
- T17.1 : Développer l'API pour sauvegarder les cas de tests (POST /projects/:id/test-cases) - 1 point
- T17.2 : Créer le formulaire de création de cas de test (front-end) - 1 point
- T18.1 : Développer l'API pour modifier des tests (POST /test-cases/:id/update-tests) - 1 point
- T18.2 : Créer l'interface d'exécution et mise à jour des résultats (front-end) - 1 point
- T19.1 : Développer l'API pour get les tests (GET /projects/:id/tests) - 1 point
- T19.2 : Créer le dashboard des tests avec graphiques (front-end) - 1 point

#### US20 à US22 : Documentation
- T20.1 : Développer l'API CRUD pour la documentation (POST/PUT/GET/DELETE /projects/:id/docs) - 1 point
- T20.2 : Créer l'éditeur Markdown pour la documentation (front-end) - 1 point
- T21.1 : Implémenter le système de catégories/sections pour la documentation (base de données + API) - 1 point
- T21.2 : Créer la navigation arborescente de la documentation (front-end) - 1 point
- T22.1 : Développer l'API de liaison documentation-issues (POST /docs/:id/link-issue) - 1 point
- T22.2 : Créer l'interface de liaison dans l'éditeur de documentation (front-end) - 1 point

#### US23 : Déployer l'application

**Coût total:** 21 points

---

## Conventions

- **Priorité:** Haute | Moyenne | Basse
- **Estimation:** Points de complexité (1-5)

