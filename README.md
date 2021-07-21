

Kubernetes-demo

This is the simple example of kubernetes deployment of mongodb(It is database) and mongo-express( It is MongoDB admin interface ).
## Run Locally

Clone the project

```bash
  git clone https://github.com/Gauravkumar2701/Kubernetes-demo.git
```

Go to the project directory

```bash
  cd Kubernetes-demo
```
To run in local kubernetes cluster(such as in minikube case) run the following command:
```bash
kubectl apply -f secrets.yaml
kubectl apply -f ConfigMap.yaml
kubectl apply -f mongodb-deployment.yaml
kubectl apply -f mongodb-express-deployment.yaml
```

To access the mongo-express from external
```bash
1. minikube service [service name (In our case it "mongo-express-service" which you can see in the mongo-express-deployment.yaml file)] 

Note: Here i used minikube to setup my local kubernetes cluster if you are using any other tool then accessing the minikube service [service name] command will vary.

2.It automatically open a browser in your system and you can manage you database with the mongo-express.
```

  
For any further information you can ping me here https://www.linkedin.com/in/gaurav-kumar-1314748a/