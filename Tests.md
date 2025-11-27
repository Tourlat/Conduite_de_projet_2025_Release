# Tests

### Tests Backend:

- Test d'Intégration avec les controllers, services et repositories et un docker container pour la base de données

### Tests Frontend:

- Frontend tests
    * Tests unitaires et d’intégration réalisés avec Vitest et Vue Test Utils:
        * Vérification du rendu des composants
        * Validation des événements et état réactifs
        * Simulation d’action utilisateur
        * Composants isolés / comlexes
        * Services API

- CI/CD
    * Github workflows qui exécutent les tests frontend et backend automatiquement pour chaque pull request et chaque push/commit sur la branche main
