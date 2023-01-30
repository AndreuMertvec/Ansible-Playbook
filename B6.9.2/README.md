# Nginx + php-fpm role
При запуске playbook'а без аргументов, `documet_root` будет дефотным (`/var/www/html`)
```sh
ansible-playbook nginx_php_playbook.yml -vvv --ask-become-pass
```

Чтобы изменить `document_root` нужно при запуске добавить аргумент
```sh
ansible-playbook nginx_php_playbook.yml -vvv --ask-become-pass --extra-vars "document_root=/opt/nginx/ansible"
```
