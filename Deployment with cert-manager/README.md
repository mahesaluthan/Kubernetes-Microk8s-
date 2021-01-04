- apply the 00-deployment and 01-ingress
- if you use kubernetes exec microk8s you should apply this  kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.34.1/deploy/static/provider/do/deploy.yaml
  or you can use mandatory select one of that kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/nginx-0.30.0/deploy/static/mandatory.yaml
  if use microk8s u dont need used that, you just enable the ingress from microk8s microk8s enable ingress
- install the certbot kubectl apply --validate=false -f https://github.com/jetstack/cert-manager/releases/download/v0.16.1/cert-manager.yaml
- next you apply 03-issuer
- after that apply 04-cert to change the ingress