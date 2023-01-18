## How to run 🚀
### Locally:
1. Install [Docker](https://docs.docker.com/get-docker/) and [Docker Compose](https://docs.docker.com/compose/install/)
2. Run local-script.sh
3. From your browser, open localhost:9001. You should be able to connect to webserver. 

### On Kubernetes:
1. Install [Kubernetes](https://kubernetes.io/docs/tasks/tools/install-kubectl/) and [Helm](https://helm.sh/docs/intro/install/)
2. Run kubernetes-script.sh
3. Expose by nodeport or ingress the service of the application
----

## 📄 Documentation 📄
### Backend:
Is a node.js application with express framework, it creates a client communication with a redis cache instance and has methods to SET, DEL or GET keys from the cache.
### Frontend:
Is at the root path of the application exposing a html file with scripts to fetch the endpoints of the backend.
### Redis:
Is a redis cache instance exposed without credentials.
