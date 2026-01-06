cat ssh.key |
kubectl create secret generic flux-sops \
--namespace=flux-system \
--from-file=identity.agekey=/dev/stdin