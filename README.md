
```
kubectl apply -f namespace.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

либо `kubectl apply -f .` но надо выполнить 2 раза тк NS созджается с задержкой

### Result

GET http://arch.homework/health/

или

GET http://localhost/health/


### "🧹 Очистка предыдущих ресурсов..."
```
kubectl delete -f . --ignore-not-found=true
kubectl delete namespace health-service --ignore-not-found=true
```
