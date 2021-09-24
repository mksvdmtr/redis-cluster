## Ansible playbook для настройки redis cluster из 6 нод

#### Запуск:
 - Заполнить переменные в файле inventory:

```
redis-1 ansible_host=10.110.0.10 ansible_user=user
```
 - Запустить плейбук:
```
ansible-playbook -i inventory redis.yml --ask-become-pass
ввести пароль от пользователя которого указали в inventory
```

Ansible 2.11.3