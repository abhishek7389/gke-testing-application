# Gke-testing-application

To deploy the application into the cluster 

Step 1. Get credential for your cluster
```
gcloud container clusters get-credentials bank-of-anthos \
  --project=<your project id> --region=<your region>
```

Step 2. Changing directory to the deployment folder
```
cd gke-testing-application
```

Step 3. Deploy the application to the GKE Cluster
```
kubectl apply -k .
```

Step 4. Validate the deployment of application(Note: If you've deployed the application in a specifc namespace then please mention it accordingly)
```
kubectl get all 
```

