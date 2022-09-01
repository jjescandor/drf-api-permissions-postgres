## LAB - Class 32

#### Project: Django REST Framework/Docker/Posgresql
#### Author: JJ Escandor

#### Description
 - This is project introduces Django Rest Framework, Docker, Postgresql

### Run the app
 - source .venv/bin/activate
 - docker compose up -d
 - go to http://0.0.0.0:8000/admin/ in the browser
 - admin username: code01 password: ASDFzxcv!@34 

### Features - General
-You have been supplied with two demos, each presenting a key new feature.
-One demonstrates how to restrict access to portions of your APIs data.
-The other demonstrates switching over to using postgres vs sqlite
-Your job is to merge the functionality of both demos.
-Customize your project to use different application features/models than what was used in demos.

### Features - Django REST Framework
- Make your site a DRF powered API as you did in previous lab.
- Adjust project’s permissions so that only authenticated user’s have access to API.
- Add a custom permission so that only appropriate users can update or delete it.
- Exactly what this means will depend on your application, so if you have any questions about “appropriate users” means reach out to TA/Instructor.
- Add ability to switch user’s directly from browsable API.

### Features - Docker
- create Dockerfile based off python:3.10-slim
- create docker-compose.yml to run Django app as a web service.
- enter docker-compose up --build to start your site.
- add postgres as a service
- Go to browsable api and confirm site properly restricts users based on their permissions.

### Stretch Goals
- Add a volume to persist data when container is shut down.

### Tests
1. In order to run the test, go to settings.py, comment in the Database entry for sqlite3
1. Comment out database entry for posgtresql
1. run python3 manage.py test in the browser
