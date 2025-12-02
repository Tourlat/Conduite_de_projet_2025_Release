# Manuel Utilisateur - Gestion de Projet

Bienvenue dans la documentation utilisateur de notre application de gestion de projet. Ce guide vous expliquera comment utiliser les différentes fonctionnalités de l'application pour gérer efficacement vos projets.

Notre application permet de gérer Issues, Tasks, Tests, Documentation et Releases dans un environnement collaboratif.

## Démonstration Vidéo

Pour un aperçu rapide des fonctionnalités, vous pouvez visionner notre vidéo de démonstration :

![Démonstration Vidéo](video_demo_cdp.webm)


---

## Premiers Pas

### 1. Authentification
Pour accéder à l'application, vous devez vous connecter ou créer un compte.

*   **Inscription** : Cliquez sur "S'inscrire", remplissez votre nom, email et mot de passe.
*   **Connexion** : Utilisez vos identifiants pour accéder à votre tableau de bord personnel.

### 2. Tableau de Bord (Dashboard)
Une fois connecté, vous arrivez sur votre tableau de bord. Ici, vous pouvez voir :
*   La liste de vos projets existants.
*   Un bouton pour créer un nouveau projet.
*   Un aperçu rapide de votre profil.
*   Modifier vos paramètres utilisateur (mot de passe, email et nom).

---

## Gestion des Projets

### Créer un Projet
1.  Cliquez sur le bouton **"Nouveau Projet"** depuis le tableau de bord.
2.  Remplissez le nom du projet, une description et définissez une clé (identifiant court).
3.  Validez pour créer l'espace de travail.

### Détails du Projet
En cliquant sur un projet, vous accédez à sa vue détaillée qui comprend plusieurs onglets :
*   **Vue d'ensemble** : Statistiques et informations générales.
*   **Membres** : Gestion de l'équipe.
*   **Issues** : Liste des tickets et tâches.
*   **Sprints** : Gestion des cycles de développement.
*   **Paramètres** : Modification ou suppression du projet.

---

## Gestion des Tickets (Issues)

Les "Issues" représentent les features, bugs ou fix à réaliser dans le projet. Voici comment les gérer :

*   **Créer une Issue** : Dans l'onglet "Issues" ou "Backlog", cliquez sur "Créer une issue". Définissez un titre, une description, une priorité (Basse, Moyenne, Haute) et une estimation (Story Points).
*   **Modifier/Assigner** : Cliquez sur une issue pour voir les détails, changer son statut (À faire, En cours, Terminé) ou l'assigner à un membre de l'équipe.
*   **Tâches** : Vous pouvez découper une issue en plusieurs **tâches** plus petites pour un suivi plus fin.
*   **Supprimer** : Possible si vous êtes le créateur du projet.

---

## Planification (Backlog & Sprints)

### Le Backlog
Le Backlog rassemble toutes les tâches à faire qui ne sont pas encore planifiées dans un sprint actif. C'est votre réservoir de travail.

### Les Sprints
Les Sprints sont des périodes de temps (ex: 2 semaines) durant lesquelles l'équipe s'engage à terminer un ensemble de tickets.

1.  **Créer un Sprint** : Allez dans l'onglet "Sprints", cliquez sur "Créer un Sprint". Définissez un nom et des dates de début/fin.
2.  **Planifier** : Ajoutez des issues du Backlog vers votre Sprint.
3.  **Démarrer/Terminer** : Un sprint peut être "Planifié", "En cours" (Actif) ou "Terminé".
    *   Le statut du sprint change automatiquement selon les dates ou peut être géré manuellement.
    *   Vous pouvez suivre l'avancement grâce aux indicateurs (nombre d'issues, points d'effort).

---

## Gestion d'Équipe

Dans l'onglet **Membres** d'un projet :
*   Invitez des collaborateurs par leur email ou nom d'utilisateur.
*   Retirez des membres si nécessaire.

---

## Tests

L'application intègre un système complet de tests pour valider le code de vos issues.

### Tests JavaScript pour les Issues

Chaque issue peut avoir son propre **playground de tests JavaScript** accessible depuis la page de détails de l'issue.

#### Fonctionnalités

*   **Éditeur de Code** : Écrivez votre code JavaScript dans un éditeur dédié.
*   **Éditeur de Tests** : Rédigez vos tests unitaires pour valider le code.
*   **Exécution Sandbox** : Les tests s'exécutent dans un Web Worker isolé (sandbox) avec un timeout de 5 secondes pour éviter les boucles infinies.
*   **Résultats Détaillés** : Après exécution, visualisez :
    *   Le nombre de tests réussis/échoués
    *   Les logs de console
    *   Les messages d'erreur avec stack traces
*   **Sauvegarde** : Enregistrez vos tests pour les réutiliser plus tard.
*   **Import/Export** : Importez du code depuis des fichiers ou téléchargez vos tests.
*   **Historique** : Consultez et rechargez les tests sauvegardés précédemment.

#### Utilisation

1.  Accédez à une issue depuis votre projet.
2.  Cliquez sur l'onglet ou le bouton **"Tests"**.
3.  Écrivez votre code et vos tests dans les éditeurs respectifs.
4.  Cliquez sur **"Exécuter les tests"** pour lancer la vérification.
5.  Consultez les résultats affichés en dessous.
6.  Utilisez **"Sauvegarder ce test"** pour conserver votre travail.

---

## Documentation

Chaque projet peut avoir sa propre **documentation** accessible via l'onglet "Documentation".

### Créer et Éditer
*   Cliquez sur **"Nouveau Document"** pour créer une page.
*   Remplissez le titre et rédigez le contenu en **Markdown**.
*   L'aperçu en temps réel vous montre le rendu final.
*   Vous pouvez **lier des issues** au document pour tracer la documentation avec les tâches du projet.

### Consulter
*   Les documents sont affichés sous forme de cartes.
*   Cliquez sur une carte pour voir le contenu complet.
*   Modifiez ou supprimez les documents selon vos besoins.

---

## Releases (Versions)

L'onglet **Releases** vous permet de créer des versions de votre logiciel, en regroupant les tickets terminés et en marquant une étape importante du projet. Le versionning suit le format MAJEUR.MINEUR.PATCH (ex: 1.0.0).
