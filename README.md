# Descomplicando ArgoCD

argocd login localhost:8080 # Faz o login no ArgoCD

argocd add cluster minikube # Adiciona um cluster ao ArgoCD

argocd app create nginx-app --repo https://github.com/LuizSilva-1/kube-argoCD.git --path . --dest-server minikube --dest-namespace default

argocd app list # Lista os aplicativos

argocd app get nginx-app # Mostra o status do aplicativo

argocd app logs nginx-app --container nginx # Mostra os logs do aplicativo

argocd app sync nginx-app # Sincroniza o aplicativo com o repositório

![image](https://github.com/LuizSilva-1/kube-argoCD/assets/108982016/723c50dd-90e5-45ec-a935-79abac5d1e36)
