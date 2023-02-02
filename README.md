# 08-ansible-02-playbook

Подготовьте README.md файл по своему playbook. В нём должно быть описано: что делает playbook, какие у него есть параметры и теги.

#Что делает playbook

Playbook устанавливает на 2 машины (ОС из семейства RedHat, CentOS, Fedora, Oracle Linux) с доступом по ssh  - пакеты ПО Clickhouse и Vector

#Параметры

В group_vars/clickhouse/vars.yml и group_vars/vector/vars.yml  задаются соответственно версии Clickhouse и Vector
В inventory/prod.yml задаются хосты для установки и доступы к ним

#Теги

Тегирование --tags clickhouse и --tags vector позволяет выполнить задачи по установке по-отдельности
