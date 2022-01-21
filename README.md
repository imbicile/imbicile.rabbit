# Действия

Установка последней версии RabbitMQ https://www.rabbitmq.com/ из репозитария https://packagecloud.io/

Так как в родном репозитарии поломаны зависимости то добавляется репозитарий erlang https://www.erlang-solutions.com

## Роль проверялась на дистрибутиве

Description:	Ubuntu 20.04.2 LTS
Release:	20.04
Codename:	focal

## inventory

В файле инвентаря задаются адреса хостов где необходимо развернуть роль https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html

## Подготовка

```bash
sudo apt install git python3-pip -y
pip3 install -r requirements.txt
git clone https://github.com/imbicile/imbicile.rabbit.git
cd imbicile.rabbit/
```

## Использование

```bash

```
