# Run `nginx-php-user_playbook.yml`
Для настройки адреса php-fpm при запуске playbook'а нужно аргументом задать ip
Пример:
```sh
ansible-playbook nginx-php-user_playbook.yml -vvv --ask-become-pass --extra-vars "php_ip=172.17.7.192"
```
