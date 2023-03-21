Instructions

      docker build -t <your tag name> .
  docker push to your docker registry if needed
  update any config values(pushed image name) in deployment.yaml
      kubectl apply -f deployment.yaml
      kubectl get pods
      kubectl exec <mediawiki pod name> -- /var/config/setup.sh
