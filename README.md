# lab-09 JS401 - Lab-09 API-Server
## Author: Cory Henderson
This lab contains a running server and provides practice for documenting the server modules, functions, and classes. Jsdocs and Swagger are used to document functionality and API routes.

## Links and Resources
- [Github Repo](https://github.com/401-advanced-javascript-1/lab-09)

## Documentation
- [Jsdocs](localhost:3000/docs)
- [Swagger](https://editor.swagger.io/?_ga=2.173881315.1132580723.1553560602-1879537872.1553560602)

# Modules
- index.js
- v1.js
- app.js
- memory-model.js
- mongo-model.js
- categories-model.js
- 404.js
- 500.js
- model-finder.js
- players-model.js
- teams-model.js
- categories-model.js

# Setup
- .env requirements
    - MONGODB_URI=mongodb://localhost:27017/teams
    - PORT=3000 (for nodemon)
- Running the app:
    - Start mongo server (CLI command 'mongo')
    - Get record from DB (http get :3000/categories)
    - Post to DB (echo '{"category": "Electronics", "name": "Television", "display_name": "TV", "description": "Tool for watching shows" }' | http post :3000/categories)
    - Update DB (echo '{"category": "Electronics", "name": "Radio", "display_name": "Rad", "description": "Tool for watching shows" }' | http put :3000/categories{id})
    - Delete from DB (http delete :3000/categories/{id})

## Tests
- Testing for expected route endpoints is performed using jest.

## UML
- ![alt](https://github.com/401-advanced-javascript-1/lab-09/blob/submission/images/uml-get-post.JPG)
- ![alt](https://github.com/401-advanced-javascript-1/lab-09/blob/submission/images/uml-put.JPG)
- ![alt](https://github.com/401-advanced-javascript-1/lab-09/blob/submission/images/uml-delete.JPG)