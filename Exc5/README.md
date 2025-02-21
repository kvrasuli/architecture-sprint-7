#### Управление трафиком

- Назначение меток
```
kubectl run front-end-app --image=nginx --labels role=front-end --expose --port 80
kubectl run back-end-api-app --image=nginx --labels role=back-end-api --expose --port 80
kubectl run admin-front-end-app --image=nginx --labels role=admin-front-end --expose --port 80
kubectl run admin-back-end-api-app --image=nginx --labels role=admin-back-end-api --expose --port 80
```
- Применение сетевых политик
```
kubectl apply -f non-admin-api-allow.yaml
kubectl apply -f admin-api-allow.yaml
```