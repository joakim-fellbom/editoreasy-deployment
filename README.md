![image](https://github.com/user-attachments/assets/a9ddf989-ff37-444a-bc6b-119c256d6b87)
![image](https://github.com/user-attachments/assets/ce6a8231-671b-4c1e-9755-8779a3da937b)

Le déploiement sur ArgoCD a l'air de fonctionner correctement mais l'URL, il semblerait que le domaine n'existe pas publiquement.

Test sur le Terminal VSCode de l'application sur le SSPCloud :  

(base) onyxia@vscode-python-739592-0:~/work/editoreasy-showcase$ kubectl describe ingress vite-frontend
Name:             vite-frontend
Labels:           argocd.argoproj.io/instance=vite-frontend
Namespace:        user-joakimfellbom
Address:          10.233.1.91
Ingress Class:    nginx
Default backend:  <default>
Rules:
  Host                                                  Path  Backends  
  vite-frontend.user-joakimfellbom.cloud.sp5.onyxia.io  
                                                           vite-frontend:80 (10.233.115.77:4173)
Annotations:                                            nginx.ingress.kubernetes.io/rewrite-target: 
Events:                                                 <none>


