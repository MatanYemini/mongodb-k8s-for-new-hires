# Mongodb k8s

Helping new hires to understand k8s with MongoDB example.
Full description of steps is under the company's property :) 

## k8s Notes

* Need to generate secret before pointing on it in the mongo deployment configuration
* `kubectl apply -f ./k8s/mongo-secret.yml`

* Need to apply the deployment cfg (includes the service as well. In k8s they go together usually)
* `kubectl apply -f ./k8s/mongo.yml`

* Check that mongo-service is running
* `kubectl describe service mongodb-service`

* Adding deployment for mongo-express for admin UI


