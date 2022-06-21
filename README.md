# playdate-api
PlayDate API - Node.js, Express, MongoDB, k8s environment 

## k8s Notes

* Need to generate secret before pointing on it in the mongo deployment configuration
* `kubectl apply -f ./k8s/mongo-secret.yml`

* Need to apply the deployment cfg (includes the service as well. In k8s they go together usually)
* `kubectl apply -f ./k8s/mongo.yml`

* Check that mongo-service is running
* `kubectl describe service mongodb-service`

* Adding deployment for mongo-express for admin UI


