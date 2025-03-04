# Helm
____________________________________________________________________

📌 Install the Chart

helm install multi-app ./multi-app-chart --namespace pz-dev-api

📌 Update Image for Only app2

helm upgrade multi-app ./multi-app-chart --set apps.app2.image=pzdevcr.azurecr.io/billing-ms:Development-2025.02.10

📌 Verify Deployment

kubectl get pods -n pz-dev-api -o wide
