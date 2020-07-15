From the root of the node-docker directory, build container:
```
docker build -t node-docker .
```

From the root of the node-docker directory, run the service:
```
docker-compose run --rm --service-ports nod_dev_env
```

In the container shell, initialize the Node project and install dependencies by issuing the following commands (if you prefer, use npm):
```
yarn init -y
yarn add express
yarn add -D nodemon
```

To test the server, visit http://localhost:8080/ in your local browser.

Reference links for better explaination and further information:
* [Use Docker to create a node development environment](https://auth0.com/blog/use-docker-to-create-a-node-development-environment)
* Le même article backupé: [Utiliser Docker pour créer un environnement de développement Node JS](http://devfrontend.info/dockernodejs-utiliser-docker-pour-creer-un-environnement-de-developpement-nodejs/)
