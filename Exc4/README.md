#### Управление трафиком

- Создание юзеров
```
kubectl create serviceaccount ivanov
kubectl create serviceaccount petrov
kubectl create serviceaccount sidorov
```
- Создание ролей
```
kubectl apply -f roles.yaml
```
- Назначение ролей пользователям
```
kubectl apply -f role_bindings.yaml
```
