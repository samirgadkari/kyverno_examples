# Testing on minikube did not work

1. kubectl create ns production
2. kubectl create -f require-pod-requests-and-limits.yaml
3. kubectl create -f pod-without-limits.yaml
4. kubectl create -f pod-with-limits.yaml

Step 4 should have worked, but we still get the error that the
validate-resource-limits rule failed.
