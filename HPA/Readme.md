# Download the Metrics-server

`wget -O metricserver.yml https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml`

# Open the metricserver.yml under spec.args add this line

`- --kubelet-insecure-tls`

# Run the Metrics server

`kubectl apply -f metricserver.yml`

# Create Deployment and apply HPA Using the Below Command 

`kubectl autoscale deployment <deployment-name> --cpu-percent=10 --min=1 --max=10`
  
# To list the of HPA
  
`kubectl get hpa`
  
# Now go inside the Pod and perform some actions the cpu will increase and it will spin up the new Pods 
  
