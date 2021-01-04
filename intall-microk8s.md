#Install microk8s 
sudo snap install microk8s --classic

#Enable add-ons from microk8s
microk8s enable dashboard dns registry istio prometheus

#Enabe user mod for microk8s
sudo usermod -a -G microk8s your-user

sudo chown -f -R your-user ~/.kube



