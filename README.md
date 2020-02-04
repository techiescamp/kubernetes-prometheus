# kubernetes-prometheus
Configuration files for setting up prometheus monitoring on Kubernetes cluster.

You can find the full tutorial from here https://devopscube.com/setup-prometheus-monitoring-on-kubernetes/

# Fork Adjustments

In this fork, I have modified the service by removeing the nodePort, also I have added an Ingress to map in port 80/443 to the prometheus container. In this case, I find it easier than nodePorts.

Additionally, a Pull request was issued to modify the Deployment to support apps/v1 in K8s 1.16.x - and remove the image tag to automatcally support "latest".