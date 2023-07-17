1) В работе используются:


     Ubuntu 20.04.
     GitLab.
     Docker Hub.



2) Перед созданием ВМ в Terraform создаем файл variables.tf с указанием данных для подключения к облаку. Имена переменных указаны в файле main.tf


3) Проверяем правильность указания адресов машин в Ansible Inventory


4) После развертывания инфраструктуры с помощью Ansible, регистрируем Runner на Gitlab c помощью команды gitlab-runner register

5) Для корректной работы kubectl на srv берем содержимое файла /etc/kubernetes/admin.conf с мастера kubernetes и копируем его в такой же файл на srv.
