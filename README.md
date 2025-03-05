# Helm
____________________________________________________________________

📌 Install the Chart

helm install Haku . 

📌 Update Image for Only app2

helm upgrade Haku ./Haku-chart --set apps.app2.image=dev.azurecr.io/billing-ms:Development-2025.02.10

📌 Verify Deployment

kubectl get pods -n pz-dev-api -o wide

📌 Uninstall the Chart

helm uninstall Haku
