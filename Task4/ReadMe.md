# Запуск и проверка

1. Поднимим пустой Minikube. 
2. Запустим скрипт для создания пользователей.
```bash
chmod +x create-users.sh
./create-users.sh
```
3. Все роли записаны в один файл:  roles.yaml. 
```bash
kubectl apply -f roles.yaml
```
4. Все привязки пользователей к ролям сохранены в файле: rolebinding.yaml
```
kubectl apply -f rolebindings.yaml
```