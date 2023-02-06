## 08-ansible-02-playbook

## Описание

Playbook устанавливает на 2 машины (ОС из семейства RedHat, CentOS, Fedora, Oracle Linux) с доступом по ssh  - пакеты ПО Clickhouse и Vector

## Параметры

В group_vars/clickhouse/vars.yml и group_vars/vector/vars.yml  задаются соответственно версии Clickhouse и Vector.

В inventory/prod.yml задаются хосты для установки и доступы к ним

group_vars/clickhouse/vars.yml

| Имя           | Значение по умолчанию | Описание                        |
| -------------- | ------------- | -----------------------------------|
| `clickhouse_version` |  "22.3.3.44" | Версия Clickhouse |
| `clickhouse_packages` |    - clickhouse-client  - clickhouse-server  - clickhouse-common-static | Пакеты Clickhouse для установки |


## Теги

Тегирование --tags clickhouse или --tags vector позволяет выполнить задачи по установке по-отдельности
