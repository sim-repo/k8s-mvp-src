git add . && git commit -m "f" && git push
helm package ./redis .
helm repo index .

docker image prune --all

helm upgrade --dry-run --debug --install some ./cart


kubectl get gateway -n prod

kubectl get svc istio-ingressgateway -n istio-system
kubectl get VirtualService -n prod