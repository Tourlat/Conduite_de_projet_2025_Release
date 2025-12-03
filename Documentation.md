## Documentation

### Documentation pour les utilsateurs :
- Voir [User.md](docs/User.md)

### Documentation pour les admin :
- Voir [Admin.md](docs/Admin.md)

### Documentation pour les développeurs :

- Voir [https://github.com/Tourlat/Conduite_de_projet_2025_Dev](https://github.com/Tourlat/Conduite_de_projet_2025_Dev).
  
- Frontend : excuter `npm run doc` dans le dossier `frontend` pour générer la documentation avec TypeDoc. La documentation sera générée dans le dossier `frontend/docs/gen`.

- Backend : 
    - La documentation des points de terminaison (endpoints) du backend est disponible sous forme de spécification OpenAPI dans backend/docs/openapi.json.

    - Pour régénérer la spécification OpenAPI, exécutez la commande suivante. Assurez-vous que la variable d'environnement API_DOCS_ENABLED est définie sur true dans .env et que l'application est en cours d'exécution.

    `mvn -DskipTests springdoc-openapi:generate`

    - Pour accéder à la documentation Swagger, démarrez l'application backend et rendez-vous à l'URL suivante dans votre navigateur: `http://localhost:8080/swagger-ui/index.html`.
