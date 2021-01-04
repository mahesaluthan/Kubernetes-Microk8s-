1.Install microk8s 
sudo snap install microk8s --classic

2.Enable add-ons from microk8s
microk8s enable dashboard dns registry istio prometheus

3.Enabe user mod for microk8s
sudo usermod -a -G microk8s your-user
sudo chown -f -R your-user ~/.kube



