# Запуск playbook'ов

## Запуск `create_user_playbook.yml`
Для расшифровки ключей надо добавить запрос на ввод `vault` пароля.
Команда запуска:
```sh
ansible-playbook create_user_playbook.yml -vvv --ask-become-pass --ask-vault-pass
```

## Запуск `postfix_playbook.yml`
Для установки `postfix`
```sh
ansible-playbook postfix_playbook.yml -vvv --ask-become-pass --tags "init postfix"
``` 
Для удаления `postfix`
```sh
ansible-playbook postfix_playbook.yml -vvv --ask-become-pass --tags "drop postfix"
```
