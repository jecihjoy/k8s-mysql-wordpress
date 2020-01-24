###Deploy wordpress and mysql using kubernetes
Ensure you've installed minikube then run the following commands
1. minikube start
2. kubectl create -f volumes.yaml 
3. kubectl create -f mysql.yaml 
4. kubectl create -f wordpress.yaml

This should setup all the volumes, services and pods(containers) needed.

5. minikube service wordpress --url

Copy the echoed url and open it in a browser. This should take you to the setup page of wordpress