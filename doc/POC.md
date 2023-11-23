# ArgoCD: Get Default (Initial) Admin Password

To print the initial ArgoCD password, execute the following command:

`kubectl -n argocd get secret argocd-initial-admin-secret -o jsonpath="{.data.password}" | base64 -d; echo`

Port-forwarding

`kubectl port-forward svc/argocd-server -n argocd 8080:443`

Get access

> https://localhost:8080/

# DEMO
![Image](../demo3.gif)
