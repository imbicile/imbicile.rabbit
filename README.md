# Действия

Установка последней версии RabbitMQ https://www.rabbitmq.com/ из репозитария https://packagecloud.io/

Так как в родном репозитарии поломаны зависимости то добавляется репозитарий erlang https://www.erlang-solutions.com

## Роль проверялась на дистрибутиве
```
Description: Ubuntu 20.04.2 LTS
Release: 20.04
Codename: focal
```

## Переменные

ЗАводимые пользователи с паролями задаются в файле `roles/imbicile.rabbit/defaults/main.yml`

## inventory

В файле инвентаря задаются адреса хостов `ip:port` где необходимо развернуть роль https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html

## Подготовка

```bash
sudo apt install git python3-pip -y
git clone https://github.com/imbicile/imbicile.rabbit.git
cd imbicile.rabbit/
pip3 install -r requirements.txt
```

## Использование

Для установки на локальных хост

```bash
~/.local/bin/ansible-playbook playbooks/rabbit_local.yml
```

Для установки на хост в сети

```bash
 ~/.local/bin/ansible-playbook playbooks/rabbit_hosts.yml
```
