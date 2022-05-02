# 08-ansible-03-yandex

## Что делает playbook

Плейбук развернёт три приложения на разных хостах:

- Clickhouse
- Lighthouse	
- Vector

## Какие у него есть параметры

- Все приложения будут установлены из RPM-пакетов.
- IP хостов нужно задать в файле инвентаризации [prod.yml](playbook/inventory/prod.yml)
- Изменить переменные для соответствующих приложений, можно в файлах находящихся в одноимённых папках [group_vars](playbook/group_vars).
- Изменить конфиги приложений можно в дирректории [templates](playbook/templates)

## Для веб доступа к БД clickhouse

- После установки необходимо в строке браузера указать IP адрес сервера clickhouse-02
- После перехода на сайт необходимо указать IP адрес сервера clickhouse-01
