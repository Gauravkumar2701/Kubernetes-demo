This is the simple example of kubernetes deployment of mongodb(It is database) and mongo-express( It is MongoDB admin interface ).

To run in local kubernetes cluster(such as minikube) run the following command: :-)
 
 1. kubectl apply -f secrets.yaml
 2. kubectl apply -f ConfigMap.yaml
 3. kubectl apply -f mongodb-deployment.yaml
 4. kubectl apply -f mongodb-express-deployment.yaml

To access the mongo-express from external :-)

    1. minikube service [service name (In our case it "mongo-express-service" which you can see in the mongo-express-deployment.yaml file)] 

    Note: Here i used minikube to setup my local kubernetes cluster if you are using any other tool then accessing the minikube service [service name] command will vary.

    2.It automatically open a browser in you system and you can manage you database with the mongo-express.

    

For any further information you can ping me here https://www.linkedin.com/in/gaurav-kumar-1314748a/